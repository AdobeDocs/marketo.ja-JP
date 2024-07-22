---
description: リリースノート - 2024年1月 - Marketo ドキュメント - 製品ドキュメント
title: リリースノート - 2024年1月
feature: Release Information
exl-id: 64e85f6c-b746-46b6-ab51-5ad1817396b2
source-git-commit: 2b610cc3486b745212b0b1f36018a83214d7ecd7
workflow-type: tm+mt
source-wordcount: '782'
ht-degree: 21%

---

# リリースノート：2024年1月 {#release-notes-jan-24}

以下に、2024 年 1 月リリースに含まれるすべての機能を示します。 機能の可用性についてはお使いの Marketo Engage のエディションをご確認ください。

>[!AVAILABILITY]
>
>星（![星](assets/yellow-star.png)）で示す機能は有償オプションです。詳しくは、Marketo Engage 担当営業にお問い合わせください。

## 標準リリースサイクルの機能 {#standard-release-cycle-features}

以下の機能は標準リリースサイクルに該当し、リリースは **2024年1月12日**（PT）から開始し、その次の週から残りの機能が段階的にロールアウトされます。リリースの機能と日付は変更される場合があります。各機能のステータスについては、各機能の隣で確認してください。

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:65%">機能</th> 
   <th style="width:10%">ステータス</th>
   <th style="width:25%">ドキュメント</th>
  </tr>
    <tr> 
   <td><strong> インタラクティブウェビナーのオンデマンドウェビナー </strong>：オンデマンドウェビナーでは、ウェビナー録画を公開したり、訪問回数/ウォッチを追跡したりできます。 これにより、ウェビナーに参加しなかったものの、詳細を見つけたり録画を視聴したりすることに関心のある登録者を通じて、より多くのリードを獲得できます。</td> 
   <td>出荷済み</td>
   <td><a href="/help/marketo/product-docs/demand-generation/events/interactive-webinars/on-demand-webinars.md" target="_blank">オンデマンドウェビナー</a></td>
  </tr>
   <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
    <tr> 
   <td><strong> 対話型ランディングページ </strong>:Dynamic Chatの対話型フローをMarketo Engageランディングページに直接埋め込むと、訪問者は、フォームに入力したりチャットボットとやり取りしたりしなくても、Dynamic Chatを通じてミーティングをスケジュールできます。</td> 
   <td><i>まもなくリリース</i></td>
   <td><i>まもなくリリース</i></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
    <tr> 
   <td><strong> メールボットアクティビティのフィルタリング </strong>：ボットアクティビティ識別フィルタリングのアグレッシブを選択できるようにすることで、メールエンゲージメントのボットアクティビティのキャプチャを改善します。</td> 
   <td>出荷済み</td>
   <td><a href="/help/marketo/product-docs/administration/email-setup/filtering-email-bot-activity.md" target="_blank">メールボットアクティビティのフィルター</a></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
   </tr>
    <tr> 
   <td><strong> リード一括読み込み API の更新 </strong>：ジョブ作成中に <b>id</b> が <b>lookupField</b> として指定された場合のリード一括読み込み API の動作に軽微な調整が加えられました。 指定された <b>id</b> にリンクされている人物レコードがMarketo Engageデータベースで見つからない場合、レコードが見つからないので、レコードは更新されません。 更新された動作には、応答内の <b>numOfRowsFailed</b> プロパティのカウントが増分され、このような場合に操作が失敗したことを示すようになりました。</td> 
   <td>リリース済み</td>
   <td>該当なし</td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
   </tr>
  <tr> 
   <td><strong> インタラクティブウェビナーのコホスト </strong>：インタラクティブウェビナーの「ウェビナーチーム」セクションのコホストを使用すると、イベント作成者は、内部または外部のユーザーをインタラクティブウェビナープログラムに追加して、管理と配信の責任を共有できます。</td> 
   <td>出荷済み</td>
   <td><a href="/help/marketo/product-docs/demand-generation/events/interactive-webinars/create-an-interactive-webinar.md#adding-a-webinar-team" target="_blank">ウェビナーチームの追加</a></td>
  </tr>
  <tr>
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
    <tr> 
   <td><strong> インタラクティブウェビナーでのユーザーの削除 </strong>:Marketo Engage管理者は、インタラクティブウェビナーで特定のユーザーを削除できるようになりました。</td> 
   <td>リリース済み</td>
   <td>該当なし</td>
  </tr>
 </tbody> 
</table>
<br/>

## アジャイルリリースの機能 {#agile-release-features}

以下のすべての機能は、アジャイル形式に従い、標準リリース日の前後の様々な日付にリリースされます。 各機能のステータスについては、各機能の隣で確認してください。

### Sales Insight Actions {#sales-insight-actions}

![（星印）](assets/yellow-star.png)

