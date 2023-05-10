---
description: ユーザーとライセンスの管理 — Marketoドキュメント — 製品ドキュメント
title: ユーザーとライセンスの管理
hide: true
hidefromtoc: true
exl-id: 1fee628b-e9f3-46ab-b993-f2d09fe5e183
source-git-commit: 093af2946aa0279aff20d4388312fa7630e693a2
workflow-type: tm+mt
source-wordcount: '412'
ht-degree: 8%

---

# ユーザーとライセンスの管理 {#user-and-license-management}

ユーザーの追加と削除の方法、および現在のライセンスの表示について説明します。

## ユーザの追加 {#add-a-user}

1. 「**管理者**」領域に移動します。

   ![](assets/user-and-license-management-1.png)

1. クリック **インタラクティブ Web セミナー**.

   ![](assets/user-and-license-management-2.png)

1. クリック **ユーザーの追加/削除**.

   ![](assets/user-and-license-management-3.png)

1. 利用可能なユーザードロップダウンをクリックし、追加するユーザーを選択して、 **OK**.

   ![](assets/user-and-license-management-4.png)

## ユーザの削除 {#remove-a-user}

1. 「**管理者**」領域に移動します。

   ![](assets/user-and-license-management-5.png)

1. クリック **インタラクティブ Web セミナー**.

   ![](assets/user-and-license-management-6.png)

1. クリック **ユーザーの追加/削除**.

   ![](assets/user-and-license-management-7.png)

1. 削除するユーザーをハイライトし、キーボードの Delete キーを押します。 終了したら「**OK**」をクリックします。

   ![](assets/user-and-license-management-8.png)

## ライセンスの使用状況 {#license-usage}

インタラクティブウェビナーには、Adobe Connectイベントを作成するための特定のライセンスが用意されています。 ライセンスが追加されるたびに、新しいライセンス使用状況ボックスが表示されます。 Marketo管理者は、次の手順に従ってライセンスを表示（編集ではなく）できます。 追加のライセンスを取得するには、Adobeアカウントチーム（担当のアカウントマネージャー）にお問い合わせください。

1. 「**管理者**」領域に移動します。

   ![](assets/user-and-license-management-9.png)

1. クリック **インタラクティブ Web セミナー**.

   ![](assets/user-and-license-management-10.png)

1. 下にスクロールしてライセンス使用状況カードを表示します。

   ![](assets/user-and-license-management-11.png)

<table> 
  <tr> 
   <td><b>開始日</b></td>
   <td>ライセンスが開始される日付。</td>
  </tr>
  <tr> 
   <td><b>有効期限</b></td>
   <td>ライセンスの有効期限日。</td>
  </tr>
  <tr> 
   <td><b>タイプ</b></td>
   <td>購入したライセンスのタイプ。 次の 3 つのタイプを使用できます。共有イベントライセンス、共有ルームライセンス、追加のストレージライセンス。</td>
  </tr>
  <tr> 
   <td><b>イベントの処理能力</b></td>
   <td>イベントに対応できる最大参加者数。</td>
  </tr>
  <tr> 
   <td><b>合計イベント数</b></td>
   <td>このライセンスでプロビジョニングされたイベントの合計数です。</td>
  </tr>
  <tr> 
   <td><b>消費されたイベント</b></td>
   <td>完了したイベントの合計数。</td>
  </tr>
  <tr> 
   <td><b>ストレージ容量</b></td>
   <td>記録、関連資料、hero images、ドキュメント、その他のアセットの保存に使用できるストレージの量。</td>
  </tr>
  </tbody>
</table>

**注意事項**

* 「Additional Storage License」というタイプの場合は、ストレージが提供されるので、すべてのフィールドに値が表示されます _indes_ ストレージ容量は、単に「 — 」と表示されます。

* 「Shared Room License」には無制限のイベントがあり、「Additional Storage License」にはストレージが提供されるだけなので、これらのライセンスの「Total Events」フィールドは単に「 — 」と表示されます。

* イベントが作成されるたびに、それぞれのライセンスから「消費済み」としてカウントされます（Shared Room ライセンスの場合を除く）。 同じ容量の「共有イベントライセンス」と「共有ルームライセンス」の両方がある場合、「共有イベントライセンス」が優先されます。 イベントが配信されておらず、予定時間より前にイベントプログラムが削除された場合、消費済みイベントからイベントを引くことで、イベント数が補充されます。

* ライセンスを消費すると、そのタイルは「管理者」セクションのインタラクティブウェビナー画面に残り、「合計イベント数」と「消費されたイベント数」の値が同じになります。 ライセンスの有効期限が切れた場合にのみ、ライセンスは画面から削除されます。
