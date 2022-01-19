---
description: プッシュ複製 — Marketoドキュメント — 製品ドキュメント
title: 複製をプッシュ
hide: true
hidefromtoc: true
source-git-commit: 8920bc525075923b32e7330da20debb7b8f47b06
workflow-type: tm+mt
source-wordcount: '467'
ht-degree: 38%

---

# 複製をプッシュ {#push-clone}

この機能を使用すると、Adobe Experience Platform にあるセグメントを静的リストの形式で Marketo にプッシュできます。

>[!PREREQUISITES]
>
>* Marketo で [API ユーザーを作成](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user.md)します。
>* 次に、**管理**／ **Launchpoint** に移動します。作成した役割の名前を探し、「**詳細を表示**」をクリックします。この機能に必要なので、**クライアント ID** と&#x200B;**クライアントシークレット**&#x200B;の情報をコピーして保存します。


1. [Adobe Experience Platform](https://experience.adobe.com/) にログインします。

   ![](assets/push-an-adobe-experience-platform-segment-1.png)

1. グリッドアイコンをクリックし、「**Experience Platform**」を選択します。

   ![](assets/push-an-adobe-experience-platform-segment-2.png)

1. 左側のナビゲーションで、「**宛先**」をクリックします。

   ![](assets/push-an-adobe-experience-platform-segment-3.png)

1. 「**カタログ**」をクリックします。

   ![](assets/push-an-adobe-experience-platform-segment-4.png)

1. 「Marketo Engage」タイルを探し、 **セグメントのアクティブ化**.

   ![](assets/push-an-adobe-experience-platform-segment-5.png)

1. クリック **新しい宛先の設定**.

   ![](assets/push-an-adobe-experience-platform-segment-6.png)


1. 「アカウントタイプ」で、「既存または新規のアカウント」ラジオボタンを選択します ( この例では、 **既存のアカウント**) をクリックします。 「アカウントを選択」アイコンをクリックします。

   ![](assets/push-an-adobe-experience-platform-segment-7.png)

1. 宛先アカウントを選択し、 **選択**.

   ![](assets/push-an-adobe-experience-platform-segment-8.png)

次に、既存のMarketoの人物のみを照合するか、既存のMarketoの人物と照合してMarketoで足りない人物を作成するかを選択する必要があります。 以下に、それぞれの方法を説明する節を示します。

## 既存のMarketoの担当者の照合とMarketoでの見つからない担当者の作成 {#match-existing-marketo-people-create-missing-people}

上記の手順 1～8 に従った後、

1. 宛先を入力 **名前** およびオプションの説明。 ユーザーの作成ドロップダウンをクリックし、 **既存のMarketoの担当者の照合とMarketoでの見つからない担当者の作成**.

   ![](assets/push-an-adobe-experience-platform-segment-9.png)

1. この節はオプションです。 クリック **作成** スキップします。

   ![](assets/push-an-adobe-experience-platform-segment-10.png)

1. 作成した宛先を選択し、「 **次へ**.

   ![](assets/push-an-adobe-experience-platform-segment-11.png)

1. Marketoに送信するセグメントを選択し、 **次へ**.

   ![](assets/push-an-adobe-experience-platform-segment-12.png)

1. 「**新規マッピングを追加**」をクリックします。

   ![](assets/push-an-adobe-experience-platform-segment-13.png)

1. マッピングアイコンをクリックします。

   ![](assets/push-an-adobe-experience-platform-segment-14.png)

1. 「 」を選択して名をマッピング **firstName** をクリックし、 **選択**.

   ![](assets/push-an-adobe-experience-platform-segment-15.png)

1. 「 **新しいマッピングを追加** を繰り返し、手順 7 を 2 回繰り返します。lastName を選択し、次に companyName を選択します。

   ![](assets/push-an-adobe-experience-platform-segment-16.png)

1. 次に、E メールアドレスをマッピングします。 クリック **新しいマッピングを追加** 再び

   ![](assets/push-an-adobe-experience-platform-segment-17.png)

1. マッピングアイコンをクリックします。

   ![](assets/push-an-adobe-experience-platform-segment-18.png)

1. 「 ID 名前空間を選択」ラジオボタンをクリックし、「  **電子メール**&#x200B;を選択し、「 **選択**.

   ![](assets/push-an-adobe-experience-platform-segment-19.png)

1. 次に、ソースフィールドを選択します。 電子メールの場合は、カーソルアイコンをクリックします。

   ![](assets/push-an-adobe-experience-platform-segment-20.png)

1. 「 ID 名前空間を選択」ラジオボタンをクリックし、「検索」をクリックして「 **電子メール**&#x200B;を選択し、「 **選択**.

   ![](assets/push-an-adobe-experience-platform-segment-21.png)

MORREEEE

## 既存のMarketo担当者のみに一致 {#match-existing-marketo-people-only}

>[!NOTE]
>
>ID は、Marketoで一致を検索するために使用されます。 一致が見つかった場合、そのユーザーは静的リストに追加されます。 一致が見つからない場合、そのユーザーは削除されます ( つまり、Marketoで作成されません )。

1. _Marketo_ で、静的リストを作成するか、既に作成した静的リストを見つけて選択します。URL の末尾からマッピング ID をコピーします。

PICC

>[!NOTE]
>
>最良の結果を得るには、Marketo で参照するリストが空であることを確認してください。

1. Adobe Experience Platform に戻り、コピーした ID を入力します。「開始日」を選択します。選択された終了日まで同期が続きます。無期限同期の場合は、終了日を空白のままにします。終了したら「**次へ**」をクリックします。

PICC

1. 変更を確認し、「**完了**」をクリックします。

PICC
