---
unique-page-id: 4720232
description: 新しいアカウントリストの作成 —Marketoドキュメント — 製品ドキュメント
title: 新しいアカウントリストの作成
exl-id: 644c5b3b-852a-4dd9-8e55-b434505504ea
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '404'
ht-degree: 12%

---

# 新しいアカウントリストの作成{#create-a-new-account-list}

組織名とドメイン名のリストを作成し、パーソナライズされたキャンペーンを持つターゲットにこれらの主要アカウントをアップロードします。

>[!NOTE]
>
>この記事は、レガシーのWeb ABMユーザーのみを対象とします。 2016年9月以降にWeb ABMを取得した場合は、[この記事](https://docs.marketo.com/display/DOCS/Account+Lists#AccountLists-CreateaNewAccountList)の手順に従ってください。

## 新しいアカウントリストの作成{#create-a-new-account-list-1}

1. **アカウントリスト**&#x200B;に移動します。

   ![](assets/dropdown-account-lists-hand.jpg)

1. 「**新規作成**」を選択します。

   ![](assets/create-new-account-list-hand.jpg)

1. 「**参照**」を選択し、CSVファイルをアップロードします（csvファイルが条件を満たしていることを確認します）。 追加&#x200B;**名前**&#x200B;と&#x200B;**説明**。 「**保存**」をクリックします。

   ![](assets/create-account-list-hands.jpg)

   >[!NOTE]
   >
   >**CSVファイルの形式は何ですか。**
   >
   >この名前のアカウントのCSVファイルが次の要件を満たしていることを確認します。
   >
   >* CSV形式で保存
   >* 10 MBを超えない
   >* ヘッダー列Aを持つ4列のみ：名前、列B:ドメイン、列C:国、列D:米国の州。
   >* アップロードされたファイルが承認されるまでに最大で 2 営業日かかります。
   >* 承認のメール通知が送信されます。あるいは、特定顧客ページでファイルの状態を確認してください。
   >* アップロードしたすべてのリストに対して合計10Kの開始数と、合計100Kの最大パッケージ数が累積されたレコード数/行数です。


   >[!NOTE]
   >
   >**CSVファイルの例**
   >
   >* 行1列A値=組織
   >* 行1列Bの値=ドメイン
   >* 行1列Cの値=国
   >* 行1列D値=米国の州
   >* 列の値の1つは必須です。 ただし、組織名とドメイン名の両方を指定すると、アカウントリストの一致率が向上します。
   >* 国と州はオプションの値です。

      >
      >   
      * 国名には、完全な国名または省略形コードを使用します。 例: 米国または米国。
      >   * 米国の州の場合は、2文字の省略コード（CAなど）を使用します。 米国の州のみが認識されます。

   >
   >![](assets/image2015-2-25-12-3a19-3a10.png)

## アカウントリストの編集{#edit-an-account-list}

**アカウントリスト**&#x200B;ページで、リストの&#x200B;**編集**&#x200B;アイコンをクリックします。

![](assets/create-new-account-list-edit.jpg)

「**参照**」を選択し、新しいCSVファイルをアップロードします。 このファイルは元のファイルを置き換えます。 「**保存**」をクリックします。 新しくアップロードされたファイルは、Marketoサポートによって承認されるまで保留状態になります。保留状態の場合、元のファイルはアクティブなままになります。

![](assets/set-account-list-edit-hands.jpg)

CSV ファイルは既存のファイルに置き換わります。新規ファイルの処理が完了するまで、既存のリストはアクティブなまま保持されます。

## 名前付きアカウントリストの削除{#delete-a-named-account-list}

1. **アカウントリスト**&#x200B;ページで、削除するリストの削除アイコンをクリックします。

   ![](assets/create-new-account-list-delete.jpg)

1. リストを削除するかどうかを確認するメッセージが表示されます。 「**OK**」をクリックします。

   ![](assets/delete-notification-hand.jpg)

>[!MORELIKETHIS]
>
>[アカウントリストを使用したセグメントの作成](/help/marketo/product-docs/web-personalization/account-based-web-marketing/create-a-segment-using-an-account-list.md)
