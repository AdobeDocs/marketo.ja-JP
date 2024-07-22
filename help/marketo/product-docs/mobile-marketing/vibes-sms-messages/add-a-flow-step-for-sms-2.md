---
description: SMS のフローステップの追加 - Marketo ドキュメント - 製品ドキュメント
title: SMS のフローステップの追加
hide: true
hidefromtoc: true
feature: Mobile Marketing
source-git-commit: fee2d692acd8d54f2e308e2d5edc9876d13d5a4d
workflow-type: tm+mt
source-wordcount: '377'
ht-degree: 43%

---

# SMS のフローステップの追加 {#add-a-flow-step-for-sms}

Marketo Engageには、SMS スマートキャンペーンで使用できる 3 つのフローステップがあります。

<table>
<tbody>
  <tr>
    <td style="width:25%">SMS メッセージの送信</td>
    <td>このフローアクションは、オプトインした Vibes 購読リストを購読しているMarketo スマートリストのユーザーにメッセージを送信します。 購読プロセスは開始されません。 <a href="/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/send-a-vibes-sms-message.md">詳細情報</a></td>
  </tr>

<tr>
    <td style="width:25%">Vibes リストに配信登録</td>
    <td>このフローアクションは、ユーザーが選択した Vibes 獲得キャンペーンを通じて SMS 購読プロセスを開始します。 次に、Vibes が確認メッセージを送信し、受信者は 24 時間以内に「Y」と返信してオプトインを確認する必要があります。 ユーザーがオプトインすると、関連付けられた Vibes サブスクリプションリストのメンバーになります。</td>
  </tr>
  <tr>
    <td style="width:25%">Vibes リストから配信停止</td>
    <td>このフローアクションは、オプトインした Vibes 購読リストから各ユーザーを購読解除します。 ユーザーがコードに「STOP」と入力すると、ユーザーのユーザーレコードが更新され、Vibes サブスクリプションリストに登録されなくなったことを反映します。</td>
  </tr>
  </tbody>
</table>

>[!NOTE]
>
>SMS メッセージを送信する場合：
>
>* Marketo は電話番号によって重複排除をおこないます。したがって、複数のユーザーが同じ電話番号を持っている場合、1 つの Vibes サブスクリプションリストにのみメンバーであれば、1 人のユーザーのみがメッセージを受け取ります。 重複排除は、Marketo プログラムレベルではなく、Vibes サブスクリプションリストレベルで行われます。
>* メッセージはブロックリストに登録されたリードやマーケティングが中断されたリードには送信されません。

フローステップの設定に関する一般的な情報については、[スマートキャンペーンにフローステップを追加する](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md)を参照してください。

SMS を使用する際の基本事項を以下に示します。

1. My Marketo で、**マーケティング活動**&#x200B;をクリックします。

   ![](assets/add-a-flow-step-for-sms-1.png)

1. SMS フローを追加するスマートキャンペーンを見つけて選択します。

   スクリーンショット

1. 「スマートリスト」タブで、目的のトリガー（例：「入力済みフォーム」）を選択します。

   スクリーンショット

1. 「**フロー**」タブで、フローステップ上をドラッグします（例：**SMS メッセージを送信**）。 「SMS メッセージ」と「Vibes」リストをドロップダウンから選択します。

   ![](assets/send-sms-message-hands.jpg)

   >[!NOTE]
   >
   >Vibes リストセレクターは、スマートリストで既に識別されているオーディエンスに対する追加のフィルターとして機能し、Vibes リストに属するリードのみをターゲットにします。
   >
   >**Vibes リストに購読**&#x200B;および **Vibes リストから登録解除**&#x200B;フローには、異なる要件があります。**購読**&#x200B;の場合、Vibes リストと Vibes 獲得キャンペーンを選択する必要があります。**登録解除**&#x200B;の場合、Vibes リストのみが必要です。
