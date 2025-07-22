---
unique-page-id: 12981145
description: パフォーマンスインサイトの設定 - Marketo ドキュメント - 製品ドキュメント
title: パフォーマンスインサイトの設定
exl-id: f87bbaba-c2c1-4b83-9e07-f8a5d1f1738b
feature: Reporting
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '310'
ht-degree: 89%

---

# 設定 [!UICONTROL  パフォーマンスインサイト ] {#setting-up-performance-insights}

以下の手順に従って MPI を設定します。

## 商談の設定 {#opportunity-setup}

1. 「**[!UICONTROL 管理者]**」をクリックします。

   ![](assets/admin.png)

1. 「**[!UICONTROL 収益サイクルアナリティクス]**」をクリックします。

   ![](assets/two-2.png)

   >[!NOTE]
   >
   >収益サイクルアナリティクスがない場合は、手順 2 で「**[!UICONTROL プログラム分析]**」を選択する必要があります。

1. 「属性」で、「**[!UICONTROL 編集]**」をクリックします。

   ![](assets/three-1.png)

1. 「属性設定」が表示されます。

   ![](assets/four-2.png)

   属性が明示的な場合は、（商談の役割エンドポイントまたは CRM 統合を介して）商談連絡先の役割が設定されていることを確認します。

   属性が暗黙的な場合は、リード／連絡先の会社フィールドが商談の顧客名と同じであることを確認します。

   >[!NOTE]
   >
   >すべての商談に次の適切なフィールドが設定されていることを確認します。
   >
   >* [!UICONTROL  オポチュニティの金額 ]
   >* [!UICONTROL  終了 ]
   >* [!UICONTROL  勝った ]
   >* [!UICONTROL  作成日 ] （お客様の場合は設定できない場合があります）
   >* [!UICONTROL  クローズ日 ] （お客様の場合は設定できない場合があります）
   >* [!UICONTROL  商談タイプ ]

## プログラムセットアップ {#program-setup}

少なくとも 12 か月間、プログラムのコストを更新します。これは、手動で実行するか、プログラム API を使用して実行できます。この例では、手動でおこないます。

1. 「**[!UICONTROL マーケティングアクティビティ]**」をクリックします。

   ![](assets/ma.png)

1. プログラムを選択します。

   ![](assets/select-program.png)

1. 「**[!UICONTROL 設定]**」タブをクリックします。

   ![](assets/setup-tab.png)

1. **[!UICONTROL 期間原価]**&#x200B;をキャンバスにドラッグします。

   ![](assets/period-cost.png)

1. 12 か月以上前にプログラムの月を設定し、「**[!UICONTROL Ok]**」をクリックします。

   ![](assets/set-period.png)

1. 期間原価を設定し、「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/set-cost.png)

次に、分析動作をレビューして、特定のチャネルを分析に含める必要があるかどうかを示します。分析動作（標準、包括的、運用可能）を設定します。

1. 「**[!UICONTROL 管理者]**」をクリックします。

   ![](assets/admin.png)

1. 「**[!UICONTROL タグ]**」をクリックします。

   ![](assets/tags.png)

1. 「**+**」をクリックして、チャネルリストを展開します。

   ![](assets/channel.png)

1. 目的のチャネルをダブルクリックします。

   ![](assets/channel-click.png)

1. **[!UICONTROL 分析動作]**&#x200B;ドロップダウンをクリックして、目的の動作を選択します。

   ![](assets/edit-channel.png)

1. 達成基準を設定します。

   ![](assets/success.png)

1. 「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/save.png)

## プログラムをリードに結び付ける {#tie-the-program-to-the-person}

1. ファーストタッチ属性を機能させるために、データベース内の各ユーザーに対して獲得プログラムと獲得日が設定されていることを確認します。
1. プログラムで、顧客の成功状態が設定されていることを確認します。

>[!NOTE]
>
>変更は即時にはおこなわれません。変更が有効になる前には一晩が必要です。
