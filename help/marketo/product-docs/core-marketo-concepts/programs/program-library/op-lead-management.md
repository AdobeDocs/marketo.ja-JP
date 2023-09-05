---
description: OP リード管理 — Marketoドキュメント — 製品ドキュメント
title: OP-リード管理
hide: true
hidefromtoc: true
feature: Programs
source-git-commit: 9c9046d6ac889bef4ec8ab7add82fda8e72d73b4
workflow-type: tm+mt
source-wordcount: '273'
ht-degree: 15%

---

# OP-リード管理 {#op-lead-management}

これは、Marketo Engageのデフォルトプログラムを利用して、リード管理のベストプラクティスワークフローの例で、Marketo Engageデータベース内のレコードを CRM に管理するのに役立ちます。

>[!NOTE]
>
>Marketo Engageでは、データベース内のレコードは人/人と呼ばれます。 この例のリード管理は、CRM のレコードを参照しています。

戦略に関するサポートやプログラムのカスタマイズについては、Adobeアカウントチームにお問い合わせいただくか、 [Adobe Professional Services](https://business.adobe.com/customers/consulting-services/main.html) ページに貼り付けます。

## チャネルサマリ {#channel-summary}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>チャネル</th> 
   <th>メンバーシップステータス</th>
   <th>アナリティクス動作</th>
   <th>プログラムのタイプ</th>
  </tr> 
  <tr> 
   <td>オペレーショナル</td> 
   <td>01 — メンバー</td>
   <td>オペレーショナル</td>
   <td>デフォルト</td>
  </tr>
 </tbody> 
</table>

## プログラムに次のアセットが含まれています {#program-contains-the-following-assets}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>タイプ</th> 
   <th>テンプレート名</th>
   <th>アセット名</th>
  </tr> 
  <tr> 
   <td>スマートキャンペーン</td> 
   <td> </td>
   <td>01 — 新しい担当者を CRM に同期</td>
  </tr>
  <tr> 
   <td>スマートキャンペーン</td> 
   <td> </td>
   <td>02 — マーケティング認定</td>
  </tr>
  <tr> 
   <td>メール</td> 
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-email-template.md" target="_blank">クイックスタートメールテンプレート</a></td>
   <td>01 — 電子メール — アラート — MQL</td>
  </tr>
  <tr> 
   <td>フォルダー</td> 
   <td> </td>
   <td>キャンペーン</td>
  </tr>
  <tr> 
   <td>フォルダー</td> 
   <td> </td>
   <td>メールアラート</td>
  </tr>
 </tbody> 
</table>

プログラムのスクリーンショット

## 競合ルール {#conflict-rules}

* **プログラムタグ**
   * この配信登録にタグを作成 — _推奨_
   * 無視する

* **同じ名前のランディングページテンプレート**
   * 元のテンプレートをコピー — _推奨_
   * インポート先のテンプレートの使用

* **同じ名前の画像**
   * 両方のファイルを保持 — _推奨_
   * この配信登録内アイテムの置換

* **同じ名前のメールテンプレート**
   * 両方のテンプレートを保持 — _推奨_
   * 既存テンプレートの置換

競合ルールのスクリーンショット

## ベストプラクティス {#best-practices}

* 組織で追跡する可能性のある各ライフサイクルステータスニーズに対応するために、追加のスマートキャンペーンを追加することを検討します。 このプログラムで作成される各キャンペーンは、ベストプラクティスビルドの例を示すもので、すべての使用例に特有のものではありません。 特定のリードライフサイクル管理プロセスに対応するために、必ずスマートキャンペーンを更新してください。

* ご使用のプログラムの例の命名規則を更新することを検討してください。
