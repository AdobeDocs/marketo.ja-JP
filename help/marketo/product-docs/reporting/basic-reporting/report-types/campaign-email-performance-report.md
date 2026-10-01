---
unique-page-id: 2360188
description: スマートキャンペーンごとにメール統計をグループ化するCampaign メールパフォーマンスレポートについて説明します。 開封数、クリック数、バウンス数、配信停止数を追跡し、キャンペーンの効果を測定できます。
title: キャンペーンメールパフォーマンスレポート
exl-id: 524222c6-7cf6-4e6d-a1a5-20a771cd9da5
feature: Reporting
TQID: https://experienceleague.adobe.com/pMoHSEmaDbjOVpoVaUi1lvUHBYkyzOwkuF1n7mxpmY0
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: e64968b2-4ee5-47f9-8cae-0588f184b9eb
    internal-label: Programs
  - id: ea90ebee-5c84-42d9-8b21-006bdabc95a3
    internal-label: Reporting
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
source-git-commit: a3bd8b47cc9c49d4b0c164219347d003441971c0
workflow-type: tm+mt
source-wordcount: '260'
ht-degree: 75%
---
# キャンペーンメールパフォーマンスレポート {#campaign-email-performance-report}

[ スマートキャンペーン ](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/understanding-batch-and-trigger-smart-campaigns.md)でグループ化されたメールのパフォーマンス統計を確認するには、キャンペーンのメールパフォーマンスレポートを実行します。

>[!NOTE]
>
>Campaign メールパフォーマンスレポートは、マーケティングアクティビティプログラムのローカルアセットとしてのみ作成できます。 分析セクションでは使用できません。

1. [レポートを作成](/help/marketo/product-docs/reporting/basic-reporting/creating-reports/create-a-report-in-a-program.md)し、**[!UICONTROL キャンペーンメール効果]**[レポートタイプ](/help/marketo/product-docs/reporting/basic-reporting/report-types/report-type-overview.md)を選択します。

1. [レポート時間枠を設定](/help/marketo/product-docs/reporting/basic-reporting/editing-reports/change-a-report-time-frame.md)し、「**[!UICONTROL レポート]**」タブをクリックします。

1. 次に、レポートを調べて、キャンペーンの各メールの効果を確認します。

   ![](assets/image2014-9-16-16-3a19-3a59.png)

   >[!TIP]
   >
   >メールの名前をクリックして、メールプレビューツールで開きます。

   キャンペーンメール効果レポートで[選択できる列](/help/marketo/product-docs/reporting/basic-reporting/editing-reports/select-report-columns.md)は次のとおりです。

   | 列 | 説明 |
   |---|---|
   | [!UICONTROL ハードバウンス済み] | 存在しないメールアドレスなどの恒久的な状況が原因で、メールの配信が却下されました。 |
   | [!UICONTROL ソフトバウンス済み] | サーバーがダウンしている、インボックスがいっぱいになっているなどの一時的な状況が原因で、メールが却下されました。 |
   | [!UICONTROL 保留中] | メールは配信中です。 |
   | [!UICONTROL クリック済みリンク] | メール内のリンクをクリックしたメール受信者の数。 |
   | [!UICONTROL 登録解除済み] | メールの&#x200B;**[!UICONTROL 登録解除]**&#x200B;リンクをクリックし、フォームに記入したメール受信者の数。 |

   >[!NOTE]
   >
   >一般的には、常識的な判断に基づいてこれらの統計を記録しています。 例えば、メールのリンクがクリックされた場合、明らかに最初にメールが開かれたことになります。 従うルールについては、「[メール効果レポート](/help/marketo/product-docs/email-marketing/email-programs/email-program-data/email-performance-report.md)」を参照してください。

   >[!MORELIKETHIS]
   >
   >* [キャンペーンメールレポートでのアセットのフィルター](/help/marketo/product-docs/reporting/basic-reporting/report-activity/filter-assets-in-a-campaign-email-reports.md)
   >* [メールの効果レポート](/help/marketo/product-docs/email-marketing/email-programs/email-program-data/email-performance-report.md)
