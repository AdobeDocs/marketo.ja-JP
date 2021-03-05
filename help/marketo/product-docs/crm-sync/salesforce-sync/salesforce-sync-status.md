---
description: Salesforce同期ステータス — Marketto Docs — 製品ドキュメント
title: Salesforce同期ステータス
translation-type: tm+mt
source-git-commit: 98af67caaf485535ba2177aa661a503990e8698d
workflow-type: tm+mt
source-wordcount: '552'
ht-degree: 0%

---


# Salesforce同期ステータス{#salesforce-sync-status}

同期ステータスダッシュボードを使用して、同期ステータスとその成功ステータスの一部として、表示同期の統計を同期します。

同期手順は、オブジェクトスキーマとデータ自体に対する各オブジェクトタイプ別のプッシュ操作またはプル操作を反映します。 統計は、同期中の新しいレコード、更新、削除および失敗したカウントをカバーします。 日付、操作のタイプまたはオブジェクトのタイプでフィルターできます。 同期ステータスダッシュボードには、過去5日間の同期サイクルの状態が表示されます。

>[!NOTE]
>
>必要な管理者権限

## 表示同期の状態{#view-sync-status}

1. 「**管理者**」をクリックします。

   ![](assets/salesforce-sync-status-1.png)

1. 「統合」で、「Salesforce」をクリックし、「同期ステータス」タブをクリックします。

   ![](assets/salesforce-sync-status-2.png)

デフォルトでは、統計は、最も最近開始されたもので並べ替えられます。 並べ替えアイコンをクリックして、「開始日」または「終了日」を基準に並べ替えることができます。並べ替えの基準は、最新のものから最も古いものまでです。

![](assets/salesforce-sync-status-3.png)

## フィルター同期の状態{#filter-sync-status}

1. データをフィルターするには、ページの右端にあるフィルターアイコンをクリックします。

   ![](assets/salesforce-sync-status-4.png)

1. 日付と時間の範囲を選択し、ドロップダウンリストをクリックして、「オブジェクトの種類」、「操作の種類」または「ステータスの種類」（またはその両方）でフィルターします。

   ![](assets/salesforce-sync-status-5.png)

1. 「**適用**」をクリックします。

   ![](assets/salesforce-sync-status-6.png)

**オプションの手順**:同期エラーを書き出すには、「 **書き出し**」をクリックします。データはCSVとしてエクスポートされます。

![](assets/salesforce-sync-status-7.png)

## 同期ステータスフィールド{#sync-status-fields}

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
   <th>列挙値</th> 
  </tr> 
  <tr> 
   <td colspan="1">開始日</td> 
   <td colspan="1">同期サイクル開始の日付/時刻（ユーザーのタイムゾーン）</td> 
   <td colspan="1"></td> 
  </tr>  
  <tr> 
   <td colspan="1">終了日：</td> 
   <td colspan="1">同期サイクルの終了日時（ユーザーのタイムゾーン）</td> 
   <td colspan="1"></td> 
  </tr> 
  <tr> 
   <td colspan="1">オブジェクト</td> 
   <td colspan="1">オブジェクトの種類</td> 
   <td colspan="1">連絡先、担当者、タスク、オポチュニティ、リード、その他</td> 
  </tr>  
  <tr> 
   <td colspan="1">操作</td> 
   <td colspan="1">操作の種類</td> 
   <td colspan="1">次の操作タイプ</td> 
  </tr>  
  <tr> 
   <td colspan="1">ステータス</td> 
   <td colspan="1">バッチの状態</td> 
   <td colspan="1">成功、失敗、不完全、処理中、クリーンアップ*</td> 
  </tr>
  <tr> 
   <td colspan="1">新規</td> 
   <td colspan="1">新しいレコードの数</td> 
   <td colspan="1"></td> 
  </tr>  
  <tr> 
   <td colspan="1">更新済み</td> 
   <td colspan="1">更新されたレコードの数</td> 
   <td colspan="1"></td> 
  </tr>  
  <tr> 
   <td colspan="1">削除済み</td> 
   <td colspan="1">削除されたレコードの数</td> 
   <td colspan="1"></td> 
  </tr> 
  <tr> 
   <td colspan="1">失敗した項目</td> 
   <td colspan="1">同期に失敗したレコードの数</td> 
   <td colspan="1"><br></td> 
  </tr>  
  <tr> 
   <td colspan="1">スキップ</td> 
   <td colspan="1">同期に関心のあるフィールドに変更がなかったため、スキップされたレコードの数</td> 
   <td colspan="1"></td> 
  </tr>  
 </tbody> 
</table>

*同期ステップの失敗後、データは整合性の以前の状態に戻りました。

