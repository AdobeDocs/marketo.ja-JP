---
description: リリースノート - 2024年1月 - Marketo ドキュメント - 製品ドキュメント
title: リリースノート - 2024年1月
feature: Release Information
exl-id: 64e85f6c-b746-46b6-ab51-5ad1817396b2
TQID: https://experienceleague.adobe.com/H-fad0HtKRnUzLN8mBkX-i7iUboD-RqMY8-AM5z-Bz8
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: b0bb9048-d951-48d8-8232-45cf248a7e27
  - id: b3b8a63f-51fc-40f6-a7d2-a31c5d49fb45
  - id: c5f60233-d5ea-4453-a799-0ad258b4d399
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
  - id: e2290edd-b061-4880-9d79-dee306cf5aa9
subfeature_v2:
  - id: cbccec41-b38b-4693-8acf-fed684dd06ba
topic_v2:
  - id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 840
ht-degree: 90%

---

# リリースノート：2024年1月 {#release-notes-jan-24}

以下に、2024年1月リリースに含まれるすべての機能を示します。 利用可能な機能については、お使いの Marketo Engage のエディションをご確認ください。

>[!AVAILABILITY]
>
>星印（![星印](assets/yellow-star.png)）で示す機能は有償オプションです。 詳しくは、Marketo Engage 担当営業にお問い合わせください。

## 標準リリースサイクルの機能 {#standard-release-cycle-features}

次の機能は標準リリースサイクルに該当し、リリースは **2024年1月12日（PT）**&#x200B;から開始し、その次の週から残りの機能が段階的にロールアウトされます。 リリースの機能と日付は変更される場合があります。 各機能のステータスについては、各機能の隣で確認してください。

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th style="width:65%">機能</th>
   <th style="width:10%">ステータス</th>
   <th style="width:25%">ドキュメント</th>
  </tr>
    <tr>
   <td><strong>インタラクティブウェビナーのオンデマンドウェビナー</strong>：オンデマンドウェビナーを使用すると、ウェビナーの録画を公開したり、その訪問数や視聴数を追跡したりできます。 これにより、ウェビナーに出席しなかった（欠席）が、詳細を知ることや録画を視聴することにまだ興味を持っている登録者を通じて、より多くのリードを獲得できます。</td>
   <td>リリース</td>
   <td><a href="/help/marketo/product-docs/demand-generation/events/interactive-webinars/on-demand-webinars.md" target="_blank">オンデマンドウェビナー</a></td>
  </tr>
   <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
    <tr>
   <td><strong>対話型ランディングページ</strong>：Dynamic Chat の対話型フローを Marketo Engage ランディングページに直接埋め込むことで、訪問者はフォームに入力したりチャットボットとやり取りしたりすることなく、Dynamic Chat を通じてミーティングをスケジュールできます。</td>
   <td><i>まもなくリリース</i></td>
   <td><i>まもなくリリース</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
    <tr>
   <td><strong>メールボットアクティビティのフィルタリング</strong>：ボットアクティビティ識別フィルタリングのアグレッシブを選択できるようにすることで、メールエンゲージメントのボットアクティビティのキャプチャを改善します。</td>
   <td>リリース</td>
   <td><a href="/help/marketo/product-docs/administration/email-setup/filtering-email-bot-activity.md" target="_blank">メールボットアクティビティのフィルタリング</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
   </tr>
    <tr>
   <td><strong>一括リード読み込み API の更新</strong>：ジョブ作成中に <b>ID</b> を <b>lookupField</b> として指定した場合の一括リード読み込み API の動作に小規模な調整を行いました。 指定した <b>ID</b> にリンクされた個人レコードが Marketo Engage データベースで見つからない場合、レコードが見つからないので、レコードの更新は行われません。 更新された動作には、応答内の <b>numOfRowsFailed</b> プロパティのカウントを増分し、このような場合に操作が失敗したことを通知することが含まれるようになりました。</td>
   <td>リリース</td>
   <td>該当なし</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
   </tr>
  <tr>
   <td><strong>インタラクティブウェビナーの共同主催者</strong>：インタラクティブウェビナーの「ウェビナー」チームセクションの共同主催者により、イベント作成者はインタラクティブウェビナープログラムに内部または外部のユーザを追加して、管理と配信の責任を共有できます。</td>
   <td>リリース</td>
   <td><a href="/help/marketo/product-docs/demand-generation/events/interactive-webinars/create-an-interactive-webinar.md#adding-a-webinar-team" target="_blank">ウェビナーチームの追加</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
    <tr>
   <td><strong>インタラクティブウェビナーでのユーザの削除</strong>：Marketo Engage 管理者は、インタラクティブウェビナーで特定のユーザを削除できるようになりました。</td>
   <td>リリース</td>
   <td>該当なし</td>
  </tr>
 </tbody>
