---
unique-page-id: 2950578
description: ソーシャルプロファイルデータの管理 — Marketto Docs — 製品ドキュメント
title: ソーシャルプロファイルデータの管理
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '345'
ht-degree: 0%

---


# ソーシャルプロファイルデータの管理{#manage-social-profile-data}

誰かがMarketor [ソーシャルアプリ](../../../../product-docs/demand-generation/social/configuring-social-actions/customize-social-app-button.md)とやり取りするか、ソーシャルネットワークで[ソーシャルフォームの記入](../../../../product-docs/demand-generation/forms/form-actions/enable-social-form-fill-on-a-form.md)を事前入力することを承認すると、Marketoはソーシャルプロファイルから利用可能なすべてのデータを取り込みます。 [個人の詳細ページ](http://docs.marketo.com/display/DOCS/Using+the+Person+Detail+Page)でこの表示を行うか、スマートリスト](http://docs.marketo.com/display/DOCS/Create+and+Change+Views+for+Lists+and+Smart+List)のカスタム表示[の列として追加します。

ソーシャルフォームの入力とソーシャルアプリでは、少し異なるフィールドのセットが取り込まれます。以下の各セクションを参照してください。

>[!NOTE]
>
>**可用性**
>
>この機能を購入していないお客様もいます。 詳細については、セールス担当者にお問い合わせください。

## Socialアプリでキャプチャ{#captured-via-social-app}

ネットワークのプライバシー設定とユーザーのプライバシー設定に応じて、次のフィールドが1つ以上取得されます。

>[!NOTE]
>
>ソーシャルネットワークからの追加情報は、個人が承認されてから約5分後に、個人の詳細ページに表示されます。

## Twitterから：{#from-twitter}

* 名（表示名から解析）
* 姓（表示名から解析）
* プロファイル写真のURL
* プロファイルページのURL
* ソーシャルリーチ(フォロワー数)

>[!NOTE]
>
>ソーシャルアプリでは、ユーザーの電子メールアドレスは取得されません。

## Facebookから：{#from-facebook}

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
>ソーシャルフォームの入力によって取り込まれたデータは、フォームレベル](../../../../product-docs/administration/field-management/block-updates-to-a-field.md)でこれらのフィールドの更新を[ブロックしない限り、一致するフィールドを上書きします。

## Twitterから：{#from-twitter-1}

* 名（表示名から解析）
* 姓（表示名から解析）
* 電子メール

## Facebookから：{#from-facebook-1}

* 名
* 姓
* 電子メール
* 生年月日
* 肩書
* 会社

>[!NOTE]
>
>ソーシャルフォームの入力では、ユーザーがフォームに入力した場合に、電子メールアドレス&#x200B;*のみ*&#x200B;を取得します。 電子メールアドレスが必要な場合は、[フォーム](../../../../product-docs/demand-generation/forms/creating-a-form/make-a-form-field-required.md)の必須フィールドにする必要があります。

>[!MORELIKETHIS]
>
>フォームからこの情報を取り込むには、[ソーシャルフォームの記入](../../../../product-docs/demand-generation/forms/form-actions/enable-social-form-fill-on-a-form.md)を有効にします。

>[!NOTE]
>
>**ディープダイブ**
>
>フォームの使用に関する詳細は、[Forms](http://docs.marketo.com/display/docs/forms)ディープダイビングを参照してください。

