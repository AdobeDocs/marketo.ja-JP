---
description: 非ネイティブ MS Dynamics 統合用 Sales Insight - Marketoドキュメント — 製品ドキュメント
title: 非ネイティブ MS Dynamics 統合に関する Sales Insight
exl-id: 07613ff8-b197-4a3d-88e9-720b68a6b8da
source-git-commit: ff076d66a193664aa6ec05cf940143cebdd2d942
workflow-type: tm+mt
source-wordcount: '1439'
ht-degree: 42%

---

# 非ネイティブ MS Dynamics 統合に関する Sales Insight {#sales-insight-for-non-native-ms-dynamics-integrations}

Adobe Marketo Engageアカウントが、カスタマイズされた統合または非ネイティブの統合によって MS Dynamics に接続されている場合は、この記事を使用して Sales Insight を設定します。

>[!PREREQUISITES]
>
>* MSI の設定を開始する前に、Marketoインスタンスに対して「MSI 非ネイティブ」機能が有効になっています ( 有効でなく、既に購入済みの場合は、 [Marketoサポート](https://nation.marketo.com/t5/support/ct-p/Support){target=&quot;_blank&quot;} — この機能をまだ購入していない場合は、カスタマーサクセスマネージャーにお問い合わせください )。
>* ダウンロード [カスタム同期用の MSI パッケージ](https://mktg-cdn.marketo.com/community/MarketoSalesInsight_NonNative.zip){target=&quot;_blank&quot;}。
>* MSI 設定 ([オンプレミス](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/install-and-configure-marketo-sales-insight-in-microsoft-dynamics-365.md){target=&quot;_blank&quot;}, [Dynamics Online](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/install-and-configure-marketo-sales-insight-in-microsoft-dynamics-online.md){target=&quot;_blank&quot;}) です。
>* Marketo REST API [正常に設定されました](https://developers.marketo.com/rest-api/){target=&quot;_blank&quot;}。 公開されている CRUD API は、非ネイティブ同期を実行するための基盤となります。
>* 読み取り [このブログ投稿](https://developers.marketo.com/blog/create-and-associate-leads-companies-and-opportunities-with-the-marketo-rest-api/){target=&quot;_blank&quot;} を参照してください。


## MSI の非ネイティブ同期を成功させるには、以下が必要です {#successful-non-native-sync-for-msi-requires-the-following}

1. MS Dynamics セールスユーザーをMarketoに同期します。

   MS Dynamics セールスユーザーは、MS Dynamics でリード/連絡先を所有する外部ユーザーです。 MS Dynamics Sales User のMarketoセールス担当者をアップデートする必要があります。 セールス担当者のアップサートには、「externalSalesPersonId」フィールドが必須です。

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Marketo「セールス担当者」フィールド</strong></td> 
      <td><strong>MS Dynamics ユーザーフィールド</strong></td> 
      <td><strong>説明</strong></td> 
     </tr> 
     <tr> 
      <td>externalSalesPersonId</td> 
      <td>MS Dynamics ユーザーは大文字と小文字を区別せず、グローバルに一意の識別子を持ちます</td> 
      <td><p>外部の MS Dynamics User オブジェクトに対するMarketoセールス担当者レコードを識別します。</p><p>適切な関係が作成されるように、他のオブジェクトを同期する前に、まずセールス担当者を同期させる必要があります。</p></td> 
     </tr> 
    </tbody> 
   </table>

   * セールス担当者向け API ドキュメント：[https://developers.marketo.com/rest-api/lead-database/sales-persons/](https://developers.marketo.com/rest-api/lead-database/sales-persons/){target=&quot;_blank&quot;}
   * セールス担当者を同期するための API ドキュメント：[https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#! /Sales_Persons/syncSalesPersonsUsingPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#! /Sales_Persons/syncSalesPersonsUsingPOST){target=&quot;_blank&quot;}

1. MS Dynamics アカウントをMarketoに同期します。

   Marketoの会社は、MS Dynamics アカウント用にアップデートする必要があります。 企業のアップサートには、「_externalCompanyId_」および「_externalSalesPersonId_」フィールドが必須です。

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Marketo「企業」フィールド</strong></td> 
      <td><strong>MS Dynamics アカウントフィールド</strong></td> 
      <td><strong>説明</strong></td> 
     </tr> 
     <tr> 
      <td>externalCompanyId</td> 
      <td>MS Dynamics アカウントでは大文字と小文字が区別されず、グローバルに一意の ID</td> 
      <td>外部の MS Dynamics アカウントオブジェクトに対するMarketo会社レコードを識別します。</td> 
     </tr> 
     <tr> 
      <td>externalSalesPersonId</td> 
      <td>MS Dynamics Sales ユーザーは大文字と小文字を区別せず、グローバルに一意の識別子を持ちます</td> 
      <td>アカウント所有者である外部 MS Dynamics Sales User オブジェクトに対するMarketo企業レコードを識別します。<br><br>また、Marketo 内で企業レコードを所有するセールス担当者に企業を関連付けるためにも使用されます。このフィールドを設定する前に、まずセールス担当者を同期させる必要があります。</td> 
     </tr> 
    </tbody> 
   </table>

   * 企業向け API ドキュメント：[https://developers.marketo.com/rest-api/lead-database/companies/](https://developers.marketo.com/rest-api/lead-database/companies/){target=&quot;_blank&quot;}
   * 会社を同期するための API ドキュメント： [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Companies/syncCompaniesUsingPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Companies/syncCompaniesUsingPOST){target=&quot;_blank&quot;}

1. MS Dynamics リード/連絡先をMarketoに同期します。

   MS Dynamics リード/連絡先用にMarketoリードをアップサートする必要があります。 リードのアップサートには、「_externalPersonId_」、「_externalSalesPersonId_」および「_externalCompanyId_」フィールドが必須です。

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Marketo「リード」フィールド</strong></td> 
      <td><strong>MS Dynamics リード/連絡先フィールド</strong></td> 
      <td><strong>説明</strong></td> 
     </tr> 
     <tr> 
      <td>externalPersonId</td> 
      <td>MS Dynamics リード/連絡先で大文字と小文字を区別しないグローバル一意の識別子</td> 
      <td>外部の MS Dynamics リード/連絡先オブジェクトに対するMarketoリードレコードを識別します。<br><br>これは、MSI 非ネイティブ用に導入された新しいフィールドです。</td> 
     </tr> 
     <tr> 
      <td>externalSalesPersonId</td> 
      <td>MS Dynamics Sales ユーザーは大文字と小文字を区別せず、グローバルに一意の識別子を持ちます</td> 
      <td>このリード/連絡先を所有する外部 MS Dynamics セールスユーザーオブジェクトを識別します。<br><br>また、このリードを Marketo のセールス担当者と関連付けます。最初にセールス担当者を正しく同期させる必要があります。</td> 
     </tr> 
     <tr> 
      <td>externalCompanyId</td> 
      <td>MS Dynamics アカウントでは大文字と小文字が区別されず、グローバルに一意の ID</td> 
      <td>リード/連絡先が属する外部 MS Dynamics アカウントオブジェクトを識別します。<br><br>また、このリードレコードを Marketo の企業と関連付けます。最初に MS Dynamics アカウントを正しく同期する必要があります。</td> 
     </tr> 
    </tbody> 
   </table>

   * リード向け API ドキュメント： [https://developers.marketo.com/rest-api/lead-database/leads/](https://developers.marketo.com/rest-api/lead-database/leads/){target=&quot;_blank&quot;}
   * リードを同期するための API ドキュメント：[https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#! /Leads/syncLeadUsingPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Leads/syncLeadUsingPOST){target=&quot;_blank&quot;}

1. MS Dynamics 商談をMarketoに同期します。

   MS Dynamics 商談用にMarketo商談をアップサートする必要があります。 商談のアップサートには、「_externalOpportunityId_」、「_externalCompanyId_」および「_externalSalesPersonId_&#x200B;フィールドが必須です。

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Marketo「商談」オブジェクトフィールド</strong></td> 
      <td><strong>MS Dynamics 商談オブジェクトフィールド</strong></td> 
      <td><strong>説明</strong></td> 
     </tr> 
     <tr> 
      <td>externalOpportunityId</td> 
      <td>MS Dynamics リード/連絡先で大文字と小文字を区別しないグローバル一意の識別子</td> 
      <td>外部の MS Dynamics 商談オブジェクトに対するMarketo商談レコードを識別します。</td> 
     </tr> 
     <tr> 
      <td>externalCompanyId</td> 
      <td>MS Dynamics アカウントでは大文字と小文字が区別されず、グローバルに一意の ID</td> 
      <td>このオポチュニティが属する外部の MS Dynamics アカウントオブジェクトを識別します。 <br><br>最初に MS Dynamics アカウントを正しく同期する必要があります。</td> 
     </tr> 
     <tr> 
      <td>externalSalesPersonId</td> 
      <td>MS Dynamics Sales ユーザーは大文字と小文字を区別せず、グローバルに一意の識別子を持ちます</td> 
      <td>このオポチュニティを所有する外部 MS Dynamics Sales User オブジェクトを識別します。 </td> 
     </tr> 
    </tbody> 
   </table>

   * オポチュニティに関する API ドキュメント： [https://developers.marketo.com/rest-api/lead-database/opportunities/](https://developers.marketo.com/rest-api/lead-database/opportunities/){target=&quot;_blank&quot;}
   * オポチュニティを同期するための API ドキュメント： [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Opportunities/syncOpportunitiesUsingPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Opportunities/syncOpportunitiesUsingPOST){target=&quot;_blank&quot;}

1. MS Dynamics 連絡先ロールをMarketoに同期します。

   MS Dynamics Dynamics 商談の連絡先ロールは、Marketo商談ロールを介して同期できます。 商談ロールレコードには、「_externalOpportunityId_」、「_role_」および「_leadId_」フィールドが必須です。

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Marketo「商談ロール」フィールド</strong></td> 
      <td><strong>MS Dynamics 連絡先の役割フィールド</strong></td> 
      <td><strong>説明</strong></td> 
     </tr> 
     <tr> 
      <td>externalOpportunityId</td> 
      <td>MS Dynamics 商談の大文字と小文字を区別しないグローバル一意の識別子</td> 
      <td>外部の MS Dynamics 商談オブジェクトに対するMarketo商談の役割を識別します。<br><br>MS Dynamics 商談を最初に正しく同期する必要があります。</td> 
     </tr> 
     <tr> 
      <td>leadId</td> 
      <td>該当なし、これは Marketo のリード ID になります</td> 
      <td>これは、同期された MS Dynamics 連絡先のMarketoリード ID です。<br><br>連絡先がMarketoで同期されると、Marketo REST API を使用して、MS Dynamics 連絡先の大文字と小文字を区別しないグローバル一意の識別子を externalPersonId として使用し、Marketoリードに対するクエリを実行できます。</td> 
     </tr> 
     <tr> 
      <td>role</td> 
      <td>MS Dynamics 連絡先の役割フィールド</td> 
      <td>この商談の連絡先のロールを記述します。</td> 
     </tr> 
    </tbody> 
   </table>

   * オポチュニティに関する API ドキュメント： [https://developers.marketo.com/rest-api/lead-database/opportunities/](https://developers.marketo.com/rest-api/lead-database/opportunities/){target=&quot;_blank&quot;}
   * オポチュニティを同期するための API ドキュメント： [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Opportunities/syncOpportunitiesUsingPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Opportunities/syncOpportunitiesUsingPOST){target=&quot;_blank&quot;}

1. 最新の注目のアクション/MSI スコアリングフィールドを MS Dynamics に同期します。

   MS Dynamics オブジェクトをMarketoに正しく同期したら、MSI 機能を利用できます。 MSI の「最新の注目のアクション」／「スコア」フィールドは、リードの REST API で公開されます。これらのフィールドは、MSI によって計算され、読み取り専用です。

   Marketoリードの「最後の注目のアクション/スコアリング」フィールドは、REST API リードエンドポイントを使用して、MS Dynamics に定期的に同期する必要があります。 を使用してMarketoリードに対してこのエンドポイントをクエリします _externalPersonId_ を filterType として設定し、MS Dynamics リード GUID を filterValue として渡す。

   | GET/rest/v1/leads.json?filterType=externalPersonId&amp;filterValues=MS DynamicsLeadId1,MS DynamicsLeadId2 |
   |---|

   その後、これらのフィールドの値を使用して、MS Dynamics リード/連絡先オブジェクトに同期できます。

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Marketo「リード」フィールド</strong></td> 
      <td><strong>MS Dynamics リード/連絡先フィールド</strong></td> 
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

   * リード REST API 向けドキュメント：[https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#! /Leads/getLeadByIdUsingGET](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Leads/getLeadByIdUsingGET){target=&quot;_blank&quot;}。
   非ネイティブ同期を成功させるには、外部フィールドを適切に使用することが重要です。一部のビューにデータが表示されない場合は、特定のフィールドが正しく同期されていない可能性があります。例えば、アカウントの下にある MSI ウィジェットにリードのアクティビティや注目のアクションが表示されない場合、リードの企業かアカウントのどちらかが正しく同期されていない可能性があります。外部フィールドを指定してこのリードに対して GET リクエストを実行すると、リードが正しく同期されたかどうかを検証できます。さらに、Marketoの外部セールス担当者の E メールが、MS Dynamics のそのユーザーの E メールと一致している必要があります。 E メールが一致しない場合、MS Dynamics の「 Marketo 」タブにデータが表示されないことがあります。
