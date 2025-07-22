---
unique-page-id: 7511512
description: Salesforce1 での Marketo Sales Insight のインストールおよび設定 - Marketo ドキュメント - 製品ドキュメント
title: Salesforce1 での Marketo Sales Insight のインストールおよび設定
exl-id: 9f26e90b-3199-4ef8-92bc-95e8bd81f1c5
feature: Marketo Sales Insights
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '346'
ht-degree: 70%

---

# [!DNL Marketo Sales Insight] での [!DNL Salesforce1] のインストールと設定 {#install-and-configure-marketo-sales-insight-in-salesforce}

>[!NOTE]
>
>既存のお客様の場合は、続ける前に [MSI パッケージをアップグレード](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md)してください。

>[!PREREQUISITES]
>
>Salesforce Enterprise／Unlimited をお持ちの場合：
>
>* [ 手順 1/3:Marketo フィールドの追加先  [!DNL Salesforce]  （Enterprise/Unlimited） ](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md)
>* [ 手順 2/3:Marketoのユーザー  [!DNL Salesforce]  作成（Enterprise/Unlimited） ](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md)
>* [ 手順 3/3:Marketoと  [!DNL Salesforce]  を接続する（Enterprise/Unlimited） ](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-3-of-3-connect-marketo-and-salesforce-enterprise-unlimited.md)
>* [Configure [!DNL Marketo Sales Insight] in [!DNL Salesforce] Enterprise/Unlimited](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md)
>
>Salesforce Professional をお持ちの場合：
>
>* [Salesforce Professional Edition での Marketo Sales Insight の設定](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md)
>

>[!NOTE]
>
>[!DNL Marketo Sales Insight] の [!DNL Salesforce1] には、[!DNLB ベストベット ]、リードフィード、注目のモーメント、Marketo Campaign に追加が含まれます。

## [!DNL Salesforce1] モバイルアプリの有効化 {#enable-the-salesforce1-mobile-app}

1. 「**[!DNL Setup]**」をクリックし、「**[!DNL Mobile Administration]**」をクリックします。

   ![](assets/image2015-4-21-15-3a29-3a22.png)

1. 「**[!UICONTROL Salesforce1]**」をクリックします。

   ![](assets/image2015-4-21-15-3a30-3a51.png)

1. 「**[!UICONTROL Salesforce1 設定]**」をクリックします。

   ![](assets/image2015-4-21-15-3a32-3a21.png)

1. 「**[!UICONTROL Salesforce1 モバイルブラウザーアプリを有効にする]**」をクリックします。

   ![](assets/image2015-4-21-15-3a34-3a27.png)

1. 「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/image2015-4-21-15-3a42-3a48.png)

1. 「**[!UICONTROL モバイル管理]**」を選択します。

   ![](assets/image2015-4-22-11-3a10-3a14.png)

1. 「**[!UICONTROL モバイルナビゲーションメニューを管理]**」をクリックします。

   ![](assets/image2015-4-22-11-3a13-3a10.png)

1. 「**[!UICONTROL Marketo]**」を選択して、**[!UICONTROL 選択済み]**&#x200B;メニュー項目に&#x200B;**[!UICONTROL 追加]**&#x200B;します。

   ![](assets/image2015-4-22-14-3a55-3a37.png)

1. 「**[!UICONTROL Marketo]**」を選択して、目的の領域まで&#x200B;**[!UICONTROL 上]**&#x200B;に移動し、「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/image2015-4-22-17-3a20-3a56.png)

## 古い Marketo カスタムオブジェクトを非表示にする {#hide-outdated-marketo-custom-object}

1. 「**[!UICONTROL 設定]**」をクリックします。

   ![](assets/image2015-4-22-15-3a13-3a48.png)

1. 「**[!UICONTROL ユーザを管理]**」を選択します。

   ![](assets/image2015-5-5-11-3a13-3a45.png)

