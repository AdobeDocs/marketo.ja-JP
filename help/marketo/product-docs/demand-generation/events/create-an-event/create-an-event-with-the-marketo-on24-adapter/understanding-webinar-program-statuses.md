---
unique-page-id: 10096681
description: ON24とMarketoの統合におけるウェビナープログラムのステータスについて説明します。 登録済み、参加済み、その他のステータス値を把握できます。
title: ウェビナープログラムのステータスについて
exl-id: ef0b1b94-a612-4aa8-9b4a-aa7ef0e2abaa
feature: Events
TQID: 'https://experienceleague.adobe.com/7TgAEyZElmSgML0nz-FWdw-nTB9WJZMcM-X4PzFJLq4'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: c5620c2c-7950-5a31-936a-f3b3287f198b
    internal-label: Events
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '426'
ht-degree: 86%
---
# ウェビナープログラムのステータスについて {#understanding-webinar-program-statuses}

プログラムステータスは、イベントのメンバーとして人物がイベント内でたどる様々なイベントステータスを表します。 これらはチャネルタイプに関連付けられています。 Marketo には、**ウェビナー**&#x200B;というビルトインのチャネルタイプがあります。 ステータスは、バッチキャンペーンとトリガーキャンペーンの両方で使用できます。

人物は、プログラムのステータスを一方向に移行し、元のステータスに戻ることはありません。 例えば、ステータスが&#x200B;**Attended**&#x200B;の人は、**Registered**&#x200B;に戻ることができません。

次に、ウェビナーチャネルに関連するプログラムステータスの簡単な説明を示します。

>[!TIP]
>
>ステータスを手動で更新するには、**イベントアクション**&#x200B;ドロップダウンリストで「**ウェビナープロバイダーから更新**&#x200B;を」クリックします。

![](assets/image2015-12-17-13-3a52-3a39.png)

**プログラムに含まれていない** - このステータスを使用して、イベントからユーザを削除します。

**招待済み** - このステータスを使用して、イベントにユーザを追加します。

**承認待ち** - このステータスを使用して、確認メールの送信を保留します。 詳しくは、[ON24 イベント登録のアップデート](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/on24-event-registration-updates.md){target="_blank"}を参照してください。

**待機リスト** - このステータスを使用して、追加のシートが利用可能になるまでユーザーを待機させます。

**却下** - このステータスを使用して、ユーザのイベントへの登録を拒否します。

**登録済み** - ON24 統合を使用している場合、このステータスによりユーザが ON24 にプッシュされます。 ON24 がその人物が正常に登録されたと応答すると、その人物のステータスが更新されます。

**登録エラー** - このステータスは、ユーザーがイベントに登録しようとした際にエラーが発生したことを反映しています。

>[!NOTE]
>
>登録エラーが発生した場合は、プログラムの「メンバー」タブの「ステータス理由」列を確認して、その人物に関する追加情報を取得できます。 エラーが修正されたら、Marketo 内でユーザのプログラムステータスを手動で「登録済み」に変更できます。

**出席** - ウェビナーの終了時に、ON24 は出席者のリストを返します。 このステータスは Marketo に自動的に取り込まれます。

**オンデマンドで出席** - アーカイブバージョンのウェビナーに参加した人は、このステータスを受け取ります。

**欠席** - ウェビナーの終了時および ON24 から出席データを取り込むと、登録したが出席しなかった人のステータスが「欠席」にアップデートされます。 ON24 が最終的な出席情報を準備して Marketo で利用できるようにするには、30 分から 3 時間かかる場合があります。

>[!NOTE]
>
>Marketo が「欠席」ステータスを引き出すには、ユーザは *Marketo* で登録されている必要があります。 No On24 データフィードから取得された番組はキャプチャできません。

>[!MORELIKETHIS]
>
>[Marketo ON24 アダプターイベントについて](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-marketo-on24-adapter-events.md){target="_blank"}
