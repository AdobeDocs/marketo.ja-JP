---
unique-page-id: 3571838
description: Microsoft Dynamics Sync - Field Sync - Marketto Docs — 製品ドキュメント
title: Microsoft Dynamics Sync — フィールド同期
translation-type: tm+mt
source-git-commit: 96cc6a30c63c8e8dca793a52e4bf7ecaef8c08dc
workflow-type: tm+mt
source-wordcount: '364'
ht-degree: 0%

---


# Microsoft Dynamics同期：フィールドの同期 {#microsoft-dynamics-sync-field-sync}

>[!NOTE]
>
>**FYI**
>
>Marketoは現在、すべての購読で言語を標準化しているので、購読およびdocs.marketo.comの人物/人物にリード/リードを表示できます。 これらの用語は同じことを意味し、記事の説明には影響しません。 他にも変化がある。 [詳細情報](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology)。

MarkettoとDynamicsの同期は非常に強力です。 詳しくは、

## 2つのシステム間でフィールドの詳細を同期させる方法 {#how-are-field-details-kept-in-sync-between-the-two-systems}

同期は、リードと連絡先のエンティティに対しては双方向です。 Dynamicsのリードや連絡先、またはMarketoの担当者に変更を加えると、両方のシステムに更新が反映されます。

アカウント、ユーザー、オポチュニティ、チーム、カスタムエンティティの場合、同期は一方向です。Dynamics to Marketor。 Dynamicsでこれらのエンティティに変更を加えると、Marketorに更新が反映されます。

## 両方のシステムの同じフィールドに変更が同時に行われた場合はどうなりますか。 （データの衝突） {#what-if-changes-are-made-to-the-same-field-in-both-systems-at-the-same-time-data-collision}

これはまれですが、Marketoは人（リード）に勝ち、Dynamicsは連絡先に勝ちます。 これは、マーケティング部門が人々に対して権限を持つと考えられるのに対し、連絡先の正式な記録システムは販売部門(CRM)にあるからです。 一方向同期エンティティの場合、Dynamicsは常に勝ちます。

## Marketoを使用してDynamicsでフィールドを作成できますか？ {#can-i-create-a-field-in-dynamics-using-marketo}

いいえ。現在、この機能はサポートされていません。

## Dynamicsにフィールドを作成しました。 Marketoと同期できますか。 {#i-created-a-field-in-dynamics-can-i-sync-it-to-marketo}

はい、同期ユーザーがDynamicsでフィールドにアクセスできる限り [、フィールドを同期できます](https://docs.marketo.com/pages/viewpage.action?pageId=3571830#Step3of3:ConnectMicrosoftDynamicswithMarketo(Online)-SelectFieldstoSync) 。

Marketoと同期するフィールドは何ですか。

セットアップ時に同期するフィールドを [選択できます](https://docs.marketo.com/pages/viewpage.action?pageId=3571830#Step3of3:ConnectMicrosoftDynamicswithMarketo(Online)-SelectFieldstoSync) 。

## MarketorとDynamicsの同期後にカスタムフィールドを追加する必要がある場合はどうなりますか？ {#what-if-i-need-to-add-a-custom-field-after-marketo-and-dynamics-are-synced}

いつでもフィールドを追加でき、DynamicsからMarketorにデータが更新されるように期待できます。 詳細については、 [「新しいカスタムフィールドに対してMicrosoft Dynamicsとのクイック同期を使用する](microsoft-dynamics-sync-field-sync/use-quick-sync-with-microsoft-dynamics-for-a-new-custom-field.md) 」を参照してください。

>[!NOTE]
>
>**関連記事**
>
>* [Microsoft Dynamicsとのクイック同期を使用して新しいカスタムフィールドを作成する](microsoft-dynamics-sync-field-sync/use-quick-sync-with-microsoft-dynamics-for-a-new-custom-field.md)

>



