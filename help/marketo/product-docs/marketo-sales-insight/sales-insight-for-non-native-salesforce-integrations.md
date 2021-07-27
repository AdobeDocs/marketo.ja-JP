---
unique-page-id: 45417125
description: ネイティブ以外のSalesforce統合向けのSales Insight - Marketoドキュメント — 製品ドキュメント
title: ネイティブ以外のSalesforce統合に関するセールス・インサイト
exl-id: a771ecdf-c610-44e4-9e93-7fdcc9d79f4b
source-git-commit: 73c5375c6e2ec3b2dce09595be1f61f302ff4c25
workflow-type: tm+mt
source-wordcount: '1300'
ht-degree: 0%

---

# ネイティブ以外のSalesforce統合に関するセールス・インサイト {#sales-insight-for-non-native-salesforce-integrations}

Marketoアカウントが、カスタマイズされた、または非ネイティブの統合を通じてSalesforceに接続されている場合は、このドキュメントを使用してSales Insightを設定します。

>[!PREREQUISITES]
>
>* MSIの設定を開始する前に、Marketoインスタンスに対して有効になっている「MSI非ネイティブ」機能(まだ購入していない場合は、[Marketoサポート](https://nation.marketo.com/t5/support/ct-p/Support)にお問い合わせください。この機能をまだ購入していない場合は、カスタマーサクセスマネージャーにお問い合わせください)。
>* [MSIパッケージが設定されたSalesforceアカウント](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md)。
>* Marketo REST API [が正常にセットアップされました](https://developers.marketo.com/rest-api/)。 公開されたCRUD APIは、非ネイティブ同期の実行の基礎となります。
>* オブジェクトと関係を理解するために、[このブログ記事](https://developers.marketo.com/blog/create-and-associate-leads-companies-and-opportunities-with-the-marketo-rest-api/)を読んでください。
>* Salesforceオブジェクトを設定して、大文字と小文字を区別する15文字のグローバル一意識別子ではなく、大文字と小文字を区別しないグローバル一意識別子を18文字で表示するようにします。


>[!NOTE]
>
>Marketo MSI AdminパネルのREST API設定は、非ネイティブ同期には使用できません。

## MSIの非ネイティブ同期が正常に行われるには、次の条件が必要です {#successful-non-native-sync-for-msi-requires-the-following}

1. Salesforce Sales UserをMarketoに同期します。

   Salesforce Sales Userは、Salesforceでリード/連絡先を所有する外部ユーザーです。 Salesforce Sales User用にMarketoの営業担当者を更新する必要があります。 *externalSalesPersonId*&#x200B;フィールドは、営業担当者のアップサート用に必須です。

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>Marketo Sales Person Field</strong></td> 
   <td><strong>Salesforceの「Sales User」フィールド</strong></td> 
   <td><strong>説明</strong></td> 
  </tr> 
  <tr> 
   <td>externalSalesPersonId</td> 
   <td>Salesforce Salesユーザーは、大文字と小文字を区別しないグローバル一意の識別子を使用します。</td> 
   <td><p>外部のSalesforce Sales Userオブジェクトに対するMarketoのSales Personレコードを識別します。</p><p>適切な関係を作成するために、他のオブジェクトを同期する前に、営業担当者を最初に同期する必要があります。</p></td> 
  </tr> 
 </tbody> 
</table>

営業担当者向けAPIドキュメント：[https://developers.marketo.com/rest-api/lead-database/sales-persons/](https://developers.marketo.com/rest-api/lead-database/sales-persons/)\
営業担当者を同期するためのAPIドキュメント：[https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Sales_Persons/syncSalesPersonsUsingPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Sales_Persons/syncSalesPersonsUsingPOST)

1. SalesforceアカウントをMarketoに同期します。

   Marketoの会社は、Salesforceアカウント用に更新する必要があります。 _externalCompanyId_&#x200B;と&#x200B;_externalSalesPersonId_&#x200B;フィールドは、会社のアップサート用に必須です。

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>Marketo Company Field</strong></td> 
   <td><strong>Salesforceアカウントフィールド</strong></td> 
   <td><strong>説明</strong></td> 
  </tr> 
  <tr> 
   <td>externalCompanyId</td> 
   <td>Salesforceアカウントで大文字と小文字を区別しないグローバル一意の識別子</td> 
   <td>外部のSalesforceアカウントオブジェクトに対するMarketo会社レコードを識別します。</td> 
  </tr> 
  <tr> 
   <td>externalSalesPersonId</td> 
   <td>Salesforce Salesユーザーは、大文字と小文字を区別しないグローバル一意の識別子を使用します。</td> 
   <td>Marketo会社レコードを、アカウント所有者の外部Salesforce Sales Userオブジェクトに対して識別します。<br><br>また、Marketo内で会社を会社レコードを所有する営業担当者に関連付けるためにも使用します。このフィールドを設定する前に、販売担当者を最初に同期する必要があります。</td> 
  </tr> 
 </tbody> 
</table>

会社向けAPIドキュメント：[https://developers.marketo.com/rest-api/lead-database/companies/](https://developers.marketo.com/rest-api/lead-database/companies/)\
`API documentation for syncing Companies:  [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Companies/syncCompaniesUsingPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Companies/syncCompaniesUsingPOST)`

1. Salesforceのリード/連絡先をMarketoに同期します。

   Salesforceのリード/連絡先にMarketoリードを挿入する必要があります。 _externalPersonId_、_externalSalesPersonId_、_externalCompanyId_&#x200B;の各フィールドは、リードのアップサート用に必須です。

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>Marketoリードフィールド</strong></td> 
   <td><strong>Salesforceのリード/連絡先フィールド</strong></td> 
   <td><strong>説明</strong></td> 
  </tr> 
  <tr> 
   <td>externalPersonId</td> 
   <td>Salesforceリード/連絡先で大文字と小文字を区別しないグローバル一意の識別子</td> 
   <td>外部のSalesforceリード/連絡先オブジェクトへのMarketoリードレコードを識別します。<br><br>これは、MSI Non-Native用に導入された新しいフィールドです。</td> 
  </tr> 
  <tr> 
   <td>externalSalesPersonId</td> 
   <td>Salesforce Salesユーザーは、大文字と小文字を区別しないグローバル一意の識別子を使用します。</td> 
   <td>このリード/連絡先を所有する外部のSalesforce Sales Userオブジェクトを識別します。<br><br>また、リードとMarketoの営業担当者を関連付けます。営業担当者を最初に正しく同期する必要があります。</td> 
  </tr> 
  <tr> 
   <td>externalCompanyId</td> 
   <td>Salesforceアカウントで大文字と小文字を区別しないグローバル一意の識別子</td> 
   <td>リード/連絡先が属する外部Salesforce Accountオブジェクトを識別します。<br><br>また、リードレコードをMarketoの会社に関連付けます。Salesforceアカウントを最初に正しく同期する必要があります。</td> 
  </tr> 
 </tbody> 
</table>

リード向けAPIドキュメント：[`https://developers.marketo.com/rest-api/lead-database/leads/`](https://developers.marketo.com/rest-api/lead-database/leads/)\
リードを同期するためのAPIドキュメント： [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Leads/syncLeadUsingPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Leads/syncLeadUsingPOST)

1. Salesforce OpportunitiesをMarketoに同期します。

   Salesforce Opportunity用にMarketo Opportunityをアップサートする必要があります。 Opportunityのアップサートに対して、 _externalOpportunityId_ 、 _externalCompanyId_ 、 _externalSalesPersonId_&#x200B;の各フィールドが必須です。

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>Marketo Opportunity Object Field</strong></td> 
   <td><strong>Salesforce Opportunity Objectフィールド</strong></td> 
   <td><strong>説明</strong></td> 
  </tr> 
  <tr> 
   <td>externalOpportunityId</td> 
   <td>Salesforceリード/連絡先で大文字と小文字を区別しないグローバル一意の識別子</td> 
   <td>外部のSalesforce Opportunityオブジェクトに対するMarketo Opportunityレコードを識別します。</td> 
  </tr> 
  <tr> 
   <td>externalCompanyId</td> 
   <td>Salesforceアカウントで大文字と小文字を区別しないグローバル一意の識別子</td> 
   <td>このオポチュニティが属する外部Salesforce Accountオブジェクトを識別します。 <br><br>Salesforceアカウントを最初に正しく同期する必要があります。</td> 
  </tr> 
  <tr> 
   <td>externalSalesPersonId</td> 
   <td>Salesforce Salesユーザーは、大文字と小文字を区別しないグローバル一意の識別子を使用します。</td> 
   <td>このオポチュニティを所有する外部のSalesforce Sales Userオブジェクトを識別します。 </td> 
  </tr> 
 </tbody> 
</table>

Opportunity向けAPIドキュメント：[`https://developers.marketo.com/rest-api/lead-database/opportunities/`](https://developers.marketo.com/rest-api/lead-database/opportunities/)\
`API documentation for syncing Opportunities:  [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Opportunities/syncOpportunitiesUsingPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Opportunities/syncOpportunitiesUsingPOST)`

1. Salesforceの連絡先ロールをMarketoに同期します。

   Salesforce OpportunityのSalesforce Contact Rolesは、Marketo Opportunity Roleを介して同期できます。 Opportunity Roleレコードは、_externalOpportunityId_、_role_、_leadId_&#x200B;の各フィールドを指定します。

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>Marketo Opportunity Role Field</strong></td> 
   <td><strong>Salesforce連絡先役割フィールド</strong></td> 
   <td><strong>説明</strong></td> 
  </tr> 
  <tr> 
   <td>externalOpportunityId</td> 
   <td>Salesforce Opportunityでは、大文字と小文字が区別されないグローバル一意の識別子</td> 
   <td>外部のSalesforce Opportunityオブジェクトに対するMarketo Opportunity Roleを識別します。<br><br>Salesforce Opportunityを最初に正しく同期する必要があります。</td> 
  </tr> 
  <tr> 
   <td>leadId</td> 
   <td>該当なし(これはMarketoリードIDになります)</td> 
   <td>これは、Salesforceと同期された連絡先のMarketoリードIDです。<br><br>連絡先がMarketoで同期されたら、Marketo REST APIを使用して、Salesforce Contactの大文字と小文字を区別しないグローバル一意の識別子をexternalPersonIdとして使用し、Marketo Leadのクエリを実行できます。</td> 
  </tr> 
  <tr> 
   <td>役割</td> 
   <td>Salesforce連絡先の「役割」フィールド</td> 
   <td>この営業案件の連絡先の役割を説明します。</td> 
  </tr> 
 </tbody> 
</table>

Opportunity向けAPIドキュメント：[`https://developers.marketo.com/rest-api/lead-database/opportunities/`](https://developers.marketo.com/rest-api/lead-database/opportunities/)\
`API documentation for syncing Opportunities:  [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Opportunities/syncOpportunitiesUsingPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Opportunities/syncOpportunitiesUsingPOST)`

1. 最後の注目の瞬間/MSIスコアリングフィールドをSFDCに同期します。

   SalesforceオブジェクトがMarketoに正しく同期されたら、MSI機能を利用できます。 MSI Last Intersit Moment/Scoringフィールドは、リードのREST APIで公開されます。 これらのフィールドはMSIによって計算され、読み取り専用です。

   Marketoリードの最後の興味深いモーメント/スコアリングフィールドは、REST APIリードエンドポイントを使用して、Salesforceに定期的に同期する必要があります。 _externalPersonId_&#x200B;をfilterTypeとして使用し、Salesforce Lead GUIDをfilterValueとして渡して、Marketoリードに対してこのエンドポイントをクエリします。

   | GET/rest/v1/leads.json?filterType=externalPersonId&amp;filterValues=salesforceLeadId1,salesforceLeadId2 |
   |---|

   これらのフィールドの値を使用して、Salesforceのリード/連絡先オブジェクトと同期できます。

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>Marketoリードフィールド</strong></td> 
   <td><strong>Salesforceのリード/連絡先フィールド</strong></td> 
   <td><strong>説明</strong></td> 
  </tr> 
  <tr> 
   <td>msiLastIntersitiveMomentType</td> 
   <td>ラベル：最後の注目モーメントタイプ<br>名前：Last_Interestive_Moment_Type__c</td> 
   <td>リードの最後の興味深い瞬間のタイプ</td> 
  </tr> 
  <tr> 
   <td>msiLastIntertiveMomentDate</td> 
   <td><p>ラベル：最後の興味深い瞬間の日付</p><p>名前：Last_Interestive_Moment_Date__c</p></td> 
   <td>リードの最後の興味深い瞬間の日付</td> 
  </tr> 
  <tr> 
   <td>msiLastIntersitMomentDesc</td> 
   <td><p>ラベル：最後の興味深い瞬間の説明</p><p>名前：Last_Interest_Moment_Desc__c</p></td> 
   <td>リードの最後の興味深い瞬間の説明</td> 
  </tr> 
  <tr> 
   <td>msiLastIntersitiveMomentSource</td> 
   <td><p>ラベル：最後の興味深い瞬間の源</p><p>名前：Last_Interestive_Moment_Source__c</p></td> 
   <td>リードの最後の興味深い瞬間の源</td> 
  </tr> 
  <tr> 
   <td>優先度</td> 
   <td><p>ラベル：エンゲージメント</p><p>名前：優先度__c</p></td> 
   <td>リードの優先順位</td> 
  </tr> 
  <tr> 
   <td>relativeEkmensity</td> 
   <td><p>ラベル：相対的緊急度の値</p><p>名前：緊急度_値__c</p></td> 
   <td>リードの相対的緊急性</td> 
  </tr> 
  <tr> 
   <td>relativeScoring</td> 
   <td><p>ラベル：相対スコア値</p><p>名前：Relative_Score_Value__c</p></td> 
   <td>リードの相対スコア</td> 
  </tr> 
 </tbody> 
</table>

リードREST APIのドキュメント：[https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Leads/getLeadByIdUsingGET](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Leads/getLeadByIdUsingGET)

ネイティブでない同期を成功させるには、外部フィールドを適切に使用することが重要です。 一部のビューでデータを表示できなかった場合は、特定のフィールドが正しく同期されていなかった可能性があります。 例えば、リードのアクティビティと興味深い瞬間が、そのアカウントの下のMSIウィジェットを調べる際に表示されない場合、リードの会社またはアカウントが正しく同期されなかった可能性があります。 外部フィールドを指定してこのリードに対してGETリクエストを実行すると、リードが正しく同期されたかどうかを確認できます。 また、Marketoの外部の営業担当者の電子メールは、Salesforceのそのユーザーの電子メールと一致する必要があります。 電子メールが一致しない場合、Salesforceの「Marketo」タブにデータが表示されないことがあります。
