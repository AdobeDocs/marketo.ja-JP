---
unique-page-id: 2950578
description: ソーシャルプロファイルデータの管理 —Marketoドキュメント — 製品ドキュメント
title: ソーシャルプロファイルデータの管理
exl-id: 9b20c6fc-5c80-4665-9c93-1bb6e53a29ae
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '304'
ht-degree: 7%

---

# ソーシャルプロファイルデータの管理{#manage-social-profile-data}

誰かがMarketoの[ソーシャルアプリ](/help/marketo/product-docs/demand-generation/social/configuring-social-actions/customize-social-app-button.md)と対話したり、ソーシャルネットワークで[ソーシャルフォームの記入](/help/marketo/product-docs/demand-generation/forms/form-actions/enable-social-form-fill-on-a-form.md)を事前入力することを承認したりすると、Marketoはソーシャルプロファイルから使用可能なすべてのデータを取り込みます。 [個人の詳細ページ](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md)でこの表示を行うか、スマートリスト](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/create-and-change-views-for-lists-and-smart-list.md)のカスタム表示[の列として追加します。

ソーシャルフォームの入力とソーシャルアプリでは、少し異なるフィールドのセットが取り込まれます。以下の各セクションを参照してください。

>[!AVAILABILITY]
>
>この機能を購入していないお客様もいます。  詳細は、営業取引先責任者にお問い合わせください。

## Socialアプリでキャプチャ{#captured-via-social-app}

ネットワークのプライバシー設定とユーザーのプライバシー設定に応じて、次のフィールドが1つ以上取得されます。

>[!NOTE]
>
>ソーシャルネットワークからの追加情報は、個人が承認されてから約5分後に、個人の詳細ページに表示されます。

## twitter:{#from-twitter}

* 名（表示名から解析）
* 姓（表示名から解析）
* プロファイル写真のURL
* プロファイルページのURL
* ソーシャルリーチ(フォロワー数)

>[!NOTE]
>
>ソーシャルアプリでは、ユーザーの電子メールアドレスは取得されません。

## facebook:{#from-facebook}

* 名 
* 姓
* プロファイルURL
* プロファイル写真のURL
* 性別
* ソーシャルリーチ（友達の数）

### ソーシャルフォームの入力を介してキャプチャ{#captured-via-social-form-fill}

ネットワークのプライバシー設定とユーザーのプライバシー設定に応じて、次のフィールドが1つ以上取得されます。

>[!CAUTION]
>
>ソーシャルフォームの入力によって取り込まれたデータは、フォームレベル](/help/marketo/product-docs/administration/field-management/block-updates-to-a-field.md)でこれらのフィールドの更新を[ブロックしない限り、一致するフィールドを上書きします。

## twitter:{#from-twitter-1}

* 名（表示名から解析）
* 姓（表示名から解析）
* メール

## facebook:{#from-facebook-1}

* 名 
* 姓
* メール
* 生年月日
* 職位
* 企業

>[!NOTE]
>
>ソーシャルフォームの入力では、ユーザーがフォームに入力した場合に、電子メールアドレス&#x200B;_のみ_&#x200B;を取得します。 電子メールアドレスが必要な場合は、[フォーム](/help/marketo/product-docs/demand-generation/forms/creating-a-form/make-a-form-field-required.md)の必須フィールドにする必要があります。

>[!MORELIKETHIS]
>
>フォームからこの情報を取り込むには、[ソーシャルフォームの記入](/help/marketo/product-docs/demand-generation/forms/form-actions/enable-social-form-fill-on-a-form.md)を有効にします。
