---
unique-page-id: 10096679
description: ON24 イベント統合の例 - Marketo ドキュメント - 製品ドキュメント
title: ON24 イベント統合の例
exl-id: 9d34d1bf-1ff8-4b26-906e-4a6bb9d5f3f6
feature: Events
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '385'
ht-degree: 90%

---

# ON24 イベント統合の例 {#example-on-event-integration}

以下に、キャンペーンを含む ON24 ウェビナーのサンプルイベントを示します。イベントを作成する場合は、キャンペーンを実行する前に必ずテストしてください。

## マーケティングアクティビティでの新しいイベントの作成 {#create-a-new-event-in-marketing-activities}

1. **[!UICONTROL 新規]**／**[!UICONTROL 新規プログラム]**&#x200B;を選択します。

   ![](assets/image2015-12-22-15-3a35-3a15.png)

1. イベントを格納する&#x200B;**[!UICONTROL キャンペーンフォルダー]**&#x200B;を選択します。

   ![](assets/image2015-12-22-15-3a39-3a51.png)

1. イベントの&#x200B;**[!UICONTROL 名前]**&#x200B;を入力します。

   ![](assets/image2015-12-22-15-3a43-3a4.png)

1. **[!UICONTROL プログラムタイプイベント]**&#x200B;として&#x200B;**[!UICONTROL イベント]**&#x200B;を選択します。

   ![](assets/image2015-12-22-15-3a44-3a41.png)

1. イベントの&#x200B;**[!UICONTROL チャネル]**&#x200B;として&#x200B;**[!UICONTROL ウェビナー]**&#x200B;を選択します。

   ![](assets/image2015-12-22-15-3a46-3a34.png)

1. 「**[!UICONTROL 作成]**」をクリックします。

   ![](assets/image2015-12-22-15-3a48-3a20.png)

## 招待（バッチキャンペーン）  {#invite-batch-campaign}

* **スマートリスト** - イベントに招待するユーザを定義します。
* **フロー**

   * メールを送信 - これがローカルアセットの電子メールである場合、命名規則「EventName.EmailName」が適用されます。グローバルメールも使用できます。
   * 進行状況のステータスの変更 - ウェビナー／招待済みに設定します。

* **スケジュール** - 招待を送信する日付を設定します。

## 登録／確認（トリガーキャンペーン） {#registration-confirmation-trigger-campaign}

* **スマートリスト**

   * **[!UICONTROL フォームへの記入]**&#x200B;に基づいてキャンペーンをトリガーします。特にフォームが複数のランディングページで使用される場合は、「**[!UICONTROL 制約を追加]**」を使用して、フォームが存在するランディングページを必ず含めてください。

>[!CAUTION]
>
>Marketo フォームを使用してイベントに担当者を登録するか、適切な API 統合による Marketo 以外のフォームを使用して Marketo に登録データをプッシュする必要があります。これは、[!UICONTROL &#x200B; イベントパートナー &#x200B;] 統合を成功させるうえで非常に重要です。 **注意**:Marketo以外のランディングページでMarketo フォームを使用している場合、トリガーは **[!UICONTROL フォーム名]** で [!UICONTROL &#x200B; フォームに入力 &#x200B;] されます。

![](assets/image2015-12-22-15-3a50-3a22.png)

* **フロー**

   * **進行状況のステータスの変更** - ウェビナー／登録済みに設定します。**注意**：このフローステップは、子キャンペーンを設定する際に必要です。担当者の進行状態ステータスが「**登録済み**」に変更されると、Marketo は登録情報を ON24 にプッシュします。

   * **メールを送信** - 確認メール（登録解除済みのユーザが引き続きメールを受け取れるように&#x200B;**オペレーショナル**&#x200B;に設定）。

![](assets/image2015-12-22-15-3a52-3a9.png)

**メモ。**：登録エラーが発生した場合、その担当者には確認メールは送信されません。

## リマインダー（バッチキャンペーン） {#reminder-batch-campaign}

* **スマートリスト** - **プログラムのメンバー**&#x200B;を使用してフィルターし、ステータスを&#x200B;**登録済み**&#x200B;に設定。

* **フロー** - 電子メールの送信（リマインダー電子メール）。

**メモ**：同様のキャンペーンを使用して、招待されたがまだ登録されていないユーザに&#x200B;*異なる*&#x200B;フォローアップメールを送信するようにもできます。

## フォローアップキャンペーン（バッチキャンペーンまたはトリガーキャンペーン） {#follow-up-campaign-batch-or-trigger-campaign}

* **スマートリスト** - プログラムステータスの変化に基づくトリガー

![](assets/image2015-12-22-15-3a57-3a25.png)

* **フロー** - メールを送信します。選択肢を使用して、プログラムのステータスに応じて異なるメールを送信します。

![](assets/ten.png)

>[!MORELIKETHIS]
>
>[Marketo ON24 アダプターイベントについて](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-marketo-on24-adapter-events.md){target="_blank"}
