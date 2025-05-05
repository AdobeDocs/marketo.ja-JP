---
description: Salesforce 同期ステータス - Marketo ドキュメント - 製品ドキュメント
title: Salesforce 同期ステータス
exl-id: 61197808-7812-4e0a-8ac6-4a60af0f7979
feature: Salesforce Integration
source-git-commit: 4045f262889d06304111288d30da893529396e81
workflow-type: tm+mt
source-wordcount: '554'
ht-degree: 81%

---

# Salesforce 同期ステータス {#salesforce-sync-status}

同期ステータスダッシュボードを使用して、同期手順の一部として同期ステータスとその成功ステータスを確認します。

同期手順は、オブジェクトスキーマおよびデータ自体に対する各オブジェクトタイプごとのプッシュまたはプルの操作を反映します。 統計には、同期中の新しいレコード、更新、削除、失敗したカウントが含まれます。 ユーザーは、日付、操作タイプ、オブジェクトタイプでフィルタリングできます。 同期ステータスダッシュボードには、過去 5 日間の同期サイクルのステータスが表示されます。

>[!NOTE]
>
>管理者権限が必要

## 同期ステータスの表示 {#view-sync-status}

1. 「**[!UICONTROL 管理者]**」をクリックします。

   ![](assets/salesforce-sync-status-1.png)

1. [!UICONTROL Integration] で **Salesforce** をクリックし、「**[!UICONTROL Sync Status]**」タブをクリックします。

   ![](assets/salesforce-sync-status-2.png)

デフォルトでは、統計は最近開始された順に並べ替えられます。並べ替えアイコンをクリックして、開始日時または終了日時（最新から古い順）で並べ替えることができます。

![](assets/salesforce-sync-status-3.png)

## 同期ステータスのフィルタリング {#filter-sync-status}

1. データをフィルタリングするには、ページの右端にあるフィルターアイコンをクリックします。

   ![](assets/salesforce-sync-status-4.png)

