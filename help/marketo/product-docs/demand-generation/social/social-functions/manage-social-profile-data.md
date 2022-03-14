---
unique-page-id: 2950578
description: ソーシャルプロファイルデータの管理 — Marketo ドキュメント — 製品ドキュメント
title: ソーシャルプロファイルデータの管理
exl-id: 9b20c6fc-5c80-4665-9c93-1bb6e53a29ae
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: ht
source-wordcount: '304'
ht-degree: 100%

---

# ソーシャルプロファイルデータの管理 {#manage-social-profile-data}

ユーザーが Marketo [ソーシャルアプリ](/help/marketo/product-docs/demand-generation/social/configuring-social-actions/customize-social-app-button.md)を使用する、または、ソーシャルネットワークで Marketo フォームに事前に[ソーシャルフォームの入力](/help/marketo/product-docs/demand-generation/forms/form-actions/enable-social-form-fill-on-a-form.md)を許可すると、Marketo はユーザーのソーシャルプロファイルから使用可能なすべてのデータを取り込みます。この情報は、[ユーザーの詳細ページ](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md)で確認できます。また、[スマートリストのカスタム表示](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/create-and-change-views-for-lists-and-smart-list.md)で列として追加することもできます。

ソーシャルフォームの入力とソーシャルアプリで取り込まれるフィールドのセットは少し異なります。以下の各節を参照してください。

>[!AVAILABILITY]
>
>すべてのお客様がこの機能を購入しているわけではありません。詳細は、セールス担当者にお問い合わせください。

## ソーシャルアプリでの取り込み {#captured-via-social-app}

ネットワークのおよびユーザーのプライバシー設定に応じて、次のフィールドの 1 つ以上が取得されます。

>[!NOTE]
>
>ソーシャルネットワークからの追加情報は、ユーザーが承認してから約 5 分後に、ユーザーの詳細ページに表示されます。

## Twitter から： {#from-twitter}

* 名（表示名から解析）
* 姓（表示名から解析）
* プロファイル写真 URL
* プロファイルページ URL
* ソーシャルリーチ（フォロワー数）

>[!NOTE]
>
>ソーシャルアプリは、ユーザーのメールアドレスを取得しません。

## Facebook から： {#from-facebook}

* 名
* 姓
* プロファイル URL
* プロファイル写真 URL
* 性別
* ソーシャルリーチ（友達の数）

### ソーシャルフォームの入力での取り込み {#captured-via-social-form-fill}

ネットワークのおよびユーザーのプライバシー設定に応じて、次のフィールドの 1 つ以上が取得されます。

>[!CAUTION]
>
>ソーシャルフォームの入力で取り込まれたデータは、[フォームレベルでこれらのフィールドの更新をブロック](/help/marketo/product-docs/administration/field-management/block-updates-to-a-field.md)しない限り、一致するフィールドを上書きします。

## Twitter から： {#from-twitter-1}

* 名（表示名から解析）
* 姓（表示名から解析）
* メール

## 開始Facebook: {#from-facebook-1}

* 名
* 姓
* メール
* 生年月日
* 職位
* 企業

>[!NOTE]
>
>ソーシャルフォームの入力がメールアドレスを取り込むのは、ユーザーがそれをフォームに入力した場合&#x200B;_のみ_&#x200B;です。メールアドレスが必要な場合は、[フォームの必須フィールドにします](/help/marketo/product-docs/demand-generation/forms/creating-a-form/make-a-form-field-required.md)。

>[!MORELIKETHIS]
>
>フォームからこの情報を取り込むには、[ソーシャルフォームの入力](/help/marketo/product-docs/demand-generation/forms/form-actions/enable-social-form-fill-on-a-form.md)を有効にします。
