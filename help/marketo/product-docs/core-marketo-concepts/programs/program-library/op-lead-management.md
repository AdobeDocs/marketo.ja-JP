---
description: OP-Lead Management - Marketo ドキュメント – 製品ドキュメント
title: OP-リード管理
feature: Programs
exl-id: bde644fe-d40b-4c9c-925d-a0f522e6de01
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '265'
ht-degree: 16%

---

# OP-リード管理 {#op-lead-management}

これは、Marketo Engageのデフォルトプログラムを利用したリード管理のベストプラクティスワークフローの例で、Marketo Engage データベース内のレコードを CRM に対して管理する際に役立ちます。

>[!NOTE]
>
>Marketo Engageでは、データベース内のレコードは人物/人物と呼ばれます。 この例のリード管理は、CRM のレコードを参照しています。

詳細な方法に関するサポートや、プログラムのカスタマイズに関するヘルプについては、Adobe アカウントチームに問い合わせるか、[Adobe Professional Services](https://business.adobe.com/jp/customers/consulting-services/main.html) のページを参照してください。

## チャネルサマリ {#channel-summary}

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th>チャネル</th>
   <th>メンバーシップのステータス</th>
   <th>アナリティクス動作</th>
   <th>プログラムのタイプ</th>
  </tr>
  <tr>
   <td>オペレーショナル</td>
   <td>01 – メンバー</td>
   <td>オペレーショナル</td>
   <td>デフォルト</td>
  </tr>
 </tbody>
</table>

## プログラムには、次のAssetsが含まれています {#program-contains-the-following-assets}

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
   <td>01 – 新しいユーザーを CRM に同期</td>
  </tr>
  <tr>
   <td>スマートキャンペーン</td>
   <td> </td>
   <td>02 - マーケティング認定</td>
  </tr>
  <tr>
   <td>メール</td>
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-email-template.md" target="_blank">クイックスタートメールテンプレート</a></td>
   <td>01 - メール – アラート - MQL</td>
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

![](assets/op-lead-management-1.png)

## 競合ルール {#conflict-rules}

* **プログラムタグ**
   * このサブスクリプションにタグを作成 – _推奨_
   * 無視

* **同じ名前のランディングページテンプレート**
   * 元のテンプレートをコピー – _推奨_
   * インポート先のテンプレートの使用

* **同じ名前の画像**
   * 両方のファイルを保持 – _推奨_
   * このサブスクリプション内アイテムの置換

* **同じ名前のメールテンプレート**
   * 両方のテンプレートを保持 – _推奨_
   * 既存テンプレートの置換

## ベストプラクティス {#best-practices}

* 組織で追跡する可能性のあるライフサイクルステータスのニーズのそれぞれに対応するために、追加のスマートキャンペーンを追加することを検討します。 このプログラムで作成された各キャンペーンは、ベストプラクティスのビルドの例であり、すべてのユースケースに固有のものではありません。 特定のリードライフサイクル管理プロセスに対応するようにスマートキャンペーンを必ず更新してください。

* このプログラムの例の命名規則を更新して、現在の例に合わせることを検討してください。
