---
description: 非ネイティブ MS  [!DNL Dynamics]  統合用 [!DNL Sales Insight] - Marketo ドキュメント - 製品ドキュメント
title: 非ネイティブ MS  [!DNL Dynamics]  統合用 [!DNL Sales Insight]
exl-id: 07613ff8-b197-4a3d-88e9-720b68a6b8da
feature: Marketo Sales Insights
source-git-commit: 7a57e52b497b271beff95b203bddd0c911e2e6a3
workflow-type: tm+mt
source-wordcount: '1262'
ht-degree: 97%

---

# 非ネイティブ MS [!DNL Dynamics] 統合用 [!DNL Sales Insight] {#sales-insight-for-non-native-ms-dynamics-integrations}

Adobe Marketo Engage アカウントが、カスタマイズされた統合または非ネイティブ統合によって MS [!DNL Dynamics] に接続されている場合は、このドキュメントを使用して [!DNL Sales Insight] を設定してください。

>[!PREREQUISITES]
>
>* MSI の設定を開始する前に、Marketo インスタンスに対して「MSI 非ネイティブ」機能を有効にします。そうでなく、既に機能を購入している場合は、[Marketo サポート](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}にお問い合わせください。この機能をまだ購入していない場合は、アドビのアカウントチーム（担当のアカウントマネージャー）にお問い合わせください。
>* [カスタム同期用 MSI パッケージ](https://mktg-cdn.marketo.com/community/MarketoSalesInsight_NonNative.zip){target="_blank"}をダウンロードします。
>* MSI セットアップを備えた MS Dynamics サブスクリプション（現時点では [Dynamics Online](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/install-and-configure-marketo-sales-insight-in-microsoft-dynamics-online.md){target="_blank"} のみをサポートしています）。
>* Marketo REST API が[正常に設定](https://experienceleague.adobe.com/ja/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}されている。公開されている CRUD API は、非ネイティブ同期を実行するための基盤となります。
>* オブジェクトと関係を理解するには、[このブログ記事](https://developers.marketo.com/blog/create-and-associate-leads-companies-and-opportunities-with-the-marketo-rest-api/){target="_blank"}を参照してください。

## MSI の非ネイティブ同期を成功させるには、次が必要です。 {#successful-non-native-sync-for-msi-requires-the-following}

1. MS [!DNL Dynamics] セールスユーザを Marketo に同期します。

   MS [!DNL Dynamics] セールスユーザは、 MS [!DNL Dynamics] のリード／取引先責任者を所有する外部ユーザです。この MS [!DNL Dynamics] セールスユーザ用に Marketo セールス担当者をアップサートする必要があります。セールス担当者のアップサートには、「externalSalesPersonId」フィールドが必須です。

   <table>
    <colgroup>
     <col>
     <col>
     <col>
    </colgroup>
    <tbody>
     <tr>
      <td><strong>Marketo「セールス担当者」フィールド</strong></td>
        <td><strong>MS <span class="dnl">Dynamics</span> ユーザフィールド</strong></td>
      <td><strong>説明</strong></td>
     </tr>
     <tr>
      <td>externalSalesPersonId</td>
        <td>MS <span class="dnl">Dynamics</span> ユーザの大文字小文字を区別しないグローバルな一意の ID</td>
      <td><p>外部 MS <span class="dnl">Dynamics</span> ユーザオブジェクトに対する Marketo セールス担当者レコードを特定します。</p><p>適切な関係が作成されるように、他のオブジェクトを同期する前に、まずセールス担当者を同期させる必要があります。</p></td>
     </tr>
    </tbody>
   </table>

   * [セールス担当者向け API ドキュメント](https://experienceleague.adobe.com/ja/docs/marketo-developer/marketo/rest/lead-database/sales-persons){target="_blank"}
   * [セールス担当者を同期する API ドキュメント](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Sales-Persons/operation/syncSalesPersonsUsingPOST){target="_blank"}

1. MS [!DNL Dynamics] アカウントを Marketo に同期します。

   この MS [!DNL Dynamics] アカウント用に Marketo の企業をアップサートする必要があります。企業のアップサートには、「_externalCompanyId_」および「_externalSalesPersonId_」フィールドが必須です。

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
        <td>MS <span class="dnl">Dynamics</span> アカウントの大文字小文字を区別しないグローバルな一意の ID</td>
        <td>外部 MS <span class="dnl">Dynamics</span> アカウントオブジェクトに対する Marketo 企業レコードを特定します。</td>
     </tr>
     <tr>
      <td>externalSalesPersonId</td>
        <td>MS <span class="dnl">Dynamics</span> セールスユーザの大文字小文字を区別しないグローバルな一意の ID</td>
        <td>アカウント所有者である外部 MS <span class="dnl">Dynamics</span> セールスユーザオブジェクトに対する Marketo 企業レコードを特定します。<br><br>また、Marketo 内で企業レコードを所有するセールス担当者に企業を関連付けるためにも使用されます。このフィールドを設定する前に、まずセールス担当者を同期させる必要があります。</td>
     </tr>
    </tbody>
   </table>

   * 企業向け API ドキュメント：[https://experienceleague.adobe.com/ja/docs/marketo-developer/marketo/rest/lead-database/companies](https://experienceleague.adobe.com/ja/docs/marketo-developer/marketo/rest/lead-database/companies){target="_blank"}
   * 企業を同期する API ドキュメント：[https://developer.adobe.com/marketo-apis/api/mapi/#tag/Sales-Persons/operation/syncSalesPersonsUsingPOST](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Sales-Persons/operation/syncSalesPersonsUsingPOST){target="_blank"}

1. MS [!DNL Dynamics] のリード／取引先責任者を Marketo に同期します。

   この MS [!DNL Dynamics] のリード／取引先責任者用に Marketo のリードをアップサートする必要があります。リードのアップサートには、「_externalPersonId_」、「_externalSalesPersonId_」および「_externalCompanyId_」フィールドが必須です。

   <table>
    <colgroup>
     <col>
     <col>
     <col>
    </colgroup>
    <tbody>
     <tr>
      <td><strong>Marketo「リード」フィールド</strong></td>
        <td><strong>MS <span class="dnl">Dynamics</span>「リード／取引先責任者」フィールド</strong></td>
      <td><strong>説明</strong></td>
     </tr>
     <tr>
      <td>externalPersonId</td>
        <td>MS <span class="dnl">Dynamics</span> のリード／取引先責任者の大文字小文字を区別しないグローバルな一意の ID</td>
        <td>外部 MS <span class="dnl">Dynamics</span> リード／取引先責任者オブジェクトに対する Marketo リードレコードを特定します。<br><br>これは、MSI 非ネイティブ用に導入された新しいフィールドです。</td>
     </tr>
     <tr>
      <td>externalSalesPersonId</td>
        <td>MS <span class="dnl">Dynamics</span> セールスユーザの大文字小文字を区別しないグローバルな一意の ID</td>
        <td>このリード／取引先責任者を所有する外部 MS <span class="dnl">Dynamics</span> セールスユーザオブジェクトを特定します。<br><br>また、このリードを Marketo のセールス担当者と関連付けます。最初にセールス担当者を正しく同期させる必要があります。</td>
     </tr>
     <tr>
      <td>externalCompanyId</td>
        <td>MS <span class="dnl">Dynamics</span> アカウントの大文字小文字を区別しないグローバルな一意の ID</td>
        <td>リード／取引先責任者が属する外部 MS <span class="dnl">Dynamics</span> アカウントオブジェクトを特定します。<br><br>また、このリードレコードを Marketo の企業と関連付けます。最初に MS <span class="dnl">Dynamics</span> アカウントを正しく同期させる必要があります。</td>
     </tr>
    </tbody>
   </table>

   * リードに関する API ドキュメント：[https://experienceleague.adobe.com/ja/docs/marketo-developer/marketo/rest/lead-database/lead-database](https://experienceleague.adobe.com/ja/docs/marketo-developer/marketo/rest/lead-database/lead-database){target="_blank"}
   * リードの同期に関する API ドキュメント：[https://developer.adobe.com/marketo-apis/api/mapi/#tag/Leads/operation/syncLeadUsingPOST](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Leads/operation/syncLeadUsingPOST){target="_blank"}

1. MS [!DNL Dynamics] の商談を Marketo に同期します。

   この MS [!DNL Dynamics] の商談用に Marketo の商談をアップサートする必要があります。商談のアップサートには、「_externalOpportunityId_」、「_externalCompanyId_」および「_externalSalesPersonId_」フィールドが必須です。

   <table>
    <colgroup>
     <col>
     <col>
     <col>
    </colgroup>
    <tbody>
     <tr>
      <td><strong>Marketo「商談」オブジェクトフィールド</strong></td>
        <td><strong>MS <span class="dnl">Dynamics</span>「商談オブジェクト」フィールド</strong></td>
      <td><strong>説明</strong></td>
     </tr>
     <tr>
      <td>externalOpportunityId</td>
        <td>MS <span class="dnl">Dynamics</span> のリード／取引先責任者の大文字小文字を区別しないグローバルな一意の ID</td>
      <td>外部 MS <span class="dnl">Dynamics</span> 商談オブジェクトに対する Marketo 商談レコードを特定します。</td>
     </tr>
     <tr>
      <td>externalCompanyId</td>
        <td>MS <span class="dnl">Dynamics</span> アカウントの大文字小文字を区別しないグローバルな一意の ID</td>
        <td>この商談が属する外部 MS <span class="dnl">Dynamics</span> アカウントオブジェクトを特定します。<br><br>最初に MS <span class="dnl">Dynamics</span> アカウントを正しく同期させる必要があります。</td>
     </tr>
     <tr>
      <td>externalSalesPersonId</td>
        <td>MS <span class="dnl">Dynamics</span> セールスユーザの大文字小文字を区別しないグローバルな一意の ID</td>
        <td>この商談を所有する外部 MS <span class="dnl">Dynamics</span> セールスユーザオブジェクトを特定します。 </td>
     </tr>
    </tbody>
   </table>

   * 商談に関する API ドキュメント：[https://experienceleague.adobe.com/ja/docs/marketo-developer/marketo/rest/lead-database/opportunities](https://experienceleague.adobe.com/ja/docs/marketo-developer/marketo/rest/lead-database/opportunities){target="_blank"}
   * 商談の同期に関する API ドキュメント：[https://developer.adobe.com/marketo-apis/api/mapi/#tag/Opportunities/operation/syncOpportunitiesUsingPOST](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Opportunities/operation/syncOpportunitiesUsingPOST){target="_blank"}

1. MS [!DNL Dynamics] の取引先責任者ロールを Marketo に同期します。

   MS [!DNL Dynamics] の商談の MS [!DNL Dynamics] 取引先責任者ロールは、Marketo 商談ロールを介して同期できます。商談ロールレコードには、「_externalOpportunityId_」、「_role_」および「_leadId_」フィールドが必須です。

   <table>
    <colgroup>
     <col>
     <col>
     <col>
    </colgroup>
    <tbody>
     <tr>
      <td><strong>Marketo「商談ロール」フィールド</strong></td>
        <td><strong>MS <span class="dnl">Dynamics</span>「取引先責任者ロール」フィールド</strong></td>
      <td><strong>説明</strong></td>
     </tr>
     <tr>
      <td>externalOpportunityId</td>
        <td>MS <span class="dnl">Dynamics</span> 商談の大文字小文字を区別しないグローバルな一意の ID</td>
      <td>外部 MS <span class="dnl">Dynamics</span> 商談オブジェクトに対する Marketo 商談ロールを特定します。<br><br>最初に MS <span class="dnl">Dynamics</span> 商談を正しく同期させる必要があります。</td>
     </tr>
     <tr>
      <td>leadId</td>
      <td>該当なし、これは Marketo のリード ID になります</td>
        <td>これは、同期された MS <span class="dnl">Dynamics</span> 取引先責任者の Marketo リード ID になります。<br><br>取引先責任者が Marketo で同期されると、MS <span class="dnl">Dynamics</span> の取引先責任者の大文字と小文字を区別しないグローバルな一意の ID を externalPersonId として使用し、Marketo REST API を使用して Marketo のリードをクエリできます。</td>
     </tr>
     <tr>
      <td>ロール</td>
        <td>MS <span class="dnl">Dynamics</span> の取引先責任者の「ロール」フィールド</td>
      <td>この商談の取引先責任者のロールを記述します。</td>
     </tr>
    </tbody>
   </table>

   * 商談に関する API ドキュメント：[https://experienceleague.adobe.com/ja/docs/marketo-developer/marketo/rest/lead-database/opportunities](https://experienceleague.adobe.com/ja/docs/marketo-developer/marketo/rest/lead-database/opportunities){target="_blank"}
   * 商談の同期に関する API ドキュメント：[https://developer.adobe.com/marketo-apis/api/mapi/#tag/Opportunities/operation/syncOpportunitiesUsingPOST](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Opportunities/operation/syncOpportunitiesUsingPOST){target="_blank"}

1. 「最新の注目のアクション」フィールド、「MSI スコア」フィールドを MS [!DNL Dynamics] に同期します。

   MS [!DNL Dynamics] オブジェクトが Marketo に正しく同期されると、MSI 機能を活用できるようになります。MSI の「最新の注目のアクション」／「スコア」フィールドは、リードの REST API で公開されます。これらのフィールドは、MSI によって計算され、読み取り専用です。

   Marketo のリードの「最新の注目のアクション」フィールドや「スコア」フィールドは、REST API リードエンドポイントを使用することで、定期的に MS [!DNL Dynamics] に同期される必要があります。_externalPersonId_ を filterType として使用し、MS [!DNL Dynamics] リード GUID に filterValue として渡して、このエンドポイントに Marketo リードをクエリします。

   | GET /rest/v1/leads.json?filterType=externalPersonId&amp;filterValues=MS DynamicsLeadId1,MS DynamicsLeadId2 |
   |---|

   これで、これらのフィールドの値を使用して、MS [!DNL Dynamics] のリード／取引先責任者オブジェクトに同期させることができます。

   <table>
    <colgroup>
     <col>
     <col>
     <col>
    </colgroup>
    <tbody>
     <tr>
      <td><strong>Marketo「リード」フィールド</strong></td>
        <td><strong>MS <span class="dnl">Dynamics</span>「リード／取引先責任者」フィールド</strong></td>
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

   * リード REST API 向けドキュメント：[https://developer.adobe.com/marketo-apis/api/mapi/#tag/Leads/operation/getLeadByIdUsingGET](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Leads/operation/getLeadByIdUsingGET){target="_blank"}

   >[!NOTE]
   >
   >リード/連絡先およびアカウントのオブジェクトタイプの場合：Marketoでは、Marketo Sales Insights を使用する際に、独自のカスタムフィールドを外部 ID フィールドとして使用する機能がサポートされています。 このカスタマイズに関するヘルプが必要な場合は、[Marketo サポート &#x200B;](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"} にお問い合わせください。

   非ネイティブ同期を成功させるには、外部フィールドを適切に使用することが重要です。一部のビューにデータが表示されない場合は、特定のフィールドが正しく同期されていない可能性があります。例えば、リードのアカウントの下にある MSI ウィジェットを参照したときにリードのアクティビティや関心を引くモーメントが表示されない場合は、リードの会社またはアカウントが正しく同期されていない可能性があります。外部フィールドを指定してこのリードに対して GET リクエストを実行すると、リードが正しく同期されたかどうかを検証できます。また、Marketo の外部セールス担当者のメールは、MS Dynamics のそのユーザのメールと一致する必要があります。メールが一致しない場合、MS Dynamics の「Marketo」タブにデータが表示されないことがあります。
