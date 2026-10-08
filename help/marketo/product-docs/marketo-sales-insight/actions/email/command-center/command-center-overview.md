---
description: セールスメールとタスクを管理するためのコマンドセンターについて説明します。 送信されたメールを表示し、タスクを割り当て、Sales Insightアクションでクイックアクションを使用します。
title: コマンドセンターの概要
exl-id: d7441f28-a432-4443-8eb8-ca6a685524ae
feature: Sales Insight Actions
TQID: 'https://experienceleague.adobe.com/Qyv0jDwHTbvZV3dG2ywoaFkEOunuhJN2yBbWRbdp1HI'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: 412786a7-b8da-5b9d-8c3f-2539a3faad9f
    internal-label: Sales Insight Actions
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '523'
ht-degree: 84%
---
# コマンドセンターの概要 {#command-center-overview}

[!UICONTROL コマンドセンター]は単一の統合ビューで、何も抜け落ちがないように確認しながら、次のステップを考え出すのに役立ちます。

## メールの管理 {#manage-emails}

[!UICONTROL コマンドセンター]のメールセクションでは、すべてのメールアクティビティを管理できます。 [!DNL Sales Connect] から送信されたメールを確認するためのメール送信ボックスと考えてください。 スケジュールされたメールの管理、メールに関心を寄せている人の確認、メールの配信に問題があるかどうかの確認などを行います。

![](assets/command-center-overview-1.png)

メールセクションでは、すべてのメールを俯瞰して、プライマリタブとサブタブを使用して組織を簡素化できます。プライマリタブとサブタブは、メールがステータスに基づいて自動的に保存されるフォルダーの役割を果たします。

<table>
 <tr>
  <th>プライマリ</th>
  <th>サブ</th>
  <th>説明</th>
 </tr>
 <tr>
  <th rowspan="2">[!UICONTROL 送信済み]</th>
  <td>[!UICONTROL 配信済み]</td>
  <td>受信者に配信されたメール。</td>
 </tr>
 <tr>
  <td>[!UICONTROL アーカイブ済み]</td>
  <td>メールのトラッキングを無効にするためにユーザーがアーカイブしたメール。</td>
 </tr>
 <tr>
  <th rowspan="3">[!UICONTROL 保留中]</th>
  <td>[!UICONTROL スケジュール済み]</td>
  <td>現在配信がスケジュールされているメール。 メールが送信されると、配信済みフォルダーに移動します。</td>
 </tr>
 <tr>
  <td>[!UICONTROL ドラフト]</td>
  <td>下書きとして保存されたメール。<br/>
  <strong>注意</strong>：下書きとして保存できるのは1通のメールのみです。 一括メール（「メールを選択して送信」と「メールをグループ化」）は下書きとして保存されません。</td>
 </tr>
 <tr>
  <td>[!UICONTROL 進行中]</td>
  <td>これは、送信モーション中にメールが処理される中間の状態を示します。 メールが処理中であるのは、わずかの間です。</td>
 </tr>
 <tr>
  <th rowspan="3">[!UICONTROL 未配信]</th>
  <td>[!UICONTROL 失敗]</td>
  <td>配信に失敗したメール。
</td>
 </tr>
 <tr>
  <td>[!UICONTROL バウンス済み]</td>
  <td>受信者のメールサーバーから却下されたメール。<br/>
  <strong> メモ </strong>：これは、レガシーのToutApp ユーザーであり、配信チャネルとしてMSC サーバーにアクセスできる場合にのみ検出されます。</td>
 </tr>
 <tr>
  <td>[!UICONTROL スパム]</td>
  <td>受信者によって手動でスパムとマークされたメール。<br/>
  <strong> メモ </strong>：これは、レガシーのToutApp ユーザーであり、配信チャネルとしてMSC サーバーにアクセスできる場合にのみ検出されます。</td>
 </tr>
</table>

## タスクの管理 {#manage-tasks}

タスクセクションは、タスクの管理と完了を一括して行える場所です。 タスクをシームレスに管理し、生産性を高め、最も関連性の高い項目に集中できます。

![](assets/command-center-overview-2.png)

## エンゲージした見込み客のフォローアップ {#follow-up-with-engaged-prospects}

作成ウィンドウまたはキャンペーンを使用して見込み客とのエンゲージメントを開始したら、詳細検索機能を使用して、最もエンゲージメントの高い見込み客を再度ターゲティングできます。

例えば、MSC のキャンペーンに 100 人を追加する場合、メールを閲覧してクリックしたが返信しなかった人を再度ターゲティングしたいと考えるでしょう。 そのためには、キャンペーンフィルターに加えて、表示ステータスおよびクリックステータスのアクティビティフィルターを利用して、再度ターゲティングする人のリストを特定します。

補足：詳細検索を保存すると、動的リストとして機能し、受信者がメールを表示またはクリックした時点で、エンゲージメント条件を満たすメールの受信者がリストに追加されます。

>[!MORELIKETHIS]
>
>* タスク
>* 詳細検索の概要
>* 「選択して送信」による一括メールの作成
