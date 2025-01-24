---
title: Experience Manager Assets の操作
description: Adobe Marketo Engageでコンテンツをオーサリングする際に、接続されたAEM Assets リポジトリの画像アセットを使用する方法について説明します。
hide: true
hidefromtoc: true
source-git-commit: c6132bf5b393df38700ad9dd6f0c6414860e8bb6
workflow-type: tm+mt
source-wordcount: '574'
ht-degree: 2%

---

# Experience Managerアセットの操作

Adobe Experience Manager Assetsのas a Cloud ServiceをAdobe Marketo Engageと統合すると、マーケティングコンテンツで使用するデジタルアセットを簡単に見つけてアクセスできます。 コンテンツを作成する際には、左側のナビゲーションの _[!UICONTROL Assets]_ 項目から、またアカウントジャーニーのメールコンテンツを作成する際に、アセットにアクセスできます。 また、Adobe Journey Optimizer B2B editionから直接、Connected AEM Assetsのas a Cloud Serviceリポジトリにアセットをアップロードできます。

>[!NOTE]
>
>現在、Adobe Journey Optimizer B2B editionでは、Adobe Experience Manager Assetsの画像アセットのみがサポートされています。 アセットに対する変更は、Adobe Experience Manager Assets中央リポジトリから行う必要があります。 [詳細情報](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/manage/manage-digital-assets)

これらのデジタルアセットを使用すると、Assetsのas a Cloud Serviceの最新の変更が、リンクされた参照を通じてライブメールキャンペーンに自動的に反映されます。 Adobe Experience Manager Assetsのas a Cloud Serviceで画像を削除すると、メール内の参照が壊れて画像が表示されます。 現在アカウントジャーニー内で使用されているアセットが変更または削除されると、画像の変更とその画像を使用しているジャーニーのリストがジャーニー作成者に通知されます。 アセットに対するすべての変更は、Adobe Experience Manager Assets中央リポジトリで行う必要があります。

## AEM Assetsを画像ソースとして使用

お使いの環境に 1 つ以上のAssets リポジトリ接続がある場合、メール、メールテンプレートまたはビジュアルフラグメントの詳細を作成または表示する際に、AEM Assetsをアセットのソースとして指定できます。

* 新しいコンテンツを作成する場合は、ダイアログで `AEM Assets` を **[!UICONTROL Image Source]** 項目として選択します。

スクリーンショット

* 既存のコンテンツリソースを開く場合は、右側の _[!UICONTROL 本文]_ パネルで `AEM Assets` を選択します。

スクリーンショット

## オーサリング用アセットへのアクセス

>[!IMPORTANT]
>
>管理者は、Assetsへのアクセスを必要とするユーザーをAssets Consumer Users または/およびAssets Users 製品プロファイルに追加する必要があります。 [詳細情報](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/security/ims-support#managing-products-and-user-access-in-admin-console)

ビジュアルコンテンツエディターで、左側のサイドバーにある _アセットセレクター_ アイコンをクリックします。 これにより、ツールパネルが、選択したリポジトリで使用可能なアセットのリストに変更されます。

スクリーンショット

複数のAEM リポジトリが接続されている場合は、「**[!UICONTROL リポジトリ]**」のメニュー矢印をクリックして、使用するリポジトリを選択します。

スクリーンショット

画像アセットをビジュアルキャンバスに追加するには、複数の方法があります。

* 左側のナビゲーションから画像サムネールをドラッグ&amp;ドロップします。

スクリーンショット

* キャンバスに画像コンポーネントを追加し、「参照 **[!UICONTROL をクリックして]** Assetsを選択 _[!UICONTROL ダイアログを開き]_ す。

  ダイアログで、選択したリポジトリから画像を選択できます。

  必要なアセットを見つけるのに役立つツールが複数あります。

スクリーンショット

* 右上の **[!UICONTROL リポジトリ]** を変更します。

* 右上の **[!UICONTROL アセットを管理]** をクリックして、別のブラウザータブでAssets リポジトリを開き、AEM Assets management tools を使用します。

* 右上の _表示タイプ_ セレクターをクリックして、表示を **[!UICONTROL リスト表示]**、**[!UICONTROL グリッド表示]**、**[!UICONTROL ギャラリー表示]**、**[!UICONTROL ウォーターフォール表示]** に変更します。

* _並べ替え順序_ アイコンをクリックして、並べ替え順序を昇順と降順の間で変更します。

* 「**[!UICONTROL 並べ替え基準]**」メニュー矢印をクリックして、並べ替え条件を **[!UICONTROL 名前]**、**[!UICONTROL サイズ]**、**[!UICONTROL 変更]** に変更します。

* 左上の _フィルター_ アイコンをクリックし、条件に従って表示される項目をフィルタリングします。

* 「検索」フィールドにテキストを入力して、表示される項目をアセット名と一致するようにフィルタリングします。

スクリーンショット
