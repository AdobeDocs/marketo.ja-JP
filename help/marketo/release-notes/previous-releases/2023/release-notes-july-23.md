---
description: リリースノート - 2023年7月 - Marketo ドキュメント - 製品ドキュメント
title: リリースノート - 2023年7月
feature: Release Information
exl-id: 4056353c-4125-4849-8350-59c58afb9e66
source-git-commit: dc13ffb4232b39d702ba835814f272256c153f6a
workflow-type: tm+mt
source-wordcount: '654'
ht-degree: 68%

---

# リリースノート：2023年7月 {#release-notes-july-23}

2023年7月リリースに含まれるすべての機能を以下に示します。機能の可用性についてはお使いの Marketo Engage のエディションをご確認ください。

>[!AVAILABILITY]
>
>星（![星](assets/yellow-star.png)）で示す機能は有償オプションです。詳しくは、Marketo Engage 担当営業にお問い合わせください。

## 標準リリースサイクルの機能 {#standard-release-cycle-features}

以下の機能は標準リリースサイクルに従っており、**2023年7月21日**（PT）からリリースが開始され、その次の週から残りの機能が段階的にロールアウトされます。リリースの機能と日付は変更される場合があります。各機能のステータスについては、以下を確認してください。

</br>

* **エンゲージメントマップ**：エンゲージメントマップは、再利用可能なキャンペーンを作成および整理するための視覚的なツールです。 完全な下位互換性があるので、ボタンをクリックすることで、既存のすべてのキャンペーンがこの新しい構造に表示できます。マップはダウンロードして共有できます。

<table> 
  <tr> 
   <td><b>ステータス</b></td>
   <td><b>ドキュメントの更新</b></td>
  </tr>
  <tr> 
   <td>リリース済み</td>
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/engagement-map/engagement-map-overview.md" target="_blank">エンゲージメントマップ：概要</a></td>
  </tr>
  </tbody>
</table>

* **通知 — Web サービスエラー**: Web サービスエラー通知にサブスクリプション名が含まれるようになり、これにより、複数のMarketo Engageインスタンスを管理しやすくなりました。 また、エラーコードとカウントを含むテーブルに「User」列を追加しました。これにより、Marketo REST API の呼び出し時に、特定のエラーの生成を担当した API ユーザーを簡単に特定できます。

<table> 
  <tr> 
   <td><b>ステータス</b></td>
   <td><b>ドキュメントの更新</b></td>
  </tr>
  <tr> 
   <td>リリース済み</td>
   <td>該当なし</td>
  </tr>
  </tbody>
</table>

## アジャイルリリースの機能

以下の機能は、アジャイル形式に従い、標準リリース日前後の様々な日付にリリースされます。各機能のステータスについては、以下を確認してください。

### Dynamic Chat {#dynamic-chat}

</br>

* **Dynamic Chat のチャットソース**：「チャット」は、新しい人物のレコードとアクティビティのソースとして提供されるようになりました。このソースは、スマートリスト／キャンペーンのアクティビティをフィルタリングするのに役立ちます。フィールドの更新からソースをブロックすることもできます。

<table> 
  <tr> 
   <td><b>ステータス</b></td>
   <td><b>ドキュメントの更新</b></td>
  </tr>
  <tr> 
   <td>リリース済み</td>
   <td>該当なし</td>
  </tr>
  </tbody>
</table>

* **強化された Dynamic Chat アクティビティ**：Dynamic Chat アクティビティ、フィルターおよびトリガーは、追加の属性および標準化された命名規則で強化されました。

<table> 
  <tr> 
   <td><b>ステータス</b></td>
   <td><b>ドキュメントの更新</b></td>
  </tr>
  <tr> 
   <td>リリース済み</td>
   <td>該当なし</td>
  </tr>
  </tbody>
</table>

### Marketo Sales Insight {#marketo-sales-insight}

</br>

* **Sales Insight アクションの配信停止追加設定**：配信停止の追加を解除する新しい設定オプションを使用して、配信停止メッセージをより詳細に制御できるようになりました。 新機能により、管理者は、いつ、どこに、どのような登録解除メッセージをセールスメールに表示するかを制御できます。

