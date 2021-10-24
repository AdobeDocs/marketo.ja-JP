---
unique-page-id: 45417125
description: 非ネイティブ Salesforce 統合用 Sales Insight - Marketo ドキュメント - 製品ドキュメント
title: 非ネイティブ Salesforce 統合用 Sales Insight
exl-id: a771ecdf-c610-44e4-9e93-7fdcc9d79f4b
source-git-commit: 73c5375c6e2ec3b2dce09595be1f61f302ff4c25
workflow-type: tm+mt
source-wordcount: '1300'
ht-degree: 96%

---

# 非ネイティブ Salesforce 統合用 Sales Insight {#sales-insight-for-non-native-salesforce-integrations}

Marketo アカウントが、カスタマイズされた統合または非ネイティブ統合によって Salesforce に接続されている場合は、このドキュメントを使用して Sales Insight を設定してください。

>[!PREREQUISITES]
>
>* Marketo インスタンスに対して有効になっている MSI 非ネイティブ機能が有効になっていない場合は、MSI の設定を開始する前に (この機能を購入した場合は、Marketo サポートまでご連絡ください [ ](https://nation.marketo.com/t5/support/ct-p/Support) 。この機能がまだ購入されていない場合は、カスタマーの成功管理者にお問い合わせください)。
>* [MSI パッケージが設定](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md)された Salesforce アカウント。
>* Marketo REST API が[正常に設定](https://developers.marketo.com/rest-api/)されている。公開されている CRUD API は、非ネイティブ同期を実行するための基盤となります。
>* オブジェクトと関係を理解するには、[このブログ記事](https://developers.marketo.com/blog/create-and-associate-leads-companies-and-opportunities-with-the-marketo-rest-api/)を参照してください。
>* 15 文字の大文字と小文字を区別するグローバルな一意の ID ではなく、18 文字の大文字と小文字を区別しないグローバルな一意の ID を表示するように Salesforce オブジェクトを設定します。


>[!NOTE]
>
>Marketo MSI 管理者パネルの REST API 設定は、非ネイティブ同期には使用できません。

## MSI の非ネイティブ同期を成功させるには、以下が必要です {#successful-non-native-sync-for-msi-requires-the-following}

1. Salesforce Sales User を Marketo に同期します。

   Salesforce Sales User は、Salesforce のリード／連絡先を所有する外部ユーザーです。この Salesforce Sales User 用に Marketo セールス担当者をアップサートする必要があります。セールス担当者のアップサートには、「*externalSalesPersonId*」フィールドが必須です。

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>Marketo「セールス担当者」フィールド</strong></td> 
   <td><strong>Salesforce「Sales User」フィールド</strong></td> 
   <td><strong>説明</strong></td> 
  </tr> 
  <tr> 
   <td>externalSalesPersonId</td> 
   <td>Salesforce Sales User の大文字小文字を区別しないグローバルな一意の ID</td> 
   <td><p>外部 Salsforce Sales User オブジェクトに対する Marketo セールス担当者レコードを特定します。</p><p>適切な関係が作成されるように、他のオブジェクトを同期する前に、まずセールス担当者を同期させる必要があります。</p></td> 
  </tr> 
 </tbody> 
</table>

セールス担当者向け API ドキュメント：[https://developers.marketo.com/rest-api/lead-database/sales-persons/](https://developers.marketo.com/rest-api/lead-database/sales-persons/)\
セールス担当者を同期するための API ドキュメント：[https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Sales_Persons/syncSalesPersonsUsingPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Sales_Persons/syncSalesPersonsUsingPOST)

1. Salesforce アカウントを Marketo に同期します。

   この Salesforce アカウント用に Marketo の企業をアップサートする必要があります。企業のアップサートには、「_externalCompanyId_」および「_externalSalesPersonId_」フィールドが必須です。

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>Marketo「企業」フィールド</strong></td> 
   <td><strong>Salesforce「アカウント」フィールド</strong></td> 
   <td><strong>説明</strong></td> 
  </tr> 
  <tr> 
   <td>externalCompanyId</td> 
   <td>Salesforce アカウントの大文字小文字を区別しないグローバルな一意の ID</td> 
   <td>外部 Salsforce アカウントオブジェクトに対する Marketo 企業レコードを特定します。</td> 
  </tr> 
  <tr> 
   <td>externalSalesPersonId</td> 
   <td>Salesforce Sales User の大文字小文字を区別しないグローバルな一意の ID</td> 
   <td>アカウント所有者である外部 Salesforce Sales User オブジェクトに対する Marketo 企業レコードを特定します。<br><br>また、Marketo 内で企業レコードを所有するセールス担当者に企業を関連付けるためにも使用されます。このフィールドを設定する前に、まずセールス担当者を同期させる必要があります。</td> 
  </tr> 
 </tbody> 
</table>

企業向け API ドキュメント：[https://developers.marketo.com/rest-api/lead-database/companies/](https://developers.marketo.com/rest-api/lead-database/companies/)\
`API documentation for syncing Companies:  [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Companies/syncCompaniesUsingPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Companies/syncCompaniesUsingPOST)`

1. Salesforce のリード／連絡先を Marketo に同期します。

   この Salesforce のリード／連絡先用に Marketo のリードをアップサートする必要があります。リードのアップサートには、「_externalPersonId_」、「_externalSalesPersonId_」および「_externalCompanyId_」フィールドが必須です。

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>Marketo「リード」フィールド</strong></td> 
   <td><strong>Salesforce「リード」／「連絡先」フィールド</strong></td> 
   <td><strong>説明</strong></td> 
  </tr> 
  <tr> 
   <td>externalPersonId</td> 
   <td>Salesforce のリード／連絡先の大文字小文字を区別しないグローバルな一意の ID</td> 
   <td>外部 Salsforce リード／連絡先オブジェクトに対する Marketo リードレコードを特定します。<br><br>これは、MSI 非ネイティブ用に導入された新しいフィールドです。</td> 
  </tr> 
  <tr> 
   <td>externalSalesPersonId</td> 
   <td>Salesforce Sales User の大文字小文字を区別しないグローバルな一意の ID</td> 
   <td>このリード／連絡先を所有する外部 Salesforce Sales User オブジェクトを特定します。<br><br>また、このリードを Marketo のセールス担当者と関連付けます。最初にセールス担当者を正しく同期させる必要があります。</td> 
  </tr> 
  <tr> 
   <td>externalCompanyId</td> 
   <td>Salesforce アカウントの大文字小文字を区別しないグローバルな一意の ID</td> 
   <td>リード／連絡先が属する外部 Salesforce アカウントオブジェクトを特定します。<br><br>また、このリードレコードを Marketo の企業と関連付けます。最初に Salesforce アカウントを正しく同期させる必要があります。</td> 
  </tr> 
 </tbody> 
</table>

リード向け API ドキュメント：[`https://developers.marketo.com/rest-api/lead-database/leads/`](https://developers.marketo.com/rest-api/lead-database/leads/)\
リードを同期するための API ドキュメント：[https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Leads/syncLeadUsingPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Leads/syncLeadUsingPOST)

1. Salesforce の商談を Marketo に同期します。

   この Salesforce の商談用に Marketo の商談をアップサートする必要があります。商談のアップサートには、「_externalOpportunityId_」、「_externalCompanyId_」および「_externalSalesPersonId_&#x200B;フィールドが必須です。

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>Marketo「商談」オブジェクトフィールド</strong></td> 
   <td><strong>Salesforce 「商談」オブジェクトフィールド</strong></td> 
   <td><strong>説明</strong></td> 
  </tr> 
  <tr> 
   <td>externalOpportunityId</td> 
   <td>Salesforce のリード／連絡先の大文字小文字を区別しないグローバルな一意の ID</td> 
   <td>外部 Salsforce 商談オブジェクトに対する Marketo 商談レコードを特定します。</td> 
  </tr> 
  <tr> 
   <td>externalCompanyId</td> 
   <td>Salesforce アカウントの大文字小文字を区別しないグローバルな一意の ID</td> 
   <td>この商談が属する外部 Salesforce アカウントオブジェクトを特定します。<br><br>最初に Salesforce アカウントを正しく同期させる必要があります。</td> 
  </tr> 
  <tr> 
   <td>externalSalesPersonId</td> 
   <td>Salesforce Sales User の大文字小文字を区別しないグローバルな一意の ID</td> 
   <td>この商談を所有する外部 Salesforce Sales User オブジェクトを特定します。 </td> 
  </tr> 
 </tbody> 
</table>

商談向け API ドキュメント：[`https://developers.marketo.com/rest-api/lead-database/opportunities/`](https://developers.marketo.com/rest-api/lead-database/opportunities/)\
`API documentation for syncing Opportunities:  [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Opportunities/syncOpportunitiesUsingPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Opportunities/syncOpportunitiesUsingPOST)`

1. Salesforce の連絡先ロールを Marketo に同期します。

   次に、Salesforce の商談の Salesforce 連絡先ロールは、Marketo 商談ロールを介して同期できます。商談ロールレコードには、「_externalOpportunityId_」、「_role_」および「_leadId_」フィールドが必須です。

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>Marketo「商談ロール」フィールド</strong></td> 
   <td><strong>Salesforce「連絡先ロール」フィールド</strong></td> 
   <td><strong>説明</strong></td> 
  </tr> 
  <tr> 
   <td>externalOpportunityId</td> 
   <td>Salesforce の商談の大文字小文字を区別しないグローバルな一意の ID</td> 
   <td>外部 Salsforce 商談オブジェクトに対する Marketo 商談ロールを特定します。<br><br>最初に Salesforce の商談を正しく同期させる必要があります。</td> 
  </tr> 
  <tr> 
   <td>leadId</td> 
   <td>該当なし、これは Marketo のリード ID になります</td> 
   <td>これは、同期された Salesforce 連絡先の Marketo リード ID になります。<br><br>連絡先が Marketo で同期されると、Salesforce の連絡先の大文字と小文字を区別しないグローバルな一意の ID を externalPersonId として使用し、Marketo REST API を使用して Marketo のリードをクエリできます。</td> 
  </tr> 
  <tr> 
   <td>role</td> 
   <td>Salesforce の連絡先の「ロール」フィールド</td> 
   <td>この商談の連絡先のロールを記述します。</td> 
  </tr> 
 </tbody> 
</table>

商談向け API ドキュメント：[`https://developers.marketo.com/rest-api/lead-database/opportunities/`](https://developers.marketo.com/rest-api/lead-database/opportunities/)\
`API documentation for syncing Opportunities:  [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Opportunities/syncOpportunitiesUsingPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Opportunities/syncOpportunitiesUsingPOST)`

1. 「最新の注目のアクション」／「MSI スコア」フィールドを SFDC に同期します。

   Salesforce オブジェクトが Marketo に正しく同期されると、MSI 機能を活用できるようになります。MSI の「最新の注目のアクション」／「スコア」フィールドは、リードの REST API で公開されます。これらのフィールドは、MSI によって計算され、読み取り専用です。

   Marketo のリードの「最新の注目のアクション」／「スコア」フィールドは、REST API リードエンドポイントを使用することで、定期的に Salesforce に同期される必要があります。_externalPersonId_ を filterType として使用し、Salesforce リード GUID に filterValue として渡して、このエンドポイントに Marketo リードをクエリします。

   | GET /rest/v1/leads.json?filterType=externalPersonId&amp;filterValues=salesforceLeadId1,salesforceLeadId2 |
   |---|

   これで、これらのフィールドの値を使用して、Salesforce のリード／連絡先オブジェクトに同期させることができます。

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>Marketo「リード」フィールド</strong></td> 
   <td><strong>Salesforce「リード」／「連絡先」フィールド</strong></td> 
   <td><strong>説明</strong></td> 
  </tr> 
  <tr> 
   <td>msiLastInterestingMomentType</td> 
   <td>ラベル：最新の注目のアクションのタイプ<br>名前：Last_Interesting_Moment_Type__c</td> 
   <td>リードの最新の注目のアクションのタイプ</td> 
  </tr> 
  <tr> 
   <td>msiLastInterestingMomentDate</td> 
   <td><p>ラベル：最新の注目のアクション発生日</p><p>名前：Last_Interesting_Moment_Date__c</p></td> 
   <td>リードの最新の注目のアクションの日付</td> 
  </tr> 
  <tr> 
   <td>msiLastInterestingMomentDesc</td> 
   <td><p>ラベル：最新の注目のアクションの詳細</p><p>名前：Last_Interesting_Moment_Desc__c</p></td> 
   <td>リードの最新の注目のアクションの説明</td> 
  </tr> 
  <tr> 
   <td>msiLastInterestingMomentSource</td> 
   <td><p>ラベル：最新の注目のアクションのソース</p><p>名前：Last_Interesting_Moment_Source__c</p></td> 
   <td>リードの最新の注目のアクションのソース</td> 
  </tr> 
  <tr> 
   <td>優先度</td> 
   <td><p>ラベル：エンゲージメント</p><p>名前：Priority__c</p></td> 
   <td>リードの優先度</td> 
  </tr> 
  <tr> 
   <td>relativeUrgency</td> 
   <td><p>ラベル：相対的緊急度の値</p><p>名前：Urgency_Value__c</p></td> 
   <td>リードの相対的緊急度</td> 
  </tr> 
  <tr> 
   <td>relativeScoring</td> 
   <td><p>ラベル：相対スコアの値</p><p>名前：Relative_Score_Value__c</p></td> 
   <td>リードの相対スコア</td> 
  </tr> 
 </tbody> 
</table>

リード REST API 向けドキュメント：[https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Leads/getLeadByIdUsingGET](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Leads/getLeadByIdUsingGET).

非ネイティブ同期を成功させるには、外部フィールドを適切に使用することが重要です。一部のビューにデータが表示されない場合は、特定のフィールドが正しく同期されていない可能性があります。例えば、アカウントの下にある MSI ウィジェットにリードのアクティビティや注目のアクションが表示されない場合、リードの企業かアカウントのどちらかが正しく同期されていない可能性があります。外部フィールドを指定してこのリードに対して GET リクエストを実行すると、リードが正しく同期されたかどうかを検証できます。また、Marketo の外部セールス担当者のメールは、Salesforce のそのユーザーのメールと一致する必要があります。メールが一致しない場合、Salesforce の「Marketo」タブにデータが表示されないことがあります。