1. 「**[!UICONTROL プロファイル]**」を選択します。

   ![](assets/image2015-5-5-11-3a15-3a21.png)

1. 目的のプロファイルをクリックして **[!UICONTROL 編集]** します。

   ![](assets/image2015-5-5-13-3a51-3a36.png)

1. 「**[!UICONTROL タブ設定]**」で&#x200B;_1 番目の_「**[!UICONTROL Marketo]**」を選択します。

   ![](assets/image2015-5-5-13-3a55-3a36.png)

1. 「**[!UICONTROL 非表示タブ]**」を選択します。

   ![](assets/image2015-5-5-14-3a2-3a29.png)

   >[!NOTE]
   >
   >必要なすべてのプロファイルに対して、「Marketo」タブを必ず非表示にします。

## タブのカスタマイズ {#customize-tabs}

1. 「**+**」をクリックします。

   ![](assets/image2015-4-22-17-3a14-3a49.png)

1. 「**[!UICONTROL マイタブをカスタマイズ]**」をクリックします。

   ![](assets/image2015-4-22-17-3a16-3a22.png)

1. 「**[!UICONTROL Marketo]**」を選択して、選択済みタブに&#x200B;**[!UICONTROL 追加]**&#x200B;します。

   ![](assets/image2015-4-22-17-3a17-3a15.png)

1. 「**[!UICONTROL Marketo]**」を選択して、目的の領域まで&#x200B;**[!UICONTROL 上]**&#x200B;に移動し、「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/image2015-4-22-18-3a29-3a47.png)

## ページレイアウトのカスタマイズ {#customize-page-layouts}

1. 「**[!UICONTROL 設定]**」をクリックします。

   ![](assets/image2015-4-22-17-3a26-3a56.png)

1. 「**[!UICONTROL 設定]**」をクリックして、「**[!UICONTROL ページレイアウト]**」と入力して「リード」の「**[!UICONTROL ページレイアウト]**」をクリックします。

   >[!NOTE]
   >
   >連絡先、アカウント、商談のオブジェクトに対して、組織が使用するすべてのページレイアウト（マーケティング、販売など）について手順を繰り返します。

   ![](assets/image2015-4-22-17-3a34-3a33.png)

1. 「**[!UICONTROL 編集]**」をクリックして、リードレイアウトを変更します。

   ![](assets/image2015-4-22-17-3a44-3a0.png)

1. 「**[!UICONTROL Visualforce ページ]**」をクリックして、**[!UICONTROL リードモバイル]**&#x200B;をモバイルカードセクションにドラッグします。

   ![](assets/image2015-4-22-17-3a49-3a37.png)

1. 「高さ」を 66 に変更し、「**[!UICONTROL OK]**」をクリックします。

   ![](assets/image2015-4-22-17-3a52-3a15.png)

1. 「**[!UICONTROL フィールド]**」をクリックして、「**[!UICONTROL Marketo キャンペーンに追加]**」を **[!UICONTROL Marketo Sales Insight]** セクションにドラッグします。

   ![](assets/configure-step-6.png)

   >[!TIP]
   >
   >クイック検索に「Add to」と入力すると、Marketo キャンペーンに簡単に追加できます。

1. 「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/image2015-4-22-18-3a1-3a56.png)

もう少しです。[!DNL Marketo Sales Insight] for [!DNL Salesforce1] のインストールが完了しました。 これで安心です。

>[!MORELIKETHIS]
>
>* [[!DNL Best Bets] in [!DNL Salesforce1]](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/msi-for-mobile/best-bets-in-salesforce1.md)
>* [ 注目のアクション  [!DNL Salesforce1]](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/msi-for-mobile/interesting-moments-in-salesforce1.md)
>* [Marketoのメール送信、Campaign および監視リストのアクション  [!DNL Salesforce1]](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/msi-for-mobile/send-marketo-email-and-campaign-and-watchlist-actions-in-salesforce1.md)
