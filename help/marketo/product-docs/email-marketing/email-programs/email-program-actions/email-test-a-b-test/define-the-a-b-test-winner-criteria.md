---
unique-page-id: 2359545
description: A/B テストの勝者条件の定義 - Marketo ドキュメント - 製品ドキュメント
title: A/B テストの勝者条件の定義
exl-id: be8a0887-70f4-4667-93a6-d982a16cdfdb
feature: Email Programs, A/B Testing
source-git-commit: c80d25aeafe2314fcff1d99359ff146c88acad06
workflow-type: tm+mt
source-wordcount: '432'
ht-degree: 96%

---

# A/B テストの勝者条件の定義 {#define-the-a-b-test-winner-criteria}

メールプログラムに [A/B テストを追加](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/add-an-a-b-test.md){target="_blank"}する際に、[A/B テストのスケジュール設定](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/schedule-the-a-b-test.md){target="_blank"}テストタイプを選択し、勝者の条件を定義する必要があります。どのメールが優先されるかを決定する方法を次に示します。

>[!PREREQUISITES]
>
>[A/B テストの追加](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/add-an-a-b-test.md){target="_blank"}

## 勝者の条件 {#winner-criteria}

1. デフォルトの&#x200B;**[!UICONTROL 勝者の条件]**&#x200B;オプションが最初に表示されます。

   ![](assets/define-the-a-b-test-winner-criteria-1.png)

   <table>
   <tr>
   <td><b>[!UICONTROL 開封数]</b></td>
   <td>メールに画像がダウンロードされると、開封が登録されます。画像を含めていなくても、デフォルトで Marketo がすべての HTML メールに 1 つのトラッキングピクセルを挿入します。</td>
   </tr>
   <tr>
   <td><b>[!UICONTROL クリック数]</b></td>
   <td>デフォルトでは、メール内のリンクにはトラッキング情報が埋め込まれており、誰がどのリンクをクリックしたか、リンクが合計で何回クリックされたかなどを確認できます。</td>
   </tr>
   <tr>
   <td><b>[!UICONTROL クリック/開封率] %</b></td>
   <td>開封され、メール内のリンクがクリックされたメールの割合。これは、ユニーククリック数をユニーク開封数で割り、100 倍してパーセンテージとして表示することで、メールの関連性とコンテキストを測定します。</td>
   </tr>
   <tr>
   <td><b>[!UICONTROL エンゲージメントスコア]</b></td>
   <td><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/drip-nurturing/reports-and-notifications/understanding-the-engagement-score.html?lang=ja" target="_blank">エンゲージメントスコア</a>は、コンテンツの効果を判断するのに役立ちます。</td>
   </tr>
   </table>

   >[!TIP]
   >
   >「エンゲージメントスコア」を選択した場合、テストは 24 時間以上実行する必要があります。[エンゲージメントスコア](/help/marketo/product-docs/email-marketing/drip-nurturing/reports-and-notifications/understanding-the-engagement-score.md){target="_blank"}について学びます。

1. また、「**[!UICONTROL カスタムコンバージョン]**」を選択して「**[!UICONTROL 編集]**」をクリックすることで、条件をカスタマイズすることもできます。

   ![](assets/define-the-a-b-test-winner-criteria-2.png)

   >[!NOTE]
   >
   >カスタムコンバージョンでは、トリガーとフィルターを使用して、任意のイベントをコンバージョンとして設定できます。

1. ウィンドウが開きます。 任意のトリガーを見つけ、キャンバスにドラッグします。

   ![](assets/define-the-a-b-test-winner-criteria-3.png)

1. トリガーを定義します。

   ![](assets/define-the-a-b-test-winner-criteria-4.png)

   >[!IMPORTANT]
   >
   >Marketo では、このメールプログラムからメールが送信された人物に対してのみトリガー／フィルターが許可されるので、「メールが送信されました」フィルターを追加する必要はありません。さらに、メール関連のトリガー／フィルターを使用する場合は、演算子として「が次のいずれかである」が使用されます。

1. 開いた新しいウィンドウ（またはタブ）を閉じます。 スマート・リストは自動保存されます。

次に、勝者の決定方法を決めます。

## 勝者の発表 {#declare-winner}

1. 2 つの使用可能なオプションの 1 つを選択します。

   ![](assets/define-the-a-b-test-winner-criteria-5.png)

   >[!NOTE]
   >
   >**日時** A/B テストをおこなう場合、選択できるのは&#x200B;**[!UICONTROL 手動]**&#x200B;のみです。

   A/B テストが終了すると、スケジュールされた時刻に勝者のメールが自動的に送信されるようにできます。または、結果を確認して、どのメールを送信するかを決定できます。

1. 「自動」はすばらしいもので、デフォルトのオプションになっています。「**[!UICONTROL 次へ]**」をクリックします。

   ![](assets/define-the-a-b-test-winner-criteria-6.png)

   >[!TIP]
   >
   >「**[!UICONTROL 手動]**」を選択すると、テストが送信され、勝者の発表を待機します。結果のレポートが届きます。

次に、[A/B テストをスケジュール](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/schedule-the-a-b-test.md){target="_blank"}します。
