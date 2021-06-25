---
description: Adobe Experience CloudセグメントのMarketo静的リストへのプッシュ — Marketoドキュメント — 製品ドキュメント
title: Adobe Experience CloudセグメントのMarketo静的リストへの追加
hidefromtoc: true
source-git-commit: f437495fbe004177f01c57729d97d2fec1f79509
workflow-type: tm+mt
source-wordcount: '397'
ht-degree: 0%

---

# Adobe Experience CloudセグメントのMarketo静的リストへの追加 {#push-an-adobe-experience-cloud-segment-to-a-marketo-static-list}

この機能を使用すると、Adobe Experience Platformにあるセグメントを静的リストの形式でMarketoにプッシュできます。

>[!PREREQUISITES]
>
>* [MarketoでAPIユーザーを](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user.md) 作成します。
>* 次に、**管理者** > **Launchpoint**&#x200B;に移動します。 作成したロールの名前を探し、「**詳細を表示**」をクリックします。 この機能に必要なので、情報を&#x200B;**クライアントID**&#x200B;と&#x200B;**クライアントシークレット**&#x200B;にコピーして保存します。


1. [Adobe Experience Platform](https://experience.adobe.com/)にログインします。

   ![](assets/push-an-adobe-experience-cloud-segment-to-a-marketo-static-list-1.png)

1. グリッドアイコンをクリックし、「**Experience Platform**」を選択します。

   ![](assets/push-an-adobe-experience-cloud-segment-to-a-marketo-static-list-2.png)

1. 左側のナビゲーションで、「**宛先**」をクリックします。

   ![](assets/push-an-adobe-experience-cloud-segment-to-a-marketo-static-list-3.png)

1. 「**カタログ**」をクリックします。

   ![](assets/push-an-adobe-experience-cloud-segment-to-a-marketo-static-list-4.png)

1. Marketo Engageタイルを見つけ、「**アクティブ化**」をクリックします。

   ![](assets/push-an-adobe-experience-cloud-segment-to-a-marketo-static-list-5.png)

1. 「アカウントタイプ」で、「**新しいアカウント**」ラジオボタンをクリックします。 Marketoの資格情報を入力し、「**宛先に接続**」をクリックします。

   ![](assets/push-an-adobe-experience-cloud-segment-to-a-marketo-static-list-6.png)

   >[!NOTE]
   >
   >**管理者** / **Munchkin**&#x200B;に移動すると、Munchkin IDを見つけることができます(ログイン後のMarketo URLの一部でもあります)。 この記事の最上部にある前提条件に従って作成する必要があるクライアントID/シークレット。

1. 「接続済み」が資格情報の下に表示されます。 右上隅の「**次へ**」をクリックします。

   ![](assets/push-an-adobe-experience-cloud-segment-to-a-marketo-static-list-7.png)

1. **名前**&#x200B;と&#x200B;_オプションの_&#x200B;説明を入力します。 「**宛先を作成**」をクリックします。

   >[!NOTE]
   >
   >マーケティングアクションからの選択もオプションです。 Marketoは、現時点ではその情報を活用していませんが、近日中に利用される可能性が高くなります。

   ![](assets/push-an-adobe-experience-cloud-segment-to-a-marketo-static-list-8.png)

1. 「**次へ**」をクリックします。

   ![](assets/push-an-adobe-experience-cloud-segment-to-a-marketo-static-list-9.png)

1. 目的のセグメントを選択し、「**次へ**」をクリックします。

   ![](assets/push-an-adobe-experience-cloud-segment-to-a-marketo-static-list-10.png)

   >[!NOTE]
   >
   >静的リストへのセグメントは1対1です。 ここで複数のセグメントを選択する場合は、「セグメントスケジュール」タブで、各セグメントを指定した静的リストにマッピングする必要があります。

1. 「**新しいマッピングを追加**」をクリックします。

   ![](assets/push-an-adobe-experience-cloud-segment-to-a-marketo-static-list-11.png)

1. カーソルアイコンをクリックします。

   ![](assets/push-an-adobe-experience-cloud-segment-to-a-marketo-static-list-12.png)

1. ユーザーを識別するEメールアドレスを含む関連フィールドを選択します。 終了したら「**選択**」をクリックします。

   ![](assets/push-an-adobe-experience-cloud-segment-to-a-marketo-static-list-13.png)

   ![](assets/push-an-adobe-experience-cloud-segment-to-a-marketo-static-list-14.png)


   >[!NOTE]
   >
   >選択した例は、選択した例とは大きく異なる場合があります。

1. マッピングアイコンをクリックします。

   ![](assets/push-an-adobe-experience-cloud-segment-to-a-marketo-static-list-15.png)

1. ターゲットフィールドを選択し、「**選択**」をクリックします。

   ![](assets/push-an-adobe-experience-cloud-segment-to-a-marketo-static-list-16.png)

1. 「**次へ**」をクリックします。

   ![](assets/push-an-adobe-experience-cloud-segment-to-a-marketo-static-list-17.png)

1. _Marketo_&#x200B;で、静的リストを作成するか、既に作成した静的リストを探して選択します。URLの末尾からマッピングIDをコピーします。

   ![](assets/push-an-adobe-experience-cloud-segment-to-a-marketo-static-list-18.png)

   >[!NOTE]
   >
   >最良の結果を得るには、Marketoで参照するリストが空であることを確認してください。

1. Adobe Experience Platformに戻り、コピーしたIDを入力します。 「開始日」を選択します。 ユーザーは、選択された終了日まで同期を続けます。 無期限同期の場合は、終了日を空白のままにします。 終了したら「**次へ**」をクリックします。

   ![](assets/push-an-adobe-experience-cloud-segment-to-a-marketo-static-list-19.png)

1. 変更を確認し、「**完了**」をクリックします。

   ![](assets/push-an-adobe-experience-cloud-segment-to-a-marketo-static-list-20.png)
