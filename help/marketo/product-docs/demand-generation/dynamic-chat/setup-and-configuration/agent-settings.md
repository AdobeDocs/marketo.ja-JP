---
description: Agent Settings - Marketo ドキュメント – 製品ドキュメント
title: エージェント設定
feature: Dynamic Chat
exl-id: a782ef9b-6a89-448a-8bd9-f127ceea3bf5
source-git-commit: 19f7a38a6a87bc66084e7e45f5bf49cd0d29c3cd
workflow-type: tm+mt
source-wordcount: '543'
ht-degree: 24%

---

# エージェント設定 {#agent-settings}

カレンダーを設定して、会議/ライブチャットの利用を設定します。

>[!PREREQUISITES]
>
>エージェントに適切な [ 権限 ](/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/permissions.md){target="_blank"} が付与されていることを確認します。

![](assets/agent-settings-1.png)

## カレンダーの接続 {#connect-calendar}

[ 予定表の構成 ] タブで、チャットボットの予定スケジュールで使用する Outlook または Gmail の予定表を接続します。

![](assets/agent-settings-2.png)

ユーザのカレンダーが動的チャットに接続されると、そのユーザはキューに追加され、web サイトの訪問者が予定をスケジュールする際に使用できるようになります。

>[!NOTE]
>
>1 ユーザにつき 1 つのカレンダーを接続できます。複数のカレンダーで会議を受け取る場合は、複数のユーザを追加し、各ユーザにカレンダーを連携させる必要があります。

また、カレンダーに予定をスケジュールするときに訪問者に送信される、招待の本文をカスタマイズすることもできます。下部のチェックボックスを選択して、「Google Meet」リンクまたは「Microsoft Teams」リンクを含めることもできます（接続されたカレンダーに応じて異なります）。

![](assets/agent-settings-3.png)

>[!TIP]
>
>トークンアイコン（波括弧）を使用して、ユーザ属性または会社属性を使用して会議予約確認メールをパーソナライズします。

### 権限 {#permissions}

Outlook でを設定すると、Dynamic Chatに対して次の権限が付与されます。

* カレンダーへのフルアクセス
* ログインしてプロファイルを読む
* アクセス権を付与したデータへのアクセスを維持する
* メールボックスの設定を読み取る

Googleを使用して設定すると、Dynamic Chatに対して次の権限が付与されます。

* カレンダーを作成、変更または削除します
* 個々のカレンダーイベントの更新
* イベントを表示できるユーザーなど、設定を変更します
* カレンダーを共有するユーザーを変更する
* 名前、メールアドレス、言語設定、プロフィール画像へのアクセス

## 会議予約の空き時間 {#meeting-booking-availability}

会議の予約を受け取るためのタイムゾーンおよび時刻/曜日の空き時間を設定します。

![](assets/agent-settings-4.png)

<table> 
 <tbody> 
  <tr> 
   <td><b>ミーティング期間</b></td>
   <td>訪問者が使用可能な会議スロットに表示される時間の長さを決定します。</td>
  </tr> 
  <tr> 
   <td><b>ミーティング間のバッファ時間</b></td>
   <td>会議後にバッファーとして設定した時間。 30 分に設定すると、予定表で予定されている会議の終了から 30 分後まで、誰も会議を予約できません。</td>
  </tr>
 </tbody> 
</table>

>[!TIP]
>
>右側の「**+**」記号をクリックして、同じ日の複数の時間ブロック（例：8a～12p _および_ 1p～5p）を選択できます。

## ライブチャットの利用 {#live-chat-availability}

タイムゾーンとライブチャットを受信できる時刻/曜日を設定します。

![](assets/agent-settings-5.png)

アプリにログインしている場合は、受信チャットのアプリ内通知が届きます。 ログインしていない場合は、ブラウザー通知が表示されます（既に [ 設定 ](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/agent-inbox.md#live-chat-notifications){target="_blank"} している場合）。

>[!IMPORTANT]
>
>エージェントインボックスの [ 利用可能 ](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/agent-inbox.md#availability-toggle){target="_blank"} 切替スイッチ **は、「ライブチャットの利用可能」タブで入力した** を上書きします。 したがって、1p～5p から利用可能とスケジュールされていても、3p で素早く休憩する必要がある場合は、エージェント設定を変更する必要はありません。 可用性の切り替えステータスは、手動で変更するか、可用性の次のブロックに達するまで保持されます。

>[!TIP]
>
>右側の「**+**」記号をクリックして、同じ日の複数の時間ブロック（例：8a～12p _および_ 1p～5p）を選択できます。

## エージェント プロファイルの写真

エージェントは独自のプロファイル写真をアップロードできますが、その操作はDynamic Chatでは実行されません。 `account.adobe.com/profile` に移動する必要があります。 詳しくは、[ アカウントプロファイルを更新 ](https://helpx.adobe.com/jp/manage-account/using/edit-adobe-account-personal-profile.html) を参照してください。

>[!NOTE]
>
>`experience.adobe.com` に示すプロファイル画像はサポートされて **ません**。
