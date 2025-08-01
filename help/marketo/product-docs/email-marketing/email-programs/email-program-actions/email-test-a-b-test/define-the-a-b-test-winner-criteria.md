---
unique-page-id: 2359545
description: A/B テストの勝者条件の定義 - Marketo ドキュメント - 製品ドキュメント
title: A/B テストの勝者条件の定義
exl-id: be8a0887-70f4-4667-93a6-d982a16cdfdb
feature: Email Programs, A/B Testing
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '426'
ht-degree: 83%

---

# A/B テストの勝者条件の定義 {#define-the-a-b-test-winner-criteria}

メールプログラムに [A/B テストを追加](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/add-an-a-b-test.md){target="_blank"}する際に、[A/B テストのスケジュール設定](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/schedule-the-a-b-test.md){target="_blank"}テストタイプを選択し、勝者の条件を定義する必要があります。どのメールが優先されるかを決定する方法を次に示します。

>[!PREREQUISITES]
>
>[A/B テストの追加](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/add-an-a-b-test.md){target="_blank"}

## 勝者の条件 {#winner-criteria}

1. デフォルトの&#x200B;**[!UICONTROL 勝者の条件]**&#x200B;オプションが最初に表示されます。

   ![](assets/image2014-9-12-15-3a51-3a3.png)

   <table>
   <tr>
   <td><b>[!UICONTROL 開封数 &#x200B;]</b></td>
   <td>メールに画像がダウンロードされると、開封が登録されます。画像を含めていなくても、デフォルトで Marketo がすべての HTML メールに 1 つのトラッキングピクセルを挿入します。</td>
   </tr>
   <tr>
   <td><b>[!UICONTROL クリック数 &#x200B;]</b></td>
   <td>デフォルトでは、メール内のリンクにはトラッキング情報が埋め込まれており、誰がどのリンクをクリックしたか、リンクが合計で何回クリックされたかなどを確認できます。</td>
   </tr>
   <tr>
   <td><b>[!UICONTROL クリックして開く &#x200B;] %</b></td>
   <td>開封され、メール内のリンクがクリックされたメールの割合。これは、ユニーククリック数をユニーク開封数で割り、100 倍してパーセンテージとして表示することで、メールの関連性とコンテキストを測定します。</td>
   </tr>
   <tr>
   <td><b>[!UICONTROL エンゲージメントスコア &#x200B;]</b></td>
   <td><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/drip-nurturing/reports-and-notifications/understanding-the-engagement-score.html" target="_blank">エンゲージメントスコア</a>は、コンテンツの効果を判断するのに役立ちます。</td>
   </tr>
   </table>

   >[!TIP]
   >
   >「エンゲージメントスコア」を選択した場合、テストは 24 時間以上実行する必要があります。[エンゲージメントスコア](/help/marketo/product-docs/email-marketing/drip-nurturing/reports-and-notifications/understanding-the-engagement-score.md){target="_blank"}について学びます。

1. また、「**[!UICONTROL カスタムコンバージョン]**」を選択し、「**[!UICONTROL 編集]** をクリックして、条件をカスタマイズすることもできます。

   ![](assets/image2014-9-12-15-3a51-3a53.png)

   >[!NOTE]
   >
   >カスタムコンバージョンでは、トリガーとフィルターを使用して、任意のイベントをコンバージョンとして設定できます。

1. ウィンドウがポップ表示されます。任意のトリガーを見つけ、キャンバスにドラッグします。

   ![](assets/image2014-9-12-15-3a52-3a18.png)

1. トリガーを定義します。

   ![](assets/image2014-9-12-15-3a53-3a11.png)

   >[!IMPORTANT]
   >
   >Marketoでは、このメールプログラムからメールを送信されたユーザーに対してのみトリガー/フィルターを許可するので、「送信済みのメール」フィルターを追加する必要はありません。 さらに、メール関連のトリガーやフィルターを使用する場合は、演算子として「is any」を使用します。

1. 「**[!UICONTROL 閉じる]**」をクリックします。

   ![](assets/image2014-9-12-15-3a53-3a36.png)

   完成です。次に、勝者の決定方法を決めます。

## 勝者の発表 {#declare-winner}

1. 2 つの使用可能なオプションの 1 つを選択します。

   ![](assets/image2014-9-12-15-3a53-3a44.png)

   >[!NOTE]
   >
   >**日時** A/B テストをおこなう場合、選択できるのは&#x200B;**[!UICONTROL 手動]**&#x200B;のみです。

   A/B テストが終了すると、スケジュールされた時刻に勝者のメールが自動的に送信されるようにできます。または、結果を確認して、どのメールを送信するかを決定できます。

1. 「自動」はすばらしいもので、デフォルトのオプションになっています。「**[!UICONTROL 次へ]**」をクリックします。

   ![](assets/image2014-9-12-15-3a54-3a35.png)

   >[!TIP]
   >
   >「**[!UICONTROL 手動]**」を選択すると、テストが送信され、勝者の発表を待機します。結果のレポートが届きます。

完璧です。次に、[A/B テストをスケジュール](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/schedule-the-a-b-test.md){target="_blank"}します。