<table style="border: 0px">
 <tbody> 
  <tr> 
   <th style="width:65%">機能</th> 
   <th style="width:15%">ステータス</th>
   <th style="width:20%">ドキュメント</th>
  </tr> 
  </tr>
    <tr> 
   <td><strong> 展開可能なメール作成ウィンドウ </strong>：メール作成ウィンドウで未使用のスペースを自動的に圧縮できるようになり、エディターのスペースを広げることができます。 さらに、このウィンドウはポップアップ表示されてさらに拡大することができ、ユーザーはメールを編集するために必要なスペースをできる限り確保できます。</td> 
   <td><i>まもなくリリース</i></td>
   <td><i>まもなくリリース</i></td>
  </tr>
 </tbody> 
</table>
<br/>
  </tbody> 
</table>

### Dynamic Chat {#dynamic-chat}

<table style="border: 0px">
 <tbody> 
  <tr> 
   <th style="width:65%">機能</th> 
   <th style="width:15%">ステータス</th>
   <th style="width:20%">ドキュメント</th>
  </tr> 
  </tr>
    <tr> 
   <td><strong> 会話型Formsのチャットボット UI</strong>:web サイト訪問者は、会話型フローでライブチャットをリクエストできるようになりました。</td> 
   <td><i>まもなくリリース</i></td>
   <td><i>まもなくリリース</i></td>
  </tr>
   <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
   </tr>
    <tr> 
   <td><strong> チャットボットフォントカラーオプション </strong>：チャットボット設定のフォントカラーをカスタマイズします。</td> 
   <td><i>まもなくリリース</i></td>
   <td><i>まもなくリリース</i></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
   </tr>
    <tr> 
   <td><strong> ダイアログを繰り返すオプション </strong>：訪問者が終了した後、最初にダイアログを再開できるようになりました。</td> 
   <td><i>まもなくリリース</i></td>
   <td><i>まもなくリリース</i></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
    </tr>
    <tr> 
   <td><strong> 手動によるライブチャットの終了 </strong>：訪問者とエージェントの両方が、ライブチャットセッションを手動で終了できるようになりました。</td> 
   <td>出荷済み</td>
   <td><a href="/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/agent-inbox.md#end-a-session" target="_blank">エージェントのインボックス</a></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
    </tr>
    <tr> 
   <td><strong> エージェントインボックスの最近のMarketo Engageアクティビティ </strong>：開いたメールや記入したフォームなどの最近のMarketo Engageアクティビティが、エージェントインボックスのリードに表示されます。</td> 
   <td><i>まもなくリリース</i></td>
   <td><i>まもなくリリース</i></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
    <tr> 
   <td><strong> 条件付きブランチ </strong>：訪問者の場所やライブエージェントの可用性など、事前に定義された条件に基づいて、様々な会話コンテンツを訪問者に表示できるようになりました。</td> 
   <td><i>まもなくリリース</i></td>
   <td><i>まもなくリリース</i></td>
  </tr>
 </tbody> 
</table>
<br/>

## お知らせ {#announcements}

* **ワンクリックリスト – 登録解除の更新**:Gmail と Yahoo は、2024 年 2 月 1 日に有効になった、いくつかの新しい送信者要件を実装しました。 [ その概要と影響 ](https://nation.marketo.com/t5/employee-blogs/update-support-for-one-click-list-unsubscribe-for-marketo/ba-p/344514#M352){target="_blank"} を説明します。

* **リード API の更新を同期**: [ リード API を同期 ](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Leads/operation/syncLeadUsingPOST){target="_blank"} の動作が、「`unsubscribed`」フィールドの更新に関して若干調整されました。 現在は、`null` を値として渡すと、`false` の値を渡すのと同じになります。

* **Marketo EngageForms jQuery 1.x**: 2024 年 1 月のリリースで、Marketo EngageFormsの jQuery を jQuery 3.x に更新する予定です。これは、古いバージョンの jQuery に基づくカスタムフォーム実装に影響を与える可能性があります。 [詳しくは、こちらを参照してください](https://nation.marketo.com/t5/product-blogs/marketo-engage-forms-amp-forms2-js-jquery-update/ba-p/341705){target="_blank"}。

* **SSO のみのユーザー向けのメール検証**:SSO 自動で検証されるユーザーのみを対象とし、アクセスできないメールアカウントを使用できるようにしたものです。 1 月中旬以降、既存の SSO のみのユーザーは未検証になり、メールアカウントに送信するリンクからメールを再検証するように求められます。 すべての新しい SSO のみのユーザーは、今後、メールアドレスを検証する必要があります。

* [2024 年 1 月Marketo Engageリリースのウェビナー ](https://engage.marketo.com/2024_January_Release_Webinar_OnDemandPage.html){target="_blank"} をご覧ください。
