---
unique-page-id: 45417125
description: ネイティブ以外のSalesforce統合向けのSales Insight - Marketto Docs — 製品ドキュメント
title: ネイティブ以外のSalesforce統合に関するSales Insight
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '1269'
ht-degree: 0%

---


# ネイティブ以外のSalesforce統合向けのSales Insight {#sales-insight-for-non-native-salesforce-integrations}

Marketoアカウントが、カスタマイズされた統合または非ネイティブの統合を通じてSalesforceに接続している場合は、このドキュメントを使用してSales Insightを設定します。

>[!PREREQUISITES]
>
>* Marketing Suiteのインスタンスに対して「MSI非ネイティブ」機能を有効にするには、Customer Success Managerにお問い合わせください。
>* MSIパッケージが設定されたSalesforceアカウント。
>* Marketo REST API [は](https://developers.marketo.com/rest-api/)を正常にセットアップしました。 公開されたCRUD APIは、非ネイティブ同期の実行の基盤となります。
>* オブジェクトと関係を理解するために、[このブログの記事](https://developers.marketo.com/blog/create-and-associate-leads-companies-and-opportunities-with-the-marketo-rest-api/)を読んでください。
>* Salesforceオブジェクトを設定し、大文字と小文字を区別する15文字のグローバル一意識別子ではなく、大文字と小文字を区別しない18文字のグローバル一意識別子を表示します。

>



>[!NOTE]
>
>Marketo MSI管理パネルのREST API設定は、非ネイティブ同期には使用できません。

## MSIの非ネイティブ同期に成功するには、次の{#successful-non-native-sync-for-msi-requires-the-following}が必要です

1. Salesforce SalesユーザーをMarketoに同期します。

   Salesforce Sales Userは、Salesforceのリード/連絡先を所有する外部ユーザーです。 Salesforce Salesユーザーに対して、マーケティング担当者をアップセートする必要があります。 *externalSalesPersonId*&#x200B;フィールドは、販売担当者のアップサートに対して必須です。

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>「マーケティング担当者」フィールド</strong></td> 
   <td><strong>Salesforce Salesユーザーフィールド</strong></td> 
   <td><strong>説明</strong></td> 
  </tr> 
  <tr> 
   <td>externalSalesPersonId</td> 
   <td>Salesforce Salesユーザーは、大文字と小文字を区別しないグローバル一意識別子</td> 
   <td><p>外部のSalesforce Salesユーザーオブジェクトに対するMarketo Sales Personレコードを識別します。</p><p>他のオブジェクトを同期する前に、営業担当者に最初に同期を求め、適切な関係を作成する必要があります。</p></td> 
  </tr> 
 </tbody> 
</table>

販売担当者向けAPIドキュメント：[https://developers.marketo.com/rest-api/lead-database/sales-persons/](https://developers.marketo.com/rest-api/lead-database/sales-persons/)\
販売担当者を同期するためのAPIドキュメント：[https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Sales_Persons/syncSalesPersonsUsingPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Sales_Persons/syncSalesPersonsUsingPOST)

1. SalesforceアカウントをMarketoに同期します。

   Salesforceアカウントでは、マーケティング担当会社をアップセートする必要があります。 *externalCompanyId*&#x200B;と&#x200B;*externalSalesPersonId*&#x200B;の各フィールドは、会社のアップサート用に必須です。

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>マーケティング会社フィールド</strong></td> 
   <td><strong>Salesforceアカウントフィールド</strong></td> 
   <td><strong>説明</strong></td> 
  </tr> 
  <tr> 
   <td>externalCompanyId</td> 
   <td>Salesforceアカウントでは、大文字と小文字が区別されないグローバル一意識別子</td> 
   <td>外部のSalesforceアカウントオブジェクトに対するMarketo会社レコードを識別します。</td> 
  </tr> 
  <tr> 
   <td>externalSalesPersonId</td> 
   <td>Salesforce Salesユーザーは、大文字と小文字を区別しないグローバル一意識別子</td> 
   <td>アカウント所有者である外部Salesforce Salesユーザーオブジェクトに対するMarketo会社レコードを識別します。<br><br>また、マーケティングで、会社レコードを所有する営業担当者に会社を関連付けるためにも使用されます。このフィールドを設定する前に、営業担当者を最初に同期する必要があります。</td> 
  </tr> 
 </tbody> 
</table>

会社向けAPIドキュメント：[https://developers.marketo.com/rest-api/lead-database/companies/](https://developers.marketo.com/rest-api/lead-database/companies/)\
`API documentation for syncing Companies:  [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Companies/syncCompaniesUsingPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Companies/syncCompaniesUsingPOST)`

1. Salesforceのリード/連絡先をMarketorに同期します。

   Salesforceのリード/コンタクト用に、マーケティング担当者のリードを挿入する必要があります。 *externalPersonId*、*externalSalesPersonId*、*externalCompanyId*&#x200B;の各フィールドは、リードのアップサートに対して必須です。

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>マーケティング先リードフィールド</strong></td> 
   <td><strong>Salesforceのリード/連絡先フィールド</strong></td> 
   <td><strong>説明</strong></td> 
  </tr> 
  <tr> 
   <td>externalPersonId</td> 
   <td>Salesforceリード/連絡先で、大文字と小文字を区別しないグローバル一意識別子</td> 
   <td>外部のSalesforceのリード/コンタクトオブジェクトに対するMarketorのリードレコードを識別します。<br><br>これは、MSI Non-Nativeに導入された新しいフィールドです。</td> 
  </tr> 
  <tr> 
   <td>externalSalesPersonId</td> 
   <td>Salesforce Salesユーザーは、大文字と小文字を区別しないグローバル一意識別子</td> 
   <td>このリード/連絡先を所有する外部Salesforce Salesユーザーオブジェクトを識別します。<br><br>リードをMarketorの販売担当者と関連付ける。最初に営業担当者を正しく同期する必要があります。</td> 
  </tr> 
  <tr> 
   <td>externalCompanyId</td> 
   <td>Salesforceアカウントでは、大文字と小文字が区別されないグローバル一意識別子</td> 
   <td>リード/連絡先が属する外部Salesforceアカウントオブジェクトを識別します。<br><br>また、リードレコードをマーケティングトの会社に関連付けます。最初にSalesforceアカウントを正しく同期する必要があります。</td> 
  </tr> 
 </tbody> 
</table>

リードのAPIドキュメント：[`https://developers.marketo.com/rest-api/lead-database/leads/`](https://developers.marketo.com/rest-api/lead-database/leads/)\
リードを同期するためのAPIドキュメント： [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Leads/syncLeadUsingPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Leads/syncLeadUsingPOST)

1. SalesforceオポチュニティをMarketoに同期。

   Salesforceオポチュニティに対して、Marketor Opportunityを挿入する必要があります。 Opportunityのアップサートに対して、*externalOpportunityId*、*externalCompanyId*、*externalSalesPersonId*&#x200B;の各フィールドが必須です。

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>MarketorOpportunity Objectフィールド</strong></td> 
   <td><strong>Salesforceオポチュニティオブジェクトフィールド</strong></td> 
   <td><strong>説明</strong></td> 
  </tr> 
  <tr> 
   <td>externalOpportunityId</td> 
   <td>Salesforceリード/連絡先で、大文字と小文字を区別しないグローバル一意識別子</td> 
   <td>外部のSalesforceオポチュニティオブジェクトに対するMarketo Opportunityレコードを識別します。</td> 
  </tr> 
  <tr> 
   <td>externalCompanyId</td> 
   <td>Salesforceアカウントでは、大文字と小文字が区別されないグローバル一意識別子</td> 
   <td>このオポチュニティが属する外部Salesforceアカウントオブジェクトを識別します。 <br><br>最初にSalesforceアカウントを正しく同期する必要があります。</td> 
  </tr> 
  <tr> 
   <td>externalSalesPersonId</td> 
   <td>Salesforce Salesユーザーは、大文字と小文字を区別しないグローバル一意識別子</td> 
   <td>このオポチュニティを所有する外部Salesforce Salesユーザー・オブジェクトを識別します。 </td> 
  </tr> 
 </tbody> 
</table>

OpportunityのAPIドキュメント：[`https://developers.marketo.com/rest-api/lead-database/opportunities/`](https://developers.marketo.com/rest-api/lead-database/opportunities/)\
`API documentation for syncing Opportunities:  [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Opportunities/syncOpportunitiesUsingPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Opportunities/syncOpportunitiesUsingPOST)`

1. Salesforceの連絡先ロールをMarketoに同期します。

   Salesforce OpportunityのSalesforce Contactの役割は、Marketo Opportunityの役割を介して同期できます。 オポチュニティロールレコードは、*externalOpportunityId*、*role*、*leadId*&#x200B;の各フィールドを指定します。

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>「MarkettoOpportunity Role」フィールド</strong></td> 
   <td><strong>Salesforce連絡先役割フィールド</strong></td> 
   <td><strong>説明</strong></td> 
  </tr> 
  <tr> 
   <td>externalOpportunityId</td> 
   <td>Salesforceオポチュニティで大文字と小文字を区別しない、グローバル一意識別子</td> 
   <td>外部のSalesforceオポチュニティオブジェクトに対するMarketo Opportunityの役割を識別します。<br><br>Salesforce Opportunityを最初に正しく同期する必要があります。</td> 
  </tr> 
  <tr> 
   <td>leadId</td> 
   <td>該当なし。これはマーケティング担当者のリードIDになります。</td> 
   <td>これは、同期されたSalesforce ContactのMarketo Lead IDになります。<br><br>連絡先がMarketorで同期されたら、Marketor REST APIを使用して、Salesforce Contactのグローバルな一意の識別子であるexternalPersonIdおよびクエリを、大文字と小文字を区別しないで使用できます。</td> 
  </tr> 
  <tr> 
   <td>role</td> 
   <td>Salesforce連絡先の役割フィールド</td> 
   <td>このオポチュニティの連絡先の役割を説明します。</td> 
  </tr> 
 </tbody> 
</table>

OpportunityのAPIドキュメント：[`https://developers.marketo.com/rest-api/lead-database/opportunities/`](https://developers.marketo.com/rest-api/lead-database/opportunities/)\
`API documentation for syncing Opportunities:  [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Opportunities/syncOpportunitiesUsingPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Opportunities/syncOpportunitiesUsingPOST)`

1. 最後の注目のモーメント/MSIスコアリングフィールドをSFDCに同期します。

   SalesforceオブジェクトがMarketorに正しく同期されると、MSI機能を利用できます。 MSI最後の注目のモーメント/スコアリングフィールドは、リードのREST APIに公開されます。 これらのフィールドはMSIによって計算され、読み取り専用です。

   Marketorのリードの最後の興味深いモーメント/スコアリングフィールドは、REST APIリードエンドポイントを使用して、Salesforceと定期的に同期する必要があります。 *externalPersonId*&#x200B;をfilterTypeとして使用し、Salesforce Lead GUIDをfilterValueとして渡して、Marketor Leadのこのエンドポイントをクエリします。

   | GET/rest/v1/leads.json?filterType=externalPersonId&amp;filterValues=salesforceLeadId1,salesforceLeadId2 |
   |---|

   その後、これらのフィールドの値を使用して、Salesforceのリード/コンタクトオブジェクトと同期できます。

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>マーケティング先リードフィールド</strong></td> 
   <td><strong>Salesforceのリード/連絡先フィールド</strong></td> 
   <td><strong>説明</strong></td> 
  </tr> 
  <tr> 
   <td>msiLastIntersitiveMomentType</td> 
   <td>ラベル：最後の注目のモーメントのタイプ<br>名前：Last_Intersitive_Moment_Type__c</td> 
   <td>リードの最後の興味深いモーメントのタイプ</td> 
  </tr> 
  <tr> 
   <td>msiLastIntersitiveMomentDate</td> 
   <td><p>ラベル：最後の興味深い瞬間の日付</p><p>名前：Last_Intersion_Moment_Date__c</p></td> 
   <td>リードの最後に興味を引いた瞬間の日付</td> 
  </tr> 
  <tr> 
   <td>msiLastIntersitiveMomentDesc</td> 
   <td><p>ラベル：最後の興味深いモーメントの説明</p><p>名前：Last_Intersion_Moment_Desc__c</p></td> 
   <td>リードの最後の興味深い瞬間の説明</td> 
  </tr> 
  <tr> 
   <td>msiLastIntersitiveMomentSource</td> 
   <td><p>ラベル：最後の興味深い瞬間の源</p><p>名前：Last_Intersitive_Moment_Source__c</p></td> 
   <td>リードの最後の興味深い瞬間の源</td> 
  </tr> 
  <tr> 
   <td>priority</td> 
   <td><p>ラベル：関与</p><p>名前：Priority__c</p></td> 
   <td>リードの優先順位</td> 
  </tr> 
  <tr> 
   <td>relativeEkmensity</td> 
   <td><p>ラベル：相対緊急度の値</p><p>名前：緊急度_値_c</p></td> 
   <td>リードの相対的緊急性</td> 
  </tr> 
  <tr> 
   <td>relativeScoring</td> 
   <td><p>ラベル：相対スコアリング値</p><p>名前：Relative_Score_Value__c</p></td> 
   <td>リードの相対スコア</td> 
  </tr> 
 </tbody> 
</table>

リードREST APIに関するドキュメント： [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Leads/getLeadByIdUsingGET](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Leads/getLeadByIdUsingGET)。

外部フィールドを適切に使用することは、非ネイティブ同期を正常に行うための鍵となります。 一部の表示でデータを表示できない場合は、特定のフィールドが正しく同期されていなかった可能性があります。 例えば、リードのアクティビティと興味深い瞬間が、自分のアカウントの下のMSIウィジェットを閲覧すると表示されない場合、リードの会社またはアカウントが正しく同期されなかった可能性があります。 外部フィールドの指定中にこのリードに対してGETリクエストを実行すると、リードが正しく同期されたかどうかを確認できます。 また、Marketoの外部販売担当者向けの電子メールは、Salesforceのそのユーザー向けの電子メールと一致する必要があります。 電子メールが一致しない場合、Salesforceの「Marketo」タブにデータが表示されないことがあります。