1. 日付と時間の範囲を選択し、ドロップダウンをクリックして [!UICONTROL &#x200B; オブジェクトタイプ &#x200B;]、[!UICONTROL &#x200B; 操作タイプ &#x200B;]、[!UICONTROL &#x200B; ステータスタイプ &#x200B;] でフィルタリングします。

   ![](assets/salesforce-sync-status-5.png)

1. 「**[!UICONTROL 適用]**」をクリックします。

   ![](assets/salesforce-sync-status-6.png)

**オプションの手順**：同期エラーをエクスポートするには、「**[!UICONTROL エクスポート]**」をクリックします。データは CSV としてエクスポートされます。

![](assets/salesforce-sync-status-7.png)

## 同期ステータスフィールド {#sync-status-fields}

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <th>フィールド</th> 
   <th>説明</th> 
   <th>Enum 値</th> 
  </tr> 
  <tr> 
   <td colspan="1">開始：</td> 
   <td colspan="1">同期サイクルの開始日時（ユーザーのタイムゾーン）</td> 
   <td colspan="1"></td> 
  </tr>  
  <tr> 
   <td colspan="1">終了：</td> 
   <td colspan="1">同期サイクルの終了日時（ユーザーのタイムゾーン）</td> 
   <td colspan="1"></td> 
  </tr> 
  <tr> 
   <td colspan="1">オブジェクト</td> 
   <td colspan="1">オブジェクトタイプ</td> 
   <td colspan="1">連絡先、担当者、タスク、商談、リード、その他（以下を参照）</td> 
  </tr>  
  <tr> 
   <td colspan="1">操作</td> 
   <td colspan="1">操作のタイプ</td> 
   <td colspan="1">以下の操作タイプ</td> 
  </tr>  
  <tr> 
   <td colspan="1">ステータス</td> 
   <td colspan="1">バッチのステータス</td> 
   <td colspan="1">成功、失敗、不完全、処理中、クリーンアップ*</td> 
  </tr>
  <tr> 
   <td colspan="1">新規</td> 
   <td colspan="1">新規レコードの数</td> 
   <td colspan="1"></td> 
  </tr>  
  <tr> 
   <td colspan="1">更新済み</td> 
   <td colspan="1">アップデートされたレコードの数</td> 
   <td colspan="1"></td> 
  </tr>  
  <tr> 
   <td colspan="1">削除済み</td> 
   <td colspan="1">削除されたレコードの数</td> 
   <td colspan="1"></td> 
  </tr> 
  <tr> 
   <td colspan="1">失敗した項目</td> 
   <td colspan="1">同期が失敗したレコードの数</td> 
   <td colspan="1"><br></td> 
  </tr>  
  <tr> 
   <td colspan="1">スキップ済み</td> 
   <td colspan="1">同期対象のフィールドに変更がなかったためにスキップされたレコードの数</td> 
   <td colspan="1"></td> 
  </tr>  
 </tbody> 
</table>

&#42;同期ステップの失敗後、データは整合性の以前の状態に戻りました。

## オブジェクトのタイプ {#object-type}

<table> 
 <colgroup> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td colspan="1">アカウント</td> 
  </tr>  
  <tr> 
   <td colspan="1">アカウントタイプ</td> 
  </tr> 
  <tr> 
   <td colspan="1">カスタムオブジェクト</td> 
  </tr>  
  <tr> 
   <td colspan="1">キャンペーン</td> 
  </tr>  
  <tr> 
   <td colspan="1">キャンペーンメンバステータス</td> 
  </tr>
  <tr> 
   <td colspan="1">取引先責任者</td> 
  </tr>  
  <tr> 
   <td colspan="1">メールテンプレート</td> 
  </tr>  
  <tr> 
   <td colspan="1">イベント</td> 
  </tr> 
  <tr> 
   <td colspan="1">担当者（リード）</td> 
  </tr>  
  <tr> 
   <td colspan="1">商談</td> 
  </tr>  
  <tr> 
   <td colspan="1">商談連絡先のロール</td> 
  </tr>  
  <tr> 
   <td colspan="1">タスク</td> 
  </tr>  
  <tr> 
   <td colspan="1">ユーザー</td> 
  </tr>  
 </tbody> 
</table>

## 操作のタイプ {#operation-type}

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col>
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <th>操作のタイプ</th> 
   <th>これらのオブジェクトに対して見つかりました</th> 
   <th>備考</th> 
   <th>操作のタイプ</th>
  </tr> 
  <tr> 
   <td colspan="1">プログラムと初期リンク</td> 
   <td colspan="1">キャンペーン</td> 
   <td colspan="1">プログラムへのキャンペーンのリンク</td> 
   <td colspan="1">更新</td>
  </tr>  
  <tr> 
   <td colspan="1">コンバージョンをプル</td> 
   <td colspan="1">担当者（リード）*</td> 
   <td colspan="1">SFDC から Marketo に変換アクションを取り込みます。数量（数値）は連絡先に変換するリードです</td> 
   <td colspan="1">アップデート、失敗した項目、スキップ済み</td>
  </tr> 
  <tr> 
   <td colspan="1">削除をプル</td> 
   <td colspan="1">連絡先、担当者（リード）、商談、キャンペーン、キャンペーンメンバー、商談連絡先、カスタムオブジェクト、キャンペーン、キャンペーンメンバーステータス、商談連絡先ロール</td> 
   <td colspan="1">Marketo と同期中の SFDC のレコードを削除しました</td> 
   <td colspan="1">削除済み、失敗した項目またはスキップ済み</td>
  </tr>  
  <tr> 
   <td colspan="1">更新をプル</td> 
   <td colspan="1">タスク、担当者（リード）、担当者（リード）キュー、連絡先、イベント、商談、アカウント、アカウントタイプ、キャンペーンメンバー、カスタムオブジェクト、キャンペーン、キャンペーンメンバーのステータス、イベント、担当者ステータス、商談、商談連絡先のロール</td> 
   <td colspan="1">SFDC の更新または新しいレコードを Marketo に同期し、イベントをアクティビティとして取り込みます</td> 
   <td colspan="1">新規、アップデート済み、失敗した項目またはスキップ済み</td>
  </tr>  
  <tr> 
   <td colspan="1">新規をプッシュ</td> 
   <td colspan="1">タスク、メールテンプレート</td> 
   <td colspan="1">プッシュタスク（アクティビティ）</td> 
   <td colspan="1"></td>
  </tr>
  <tr> 
   <td colspan="1">更新をプッシュ</td> 
   <td colspan="1">タスク、メールテンプレート、担当者、連絡先、キャンペーン</td> 
   <td colspan="1">SFDC にアップデートをプッシュし、削除します</td> 
   <td colspan="1">アップデート、失敗した項目、スキップ済み</td>
  </tr>  
  <tr> 
   <td colspan="1">スキーマを同期</td> 
   <td colspan="1">キャンペーンメンバー、カスタムオブジェクト、キャンペーン、キャンペーンメンバーのステータス、タスク、担当者、商談、商談連絡先のロール、ユーザー</td> 
   <td colspan="1">異なるオブジェクトのメタデータを同期し、次のサイクルで同期する新しいフィールドを決定します。</td> 
   <td colspan="1"></td>
  </tr>  
  <tr> 
   <td colspan="1">プログラムと同期</td> 
   <td colspan="1">キャンペーン</td> 
   <td colspan="1">Marketo プログラムを SFDC キャンペーンと同期</td> 
   <td colspan="1">新規、更新、失敗またはスキップ</td>
  </tr> 
  <tr> 
   <td colspan="1">アクティビティを更新</td> 
   <td colspan="1">タスク</td> 
   <td colspan="1">Salesforce からアクティビティを抽出</td> 
   <td colspan="1"></td>
  </tr>  
  <tr> 
   <td colspan="1">FKS を更新</td> 
   <td colspan="1">すべて</td> 
   <td colspan="1">すべてのオブジェクトの外部キーをアップデート</td> 
   <td colspan="1">なし</td>
  </tr>  
 </tbody> 
</table>

&#42; サブスクリプションレベルでのブランディング設定によって、レポート内のラベル（「リード」または「人物」）が決まります。