</table>
<br/>

## アジャイルリリースの機能 {#agile-release-features}

以下の機能は、アジャイル形式に従い、標準リリース日前後の様々な日付にリリースされます。 各機能のステータスについては、各機能の隣で確認してください。

### セールスインサイトアクション {#sales-insight-actions}

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
   <td><strong>拡張可能な作成ウィンドウ</strong>：メールの作成ウィンドウでは、未使用のスペースが自動的に圧縮され、エディターのスペースが広く確保されるようになりました。 さらに、ウィンドウはポップアップしてさらに拡張できるので、ユーザはメールの編集に必要なだけのスペースを確保できます。</td>
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
   <td><strong>対話型フォームのチャットボット UI</strong>：Web サイト訪問者は対話型フローでライブチャットをリクエストできるようになりました。</td>
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
   <td><strong>チャットボットのフォントカラーオプション</strong>：チャットボット設定のフォントカラーをカスタマイズします。</td>
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
   <td><strong>ダイアログを繰り返すオプション</strong>：訪問者がダイアログの最後まで到達した後、ダイアログを最初から再開できるようになりました。</td>
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
   <td><strong>手動ライブチャットの終了</strong>：訪問者とエージェントの両方がライブチャットセッションを手動で終了できるようになりました。</td>
   <td>リリース</td>
   <td><a href="/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/agent-inbox.md#end-a-session" target="_blank">エージェントインボックス</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
    </tr>
    <tr>
   <td><strong>エージェントインボックスの最新の Marketo Engage アクティビティ</strong>：開封したメールや入力したフォームなどの最新の Marketo Engage アクティビティが、エージェントインボックスのリードに表示されます。</td>
   <td><i>まもなくリリース</i></td>
   <td><i>まもなくリリース</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
    <tr>
   <td><strong>条件付き分岐</strong>：訪問者の場所やライブエージェントの可用性など、事前定義済みの条件に基づいて、訪問者に様々な対話コンテンツを表示できるようになりました。</td>
   <td><i>まもなくリリース</i></td>
   <td><i>まもなくリリース</i></td>
  </tr>
 </tbody>
</table>
<br/>

## お知らせ {#announcements}

* **ワンクリックリスト登録解除の更新**：Gmail と Yahoo は、2024年2月1日（PT）に発効したいくつかの新しい送信者要件を実装しました。 [その概要と影響について説明します](https://nation.marketo.com/t5/employee-blogs/update-support-for-one-click-list-unsubscribe-for-marketo/ba-p/344514#M352){target="_blank"}。

* **リード APIの同期の更新**: [&#x200B; リード API](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Leads/operation/syncLeadUsingPOST){target="_blank"}の動作は、`unsubscribed` フィールドの更新に関して少し調整されました。 現在は、値として `null` を渡すと、`false` の値を渡すのと同じになります。

* **Marketo Engage Forms jQuery 1.x**:2024年1月のリリースでは、jQuery for Marketo Engage FormsをjQuery 3.xにアップデートします。 これは、古いバージョンのjQueryに依存するカスタムフォーム実装に影響を与える可能性があります。 詳しくは、[こちらを参照](https://nation.marketo.com/t5/product-blogs/marketo-engage-forms-amp-forms2-js-jquery-update/ba-p/341705){target="_blank"}してください。

* **SSO のみのユーザのメール検証**：SSO のみのユーザは自動的に検証され、アクセスできないメールアカウントの使用が許可されました。 1 月中旬以降、既存の SSO のみのユーザはすべて未検証になり、メールアカウントに送信されるリンクを通じてメールを再検証するように求められます。 今後、すべての新しい SSO のみのユーザはメールアドレスを検証する必要があります。

* 2024年1月[Marketo Engage リリースウェビナー](https://engage.marketo.com/2024_January_Release_Webinar_OnDemandPage.html){target="_blank"}をご覧ください。
