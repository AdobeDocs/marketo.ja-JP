---
description: 非ネイティブ MS[!DNL Sales Insight] 統合向け  [!DNL Dynamics]  キュメント - Marketo ドキュメント – 製品ドキュメント
title: '非ネイティブ MS[!DNL Sales Insight] 統合用の  [!DNL Dynamics] '
exl-id: 07613ff8-b197-4a3d-88e9-720b68a6b8da
feature: Marketo Sales Insights
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '1228'
ht-degree: 46%

---

# 非ネイティブ MS [!DNL Sales Insight] 統合用の [!DNL Dynamics] {#sales-insight-for-non-native-ms-dynamics-integrations}

カスタマイズした統合または非ネイティブ統合を使用してAdobe Marketo Engage アカウントが MS [!DNL Dynamics] に接続されている場合は、この記事を参照して [!DNL Sales Insight] を設定します。

>[!PREREQUISITES]
>
>* MSI のセットアップを開始する前に、Marketo インスタンスで「MSI 非ネイティブ」機能が有効になっていました。 そうでない場合は、[Marketo サポート ](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"} にお問い合わせください。 この機能をまだ購入していない場合は、アドビアカウントチーム（担当のアカウントマネージャー）にお問い合わせください。
>* [ カスタム同期用の MSI パッケージ ](https://mktg-cdn.marketo.com/community/MarketoSalesInsight_NonNative.zip){target="_blank"} をダウンロードします。
>* MSI セットアップを備えた MS Dynamics サブスクリプション（現時点では [Dynamics Online](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/install-and-configure-marketo-sales-insight-in-microsoft-dynamics-online.md){target="_blank"} のみをサポートしています）。
>* Marketo REST API が[正常に設定](https://experienceleague.adobe.com/ja/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}されている。公開されている CRUD API は、非ネイティブ同期を実行するための基盤となります。
>* オブジェクトと関係を理解するには、[このブログ記事](https://developers.marketo.com/blog/create-and-associate-leads-companies-and-opportunities-with-the-marketo-rest-api/){target="_blank"}を参照してください。

## MSI の非ネイティブ同期を成功させるには、以下が必要です {#successful-non-native-sync-for-msi-requires-the-following}

1. MS [!DNL Dynamics] Sales User をMarketoに同期します。

   MS [!DNL Dynamics] Sales User は、MS [!DNL Dynamics] のリード/取引先責任者を所有する外部ユーザーです。 MS [!DNL Dynamics] Sales User のMarketo担当者をアップサートする必要があります。 セールス担当者のアップサートには、「externalSalesPersonId」フィールドが必須です。

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Marketo「セールス担当者」フィールド</strong></td> 
        <td><strong>MS <span class="dnl">Dynamics</span> ユーザーフィールド</strong></td> 
      <td><strong>説明</strong></td> 
     </tr> 
     <tr> 
      <td>externalSalesPersonId</td> 
        <td>MS <span class="dnl">Dynamics</span> ユーザーの大文字と小文字を区別しないグローバル一意識別子</td> 
      <td><p>外部 MS <span class="dnl">Dynamics</span> ユーザーオブジェクトに対するMarketo販売担当者レコードを識別します。</p><p>適切な関係が作成されるように、他のオブジェクトを同期する前に、まずセールス担当者を同期させる必要があります。</p></td> 
     </tr> 
    </tbody> 
   </table>

   * [ 販売担当者向け API ドキュメント ](https://experienceleague.adobe.com/ja/docs/marketo-developer/marketo/rest/lead-database/sales-persons){target="_blank"}
   * [ 販売担当者の同期に関する API ドキュメント ](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Sales-Persons/operation/syncSalesPersonsUsingPOST){target="_blank"}

1. MS [!DNL Dynamics] アカウントをMarketoに同期します。

   Marketo会社は、MS [!DNL Dynamics] アカウントをアップサートする必要があります。 企業のアップサートには、「_externalCompanyId_」および「_externalSalesPersonId_」フィールドが必須です。

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Marketo「企業」フィールド</strong></td> 
        <td><strong>MS <span class="dnl">Dynamics</span> アカウントフィールド</strong></td> 
      <td><strong>説明</strong></td> 
     </tr> 
     <tr> 
      <td>externalCompanyId</td> 
        <td>MS <span class="dnl">Dynamics</span> アカウントの大文字と小文字を区別しないグローバル一意識別子</td> 
        <td>Marketoの会社レコードを外部の MS <span class="dnl">Dynamics</span> アカウントオブジェクトに対して識別します。</td> 
     </tr> 
     <tr> 
      <td>externalSalesPersonId</td> 
        <td>MS <span class="dnl">Dynamics</span> セールス ユーザー：大文字と小文字を区別しないグローバル一意識別子</td> 
        <td>アカウント所有者である外部 MS <span class="dnl">Dynamics</span> 営業ユーザーオブジェクトに対してMarketo会社レコードを識別します。<br><br>また、Marketo 内で企業レコードを所有するセールス担当者に企業を関連付けるためにも使用されます。このフィールドを設定する前に、まずセールス担当者を同期させる必要があります。</td> 
     </tr> 
    </tbody> 
   </table>

   * 企業向け API ドキュメント：[https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/companies](https://experienceleague.adobe.com/ja/docs/marketo-developer/marketo/rest/lead-database/companies){target="_blank"}
   * 会社の同期に関する API ドキュメント：[https://developer.adobe.com/marketo-apis/api/mapi/#tag/Sales-Persons/operation/syncSalesPersonsUsingPOST](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Sales-Persons/operation/syncSalesPersonsUsingPOST){target="_blank"}

1. MS [!DNL Dynamics] のリード/連絡先をMarketoに同期します。

   MS [!DNL Dynamics] リード/連絡先のMarketo リードをアップサートする必要があります。 リードのアップサートには、「_externalPersonId_」、「_externalSalesPersonId_」および「_externalCompanyId_」フィールドが必須です。

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Marketo「リード」フィールド</strong></td> 
        <td><strong>MS <span class="dnl">Dynamics</span> リード/連絡先フィールド</strong></td> 
      <td><strong>説明</strong></td> 
     </tr> 
     <tr> 
      <td>externalPersonId</td> 
        <td>MS <span class="dnl">Dynamics</span> リード/連絡先で大文字と小文字が区別されないグローバル一意識別子</td> 
        <td>Marketo リードレコードを外部の MS <span class="dnl">Dynamics</span> リード/連絡先オブジェクトに対して識別します。<br><br>これは、MSI 非ネイティブ用に導入された新しいフィールドです。</td> 
     </tr> 
     <tr> 
      <td>externalSalesPersonId</td> 
        <td>MS <span class="dnl">Dynamics</span> セールス ユーザー：大文字と小文字を区別しないグローバル一意識別子</td> 
        <td>このリード/連絡先を所有する外部 MS <span class="dnl">Dynamics</span> 営業ユーザーオブジェクトを識別します。<br><br>また、このリードを Marketo のセールス担当者と関連付けます。最初にセールス担当者を正しく同期させる必要があります。</td> 
     </tr> 
     <tr> 
      <td>externalCompanyId</td> 
        <td>MS <span class="dnl">Dynamics</span> アカウントの大文字と小文字を区別しないグローバル一意識別子</td> 
        <td>リード/連絡先が属する外部 MS <span class="dnl">Dynamics</span> アカウントオブジェクトを識別します。<br><br>また、このリードレコードを Marketo の企業と関連付けます。最初に MS <span class="dnl">Dynamics</span> アカウントを正しく同期する必要があります。</td> 
     </tr> 
    </tbody> 
   </table>

   * リード向け API ドキュメント：[https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/lead-database](https://experienceleague.adobe.com/ja/docs/marketo-developer/marketo/rest/lead-database/lead-database){target="_blank"}
   * リードの同期に関する API ドキュメント：[https://developer.adobe.com/marketo-apis/api/mapi/#tag/Leads/operation/syncLeadUsingPOST](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Leads/operation/syncLeadUsingPOST){target="_blank"}

1. MS [!DNL Dynamics] オポチュニティをMarketoに同期します。

   MS [!DNL Dynamics] オポチュニティのMarketo オポチュニティをアップサートする必要があります。 商談のアップサートには、「_externalOpportunityId_」、「_externalCompanyId_」および「_externalSalesPersonId_」フィールドが必須です。

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Marketo「商談」オブジェクトフィールド</strong></td> 
        <td><strong>MS <span class="dnl">Dynamics</span> 商談オブジェクトフィールド</strong></td> 
      <td><strong>説明</strong></td> 
     </tr> 
     <tr> 
      <td>externalOpportunityId</td> 
        <td>MS <span class="dnl">Dynamics</span> リード/連絡先で大文字と小文字が区別されないグローバル一意識別子</td> 
      <td>Marketo商談レコードを外部の MS <span class="dnl">Dynamics</span> 商談オブジェクトに対して識別します。</td> 
     </tr> 
     <tr> 
      <td>externalCompanyId</td> 
        <td>MS <span class="dnl">Dynamics</span> アカウントの大文字と小文字を区別しないグローバル一意識別子</td> 
        <td>このオポチュニティが属する外部 MS <span class="dnl">Dynamics</span> アカウントオブジェクトを識別します。 <br><br> 最初に MS <span class="dnl">Dynamics</span> アカウントを正しく同期する必要があります。</td> 
     </tr> 
     <tr> 
      <td>externalSalesPersonId</td> 
        <td>MS <span class="dnl">Dynamics</span> セールス ユーザー：大文字と小文字を区別しないグローバル一意識別子</td> 
        <td>このオポチュニティを所有する外部 MS <span class="dnl">Dynamics</span> 営業ユーザーオブジェクトを識別します。 </td> 
     </tr> 
    </tbody> 
   </table>

   * オポチュニティに関する API ドキュメント：[https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/opportunities](https://experienceleague.adobe.com/ja/docs/marketo-developer/marketo/rest/lead-database/opportunities){target="_blank"}
   * オポチュニティを同期するための API ドキュメント：[https://developer.adobe.com/marketo-apis/api/mapi/#tag/Opportunities/operation/syncOpportunitiesUsingPOST](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Opportunities/operation/syncOpportunitiesUsingPOST){target="_blank"}

1. MS [!DNL Dynamics] 連絡先ロールをMarketoに同期します。

   MS [!DNL Dynamics] 商談の MS [!DNL Dynamics] 連絡先ロールは、Marketo商談ロールを介して同期できます。 商談ロールレコードには、「_externalOpportunityId_」、「_role_」および「_leadId_」フィールドが必須です。

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Marketo「商談ロール」フィールド</strong></td> 
        <td><strong>MS <span class="dnl">Dynamics</span> 連絡先ロールフィールド</strong></td> 
      <td><strong>説明</strong></td> 
     </tr> 
     <tr> 
      <td>externalOpportunityId</td> 
        <td>MS <span class="dnl">Dynamics</span> 商談で大文字と小文字が区別されないグローバル一意識別子</td> 
      <td>Marketo商談ロールを外部 MS <span class="dnl">Dynamics</span> 商談オブジェクトに対して識別します。<br><br> 最初に MS <span class="dnl">Dynamics</span> 商談を正しく同期する必要があります。</td> 
     </tr> 
     <tr> 
      <td>leadId</td> 
      <td>該当なし、これは Marketo のリード ID になります</td> 
        <td>これは、同期された MS <span class="dnl">Dynamics</span> 連絡先のMarketo リード ID になります。<br><br> 連絡先がMarketoで同期されると、MS <span class="dnl">Dynamics</span> を使用できるようになります。連絡先で大文字と小文字を区別しないグローバルな一意の ID を、externalPersonId として使用し、Marketo REST API を使用してMarketo リードをクエリします。</td> 
     </tr> 
     <tr> 
      <td>ロール</td> 
        <td>MS <span class="dnl">Dynamics</span> 連絡先の役割フィールド</td> 
      <td>この商談の取引先責任者のロールを記述します。</td> 
     </tr> 
    </tbody> 
   </table>

   * オポチュニティに関する API ドキュメント：[https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/opportunities](https://experienceleague.adobe.com/ja/docs/marketo-developer/marketo/rest/lead-database/opportunities){target="_blank"}
   * オポチュニティを同期するための API ドキュメント：[https://developer.adobe.com/marketo-apis/api/mapi/#tag/Opportunities/operation/syncOpportunitiesUsingPOST](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Opportunities/operation/syncOpportunitiesUsingPOST){target="_blank"}

1. 最後の興味深い瞬間/MSI スコアリングフィールドを MS [!DNL Dynamics] に同期

   MS [!DNL Dynamics] オブジェクトがMarketoに正しく同期されると、MSI 機能を利用できるようになります。 MSI の「最新の注目のアクション」／「スコア」フィールドは、リードの REST API で公開されます。これらのフィールドは、MSI によって計算され、読み取り専用です。

   Marketo リードの最後の興味深い瞬間/スコアリングフィールドは、REST API リードエンドポイントを使用して、MS [!DNL Dynamics] に定期的に同期する必要があります。 _externalPersonId_ を filterType として使用し、MS [!DNL Dynamics] リード GUID を filterValue として渡すことで、Marketo リードのこのエンドポイントをクエリします。

   | GET /rest/v1/leads.json?filterType=externalPersonId&amp;filterValues=MS DynamicsLeadId1,MS DynamicsLeadId2 |
   |---|

   その後、これらのフィールドの値を使用して、MS [!DNL Dynamics] リード/連絡先オブジェクトに同期できます。

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Marketo「リード」フィールド</strong></td> 
        <td><strong>MS <span class="dnl">Dynamics</span> リード/連絡先フィールド</strong></td> 
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

   * リード REST API のドキュメント：[https://developer.adobe.com/marketo-apis/api/mapi/#tag/Leads/operation/getLeadByIdUsingGET](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Leads/operation/getLeadByIdUsingGET){target="_blank"}。

   非ネイティブ同期を成功させるには、外部フィールドを適切に使用することが重要です。一部のビューにデータが表示されない場合は、特定のフィールドが正しく同期されていない可能性があります。例えば、リードのアカウントの下にある MSI ウィジェットを参照したときにリードのアクティビティや関心を引くモーメントが表示されない場合は、リードの会社またはアカウントが正しく同期されていない可能性があります。外部フィールドを指定してこのリードに対して GET リクエストを実行すると、リードが正しく同期されたかどうかを検証できます。また、Marketo の外部セールス担当者のメールは、MS Dynamics のそのユーザのメールと一致する必要があります。メールが一致しない場合、MS Dynamics の「Marketo」タブにデータが表示されないことがあります。