<table> 
  <tr> 
   <td><b>ステータス</b></td>
   <td><b>ドキュメントの更新</b></td>
  </tr>
  <tr> 
   <td>リリース済み</td>
   <td><a href="/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/auto-append-unsubscribe-message-setting.md" target="_blank">配信停止メッセージの自動追加設定</a></td>
  </tr>
  </tbody>
</table>

* **Sales Insight アクション用の動的フィールドプロンプト**:Sales Insight アクションのメールテンプレートに新しいフィールドプロンプトを追加して、E メールの特定の部分をパーソナライズするようセールスチームに促すことができるようになりました。

<table> 
  <tr> 
   <td><b>ステータス</b></td>
   <td><b>ドキュメントの更新</b></td>
  </tr>
  <tr> 
   <td>リリース済み</td>
   <td><a href="/help/marketo/product-docs/marketo-sales-insight/actions/templates/field-prompts.md" target="_blank">フィールドプロンプト</a></td>
  </tr>
  </tbody>
</table>

* **Sales Insight アクションのデフォルトの動的フィールド**：デフォルトの動的フィールドを使用すると、入力可能な値がない場合に動的フィールドが解決できるフォールバック値を設定できます。 これは、確実にすべてのパーソナライゼーションが入力された状態でメールを送信するのに役立ちます。

<table> 
  <tr> 
   <td><b>ステータス</b></td>
   <td><b>ドキュメントの更新</b></td>
  </tr>
  <tr> 
   <td>リリース済み</td>
   <td><a href="/help/marketo/product-docs/marketo-sales-insight/actions/templates/dynamic-fields.md" target="_blank">動的フィールド</a></td>
  </tr>
  </tbody>
</table>

* **Sales Insight 用の Dynamic Chat サポート**：すべての Dynamic Chat ユーザーに対して、このリリースで導入される新しい Dynamic Chat 属性をサポートするためのアップデートが行われました。

<table> 
  <tr> 
   <td><b>ステータス</b></td>
   <td><b>ドキュメントの更新</b></td>
  </tr>
  <tr> 
   <td><i>まもなくリリース</i></td>
   <td><i>まもなくリリース</i></td>
  </tr>
  </tbody>
</table>

* **Sales Insight Actions 用の Dynamic Chat サポート**：リードフィードおよびライブチャットがエージェントに転送される際の通知で、Dynamic Chat アクティビティをサポートしました。

<table> 
  <tr> 
   <td><b>ステータス</b></td>
   <td><b>ドキュメントの更新</b></td>
  </tr>
  <tr> 
   <td><i>まもなくリリース</i></td>
   <td><i>まもなくリリース</i></td>
  </tr>
  </tbody>
</table>

* **Dynamic Chat トリガートークン**：注目のアクションで使用するための、Dynamic Chat アクティビティ用の新しいトリガートークンが導入されました。

<table> 
  <tr> 
   <td><b>ステータス</b></td>
   <td><b>ドキュメントの更新</b></td>
  </tr>
  <tr> 
   <td>リリース済み</td>
   <td><a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/tabs-in-the-msi-panel/interesting-moments/trigger-tokens-for-interesting-moments.md" target="_blank">Dynamic Chatトリガートークン</a></td>
  </tr>
  </tbody>
</table>

## お知らせ {#announcements}

* **Google Analytics 4 へのアップグレード**：Marketo では、以前、Universal Analytics をサポートしていましたが、2023年7月1日にデータの記録を停止します。RTP ユーザーは、Google Analytics ダッシュボードの移行プロセスに従って、RTP での Google Analytics 4 統合のサポートを完了させる必要があります。今後、ユーザーは、ランディングページに一意の英数字のタグ（html の `<head>` セクション内に配置）を持ち、Marketo が Google Analytics にデータを送信できるようになります。

* **_製品リリースウェビナー_**: [2023 年 7 月および 9 月のMarketo Engageリリースウェビナー](https://engage.marketo.com/2023_July_September_Release_Webinar_OnDemandPage.html){target="_blank"}
