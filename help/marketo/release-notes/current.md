---
description: 最新のリリースノート - Marketo ドキュメント - 製品ドキュメント
title: 最新のリリースノート
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
feature: Release Information
TQID: 'https://experienceleague.adobe.com/QJFy7PeGXlvS3jcJGcZJROlc8c1UvphO-TOOwPUQeX8'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: b0bb9048-d951-48d8-8232-45cf248a7e27
    internal-label: Forms
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
    internal-label: Integrations
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
    internal-label: Administration
  - id: f71e690b-4480-4b67-9ef5-88f42f9cdfdb
    internal-label: Resources
  - id: f82558ea-6af5-44eb-a424-5b3389abb0a3
    internal-label: Templates
subfeature_v2:
  - id: c942e9f6-ed06-481a-abdd-1195363d1452
    internal-label: Dynamic Chat
  - id: af97ce94-35fa-4fa9-b85a-46b752ac4028
    internal-label: Release information
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 29aa413a7346a79906f4021dedc79e8e48170c69
workflow-type: tm+mt
source-wordcount: '472'
ht-degree: 15%
---
# リリースノート：2026年10月 {#release-notes-oct-26}

以下では、2026年10月リリースに含まれるすべての機能について説明します。 利用可能な機能については、お使いの Adobe Marketo Engage のエディションをご確認ください。

Adobe Dynamic Chat 専用のリリースノートについて詳しくは、[こちらを参照](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}してください。

## 標準リリースサイクルの機能 {#standard-release-cycle-features}

以下の機能は標準リリースサイクルに該当し、2026年10月23日（PT）にリリースが開始され、残りの機能は今後数週間にわたって段階的にロールアウトされます。 **&#x200B;**&#x200B;リリースされる機能と日付は変更される場合があります。 各機能のステータスは、その機能の横に表示されている情報を確認してください。

<table style="table-layout:auto">
 <tbody>
 <tr>
   <th style="width:65%">機能</th>
   <th style="width:10%">ステータス</th>
   <th style="width:25%">ドキュメント</th>
  </tr>
  <tr>
   <td><strong> キャンペーンスキルの計画</strong>: CX Enterprise Coworker for Marketo Engageで、キャンペーン概要を包括的なMarketo Engage プログラム設定ドキュメントに変換できるようになりました。 このドキュメントには、フォルダー構造、スマートキャンペーン、メール設定、トークン、QA チェックリストが含まれています。 これにより、キャンペーンをより迅速に立ち上げ、プログラムの設定を標準化できます。 スキルはマークダウンで設定可能です。</td>
   <td><i>近日リリース予定</i></td>
   <td><i>近日リリース予定</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>呼び出し可能なエージェント </strong>: スマートキャンペーンのフローステップとして実行し、平易な言語で記述した指示に基づいてリードレコードに基づいて行動するAI エージェントを作成します。 たとえば、エージェントはリードのデータを正規化したり、ボットの可能性が高いフラグを立てたりした後、その結果をリードのフィールドに書き戻すことができます。 これにより、カスタムコードなしで、判断ベースのリード処理をキャンペーンに取り入れることができます。</td>
   <td><i>近日リリース予定</i></td>
   <td><i>近日リリース予定</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>このプログラム/フォルダーに複製</strong>: Marketo Engage全体の複製操作では、複製先を選択する際に、最初の選択肢として「このフォルダー」または「このプログラム」オプションが一貫して提供されるようになりました。 このオプションを選択すると、アセットが現在のアセットの親プログラムまたはフォルダーに複製されます。</td>
   <td><i>近日リリース予定</i></td>
   <td><i>近日リリース予定</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <tr>
   <td><strong>CRM同期に関する即時アラート </strong>: CRMのネイティブ同期を有効または無効にすると、CRM通知チャネルを購読しているユーザーに通知がトリガーされるようになりました。</td>
   <td><i>近日リリース予定</i></td>
   <td><i>近日リリース予定</i></td>
  </tr>
  </tr>
  </tbody>
</table>
<br/>

## お知らせ {#announcements}

* **WebからのGrab Imagesの廃止**：最新のセキュリティとプライバシーのベストプラクティスに準拠するため、10月のリリースで[WebからのGrab Images](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/images-and-files/grab-the-images-from-a-web-page){target="_blank"}機能は廃止されます。

* カスタムアクティビティ属性の&#x200B;**API名の制限**: APIまたはUIを介して作成されたカスタムアクティビティ属性のAPI名に、英数字とアンダースコアのみを含めることができるようになりました。英数字で始める必要があります。

* **リードアクティビティの取得とリードの変更の取得に関する静的リストサイズの制限**:2026年9月30日の時点で、`listId` パラメーターを含むリードアクティビティの取得またはリードの変更の取得エンドポイントへの呼び出しは、ターゲットリストに10,000個以上のリードが含まれている場合、1003 エラーコード（ターゲットの静的静的リストのレコードが多すぎることをいことを示示す）で意味）で開始します。 詳細については、[移行ガイド &#x200B;](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/migration){target="_blank"}を参照してください。
