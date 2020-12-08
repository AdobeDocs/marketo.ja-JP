---
unique-page-id: 2950578
description: ソーシャルプロファイルデータの管理 — Marketto Docs — 製品ドキュメント
title: ソーシャルプロファイルデータの管理
translation-type: tm+mt
source-git-commit: 313266a67243f0c70c25010cb4825efb7f3db0ab
workflow-type: tm+mt
source-wordcount: '398'
ht-degree: 0%

---


# ソーシャルプロファイルデータの管理 {#manage-social-profile-data}

誰かがMarketo [Socialアプリを操作したり、ソーシャルネットワークでMarketoフォームに](../../../../product-docs/demand-generation/social/configuring-social-actions/customize-social-app-button.md)ソーシャルフォームの入力を事前入力することを承認した場合 [](../../../../product-docs/demand-generation/forms/form-actions/enable-social-form-fill-on-a-form.md)、Marketorは、ソーシャルプロファイルから利用可能なすべてのデータを取り込みます。 この情報は、 [個人の詳細ページで表示するか](http://docs.marketo.com/display/DOCS/Using+the+Person+Detail+Page)、スマートリストの [カスタム表示の列として追加できます](http://docs.marketo.com/display/DOCS/Create+and+Change+Views+for+Lists+and+Smart+List)。

>[!NOTE]
>
>**FYI**
>
>Marketoは現在、すべての購読で言語を標準化しているので、購読およびdocs.marketo.comの人物/人物にリード/リードを表示できます。 これらの用語は同じことを意味し、記事の説明には影響しません。 他にも変化がある。 [詳細情報](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology)。

ソーシャルフォームの入力とソーシャルアプリでは、少し異なるフィールドのセットが取り込まれます。以下の各セクションを参照してください。

>[!NOTE]
>
>**可用性**
>
>この機能を購入していないお客様もいます。 詳細については、セールス担当者にお問い合わせください。

## Socialアプリでキャプチャ {#captured-via-social-app}

ネットワークのプライバシー設定とユーザーのプライバシー設定に応じて、次のフィールドが1つ以上取得されます。

>[!NOTE]
>
>ソーシャルネットワークからの追加情報は、個人が承認されてから約5分後に、個人の詳細ページに表示されます。

## Twitterから： {#from-twitter}

* 名（表示名から解析）
* 姓（表示名から解析）
* プロファイル写真のURL
* プロファイルページのURL
* ソーシャルリーチ(フォロワー数)

>[!NOTE]
>
>ソーシャルアプリでは、ユーザーの電子メールアドレスは取得されません。

## Facebookから： {#from-facebook}

* 名
* 姓
* プロファイルURL
* プロファイル写真のURL
* 性別
* ソーシャルリーチ（友達の数）

### ソーシャルフォームの入力を介してキャプチャ {#captured-via-social-form-fill}

ネットワークのプライバシー設定とユーザーのプライバシー設定に応じて、次のフィールドが1つ以上取得されます。

>[!CAUTION]
>
>ソーシャルフォームの入力によって取り込まれたデータは、フォームレベルでこれらのフィールドの更新を [ブロックしない限り、一致するフィールドを上書きします](../../../../product-docs/administration/field-management/block-updates-to-a-field.md)。

## Twitterから： {#from-twitter-1}

* 名（表示名から解析）
* 姓（表示名から解析）
* 電子メール

## Facebookから： {#from-facebook-1}

* 名
* 姓
* 電子メール
* 生年月日
* 肩書
* 会社

>[!NOTE]
>
>ソーシャルフォームの入力では、ユーザーがフォームに電子メールアドレスを入力した *場合にのみ* 、電子メールアドレスを取り込みます。 電子メールアドレスが必要な場合は、フォームの必須フィールド [にする必要があります](../../../../product-docs/demand-generation/forms/creating-a-form/make-a-form-field-required.md)。

>[!NOTE]
>
>**関連記事**
>
>フォームからこの情報を取り込むには、 [ソーシャルフォームの入力を有効にし](../../../../product-docs/demand-generation/forms/form-actions/enable-social-form-fill-on-a-form.md)ます。

>[!NOTE]
>
>**ディープダイブ**
>
>フォームの操作について詳しくは、 [Forms](http://docs.marketo.com/display/docs/forms) 詳細レポートを参照してください。

