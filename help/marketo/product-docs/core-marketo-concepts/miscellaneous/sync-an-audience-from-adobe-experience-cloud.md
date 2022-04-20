---
description: Adobe Experience Cloud からのオーディエンスの同期 - Marketo ドキュメント - 製品ドキュメント
title: Adobe Experience Cloud からのオーディエンスの同期
exl-id: 2288ee01-2c2e-4f33-b5c9-da3a431c1816
source-git-commit: 86451f1027e74479a415a4c6654a2625275d4112
workflow-type: tm+mt
source-wordcount: '272'
ht-degree: 98%

---

# Adobe Experience Cloud からのオーディエンスの同期 {#sync-an-audience-from-adobe-experience-cloud}

>[!NOTE]
>
>Marketo インスタンスの HIPAA 対応デプロイメントでは、この統合を使用できません。

>[!PREREQUISITES]
>
>[組織マッピングAdobeの設定](/help/marketo/product-docs/core-marketo-concepts/miscellaneous/set-up-adobe-organization-mapping.md)

## オーディエンスの同期方法 {#how-to-sync-an-audience}

1. My Marketo で、「**データベース**」タイルをクリックします。

   ![](assets/sync-an-audience-from-adobe-experience-cloud-1.png)

1. 「**新規**」ドロップダウンをクリックして、「**Experience Cloud オーディエンスから同期**」を選択します。

   ![](assets/sync-an-audience-from-adobe-experience-cloud-2.png)

1. 「**オーディエンスライブラリフォルダー**」ドロップダウンリストをクリックして、目的の元フォルダーを選択します。

   ![](assets/sync-an-audience-from-adobe-experience-cloud-3.png)

1. **オーディエンス名**&#x200B;を選択します。

   ![](assets/sync-an-audience-from-adobe-experience-cloud-4.png)

1. 宛先については、既存のリストを選択するか、新しいリストの名前を入力できます。この例では、新しく作成します。終了したら「**同期**」をクリックします。

   ![](assets/sync-an-audience-from-adobe-experience-cloud-5.png)

1. 「**OK**」をクリックします。

   ![](assets/sync-an-audience-from-adobe-experience-cloud-6.png)

## よくある質問 {#faq}

**Cookie の同期は、どのような仕組みなのですか？**

Marketo サブスクリプションに対して Cookie 同期が有効になっている場合、Marketo の munchkin.js は、統合の設定時に指定した Adobe IMS 組織の Adobe ECID を取得して保存し、その ECID を対応する Marketo の Cookie 識別子に一致させます。これにより、Marketo の匿名ユーザープロファイルを Adobe ECID で強化できます。

匿名ユーザープロファイルをリードプロファイルに関連付けるには、さらに手順を実行する必要があります。リードプロファイルは、テキスト形式メールで識別されます。この機能の正確な仕組みは、[こちらで説明しています](/help/marketo/product-docs/reporting/basic-reporting/report-activity/tracking-anonymous-activity-and-people.md)。

**Marketo のリストサイズがアドビのリストサイズと異なるのはなぜですか？**

Marketo の既知のユーザーに ECID Cookie ID を関連付けることができない場合、ユーザーも同期されません。

**これは 1 回限りの同期ですか？**

同期を開始する必要があるのは 1 回だけです。その後、レコードは自動的に同期されます。初期同期には最大 24 時間かかる場合があります。その後、新しいレコードは 2～3 時間で同期されます。