## オブジェクトタイプ{#object-type}

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
   <td colspan="1">キャンペーンメンバーの状態</td> 
  </tr>
  <tr> 
   <td colspan="1">連絡先</td> 
  </tr>  
  <tr> 
   <td colspan="1">電子メールテンプレート</td> 
  </tr>  
  <tr> 
   <td colspan="1">イベント</td> 
  </tr> 
  <tr> 
   <td colspan="1">人（リーダー）</td> 
  </tr>  
  <tr> 
   <td colspan="1">オポチュニティ</td> 
  </tr>  
  <tr> 
   <td colspan="1">商談の連絡先の役割</td> 
  </tr>  
  <tr> 
   <td colspan="1">タスク</td> 
  </tr>  
  <tr> 
   <td colspan="1">ユーザー</td> 
  </tr>  
 </tbody> 
</table>

## 操作の種類{#operation-type}

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col>
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <th>操作の種類</th> 
   <th>これらのオブジェクトに対して見つかりました</th> 
   <th>備考</th> 
   <th>操作の種類</th>
  </tr> 
  <tr> 
   <td colspan="1">プログラムとの初期リンク</td> 
   <td colspan="1">キャンペーン</td> 
   <td colspan="1">キャンペーンのプログラムへのリンク</td> 
   <td colspan="1">更新</td>
  </tr>  
  <tr> 
   <td colspan="1">プルコンバージョン</td> 
   <td colspan="1">人（リード）*</td> 
   <td colspan="1">SFDCからMarketoへのコンバージョンアクションを取り込みます。 数量（数値）はリードが連絡先に変換しています</td> 
   <td colspan="1">更新、失敗したアイテム、スキップ</td>
  </tr> 
  <tr> 
   <td colspan="1">削除の取り込み</td> 
   <td colspan="1">連絡先，個人（リード），商談，キャンペーン,キャンペーンメンバー，商談連絡先，カスタムオブジェクト，キャンペーン,キャンペーンメンバーのステータス，商談連絡先ロール</td> 
   <td colspan="1">Marketoと同期されるSFDCのレコードが削除されました</td> 
   <td colspan="1">削除済み、失敗したアイテム、またはスキップ</td>
  </tr>  
  <tr> 
   <td colspan="1">更新の取り込み</td> 
   <td colspan="1">タスク、個人（リード）、個人（リード）キュー、連絡先、イベント、営業案件、取引先企業、取引先企業、取引先企業タイプ、キャンペーンメンバー、カスタムオブジェクト、キャンペーン、キャンペーンメンバーのステータス、イベント、個人ステータス、商談、商談担当者の役割</td> 
   <td colspan="1">SFDCでMarketorと同期された更新または新しいレコード、イベントをアクティビティとして取り込む</td> 
   <td colspan="1">新規、更新、失敗したアイテム、またはスキップ</td>
  </tr>  
  <tr> 
   <td colspan="1">新規プッシュ</td> 
   <td colspan="1">タスク、電子メールテンプレート</td> 
   <td colspan="1">プッシュタスク(アクティビティ)</td> 
   <td colspan="1"></td>
  </tr>
  <tr> 
   <td colspan="1">プッシュの更新</td> 
   <td colspan="1">タスク，電子メールテンプレート，人，連絡先，キャンペーン</td> 
   <td colspan="1">SFDCに更新をプッシュして削除する</td> 
   <td colspan="1">更新、失敗したアイテム、スキップ</td>
  </tr>  
  <tr> 
   <td colspan="1">同期スキーマ</td> 
   <td colspan="1">キャンペーンメンバー，カスタムオブジェクト，キャンペーン,キャンペーンメンバーのステータス，タスク，人，商談，商談担当者の役割，ユーザー</td> 
   <td colspan="1">異なるオブジェクトのメタデータを同期し、次のサイクルで同期する新しいフィールドを決定</td> 
   <td colspan="1"></td>
  </tr>  
  <tr> 
   <td colspan="1">プログラムと同期</td> 
   <td colspan="1">キャンペーン</td> 
   <td colspan="1">MarketoプログラムとSFDCキャンペーンを同期</td> 
   <td colspan="1">新規、更新、失敗またはスキップ</td>
  </tr> 
  <tr> 
   <td colspan="1">アクティビティの更新</td> 
   <td colspan="1">タスク</td> 
   <td colspan="1">Salesforceからのアクティビティの取り込み</td> 
   <td colspan="1"></td>
  </tr>  
  <tr> 
   <td colspan="1">FKSの更新</td> 
   <td colspan="1">すべて</td> 
   <td colspan="1">すべてのオブジェクトの外部キーを更新する</td> 
   <td colspan="1">該当なし</td>
  </tr>  
 </tbody> 
</table>

*購読レベルでのブランド設定によって、レポートのラベル（「リード」または「人」）が決まります。
