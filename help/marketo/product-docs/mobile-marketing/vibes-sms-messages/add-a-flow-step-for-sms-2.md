---
description: SMS のフローステップの追加 - Marketo ドキュメント - 製品ドキュメント
title: SMS のフローステップの追加
hide: true
hidefromtoc: true
feature: Mobile Marketing
source-git-commit: cf4dcb6a316eba631ccb73a991c09e83c80b82ca
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
    <td>このフローアクションは、オプトインした Vibes サブスクリプションリストに登録されているMarketoスマートリストの担当者にメッセージを送信します。 購読手続きは開始されません。 <a href="/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/send-a-vibes-sms-message.md">詳細情報</a></td>
  </tr>

<tr>
    <td style="width:25%">Vibes リストに登録</td>
    <td>このフローアクションは、ユーザーが選択した Vibes 獲得キャンペーンを介して SMS 購読プロセスを開始します。 Vibes が確認メッセージを送信し、受信者がオプトインを確認するには、24 時間以内に「Y」と返信する必要があります。 ユーザーがオプトインすると、関連付けられた Vibes 配信登録リストのメンバーになります。</td>
  </tr>
  <tr>
    <td style="width:25%">Vibes リストから登録解除</td>
    <td>このフローアクションは、オプトインした Vibes 配信登録リストから各顧客を配信停止にします。 ユーザーがコードに「STOP」と入力すると、ユーザーレコードが更新され、Vibes 配信登録リストのメンバーでなくなったことが反映されます。</td>
  </tr>
  </tbody>
</table>

>[!NOTE]
>
>SMS メッセージを送信する場合：
>
>* Marketo は電話番号によって重複排除をおこないます。したがって、複数の人が同じ電話番号を持っている場合、1 人の人だけがメッセージを受け取ります（1 人の Vibes 配信登録リストのメンバーの場合）。 重複排除は、Marketoプログラムレベルではなく、Vibes 購読リストレベルでおこなわれます。
>* メッセージはブロックリストに登録されたリードやマーケティングが中断されたリードには送信されません。

フローステップの設定に関する一般的な情報については、[スマートキャンペーンにフローステップを追加する](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md)を参照してください。

SMS を使用する際の基本事項を以下に示します。

1. My Marketo で、**マーケティング活動**&#x200B;をクリックします。

   ![](assets/add-a-flow-step-for-sms-1.png)

1. SMS フローを追加するスマートキャンペーンを見つけて選択します。

   スクリーンショット

1. 「スマートリスト」タブで、目的のトリガー（「入力済みフォーム」など）を選択します。

   スクリーンショット

1. Adobe Analytics の **流量** タブで、フローステップ ( 例： **SMS メッセージの送信**) をクリックします。 「SMS メッセージ」と「Vibes」リストをドロップダウンから選択します。

   ![](assets/send-sms-message-hands.jpg)

   >[!NOTE]
   >
   >Vibes リストセレクターは、スマートリストで既に識別されているオーディエンスに対する追加のフィルターとして機能し、Vibes リストに属するリードのみをターゲットにします。
   >
   >**Vibes リストに購読**&#x200B;および **Vibes リストから登録解除**&#x200B;フローには、異なる要件があります。**購読**&#x200B;の場合、Vibes リストと Vibes 獲得キャンペーンを選択する必要があります。**登録解除**&#x200B;の場合、Vibes リストのみが必要です。
