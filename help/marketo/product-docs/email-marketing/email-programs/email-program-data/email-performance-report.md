---
unique-page-id: 2359467
description: メールの効果レポート — Marketo ドキュメント — 製品ドキュメント
title: メールの効果レポート
exl-id: 327d4c0e-951f-4782-989d-4a4c6a513ebc
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: ht
source-wordcount: '424'
ht-degree: 100%

---

# メールの効果レポート {#email-performance-report}

配信、開封、クリックなどの統計を使用したメールの効果を確認するには、メールの効果レポートを作成します。

1. [プログラムでレポートを作成](/help/marketo/product-docs/reporting/basic-reporting/creating-reports/create-a-report-in-a-program.md)し、**メール効果**[レポートタイプ](/help/marketo/product-docs/reporting/basic-reporting/report-types/report-type-overview.md)を選択します。
1. [レポート時間枠を変更](/help/marketo/product-docs/reporting/basic-reporting/editing-reports/change-a-report-time-frame.md)し、「**レポート**」タブをクリックします。
1. レポートが表示されました。次に、レポートを表示して、メールの効果を確認します。

   >[!NOTE]
   >
   >「送信日」フィルターは、メールが最初に送信された日付に基づきます。

   ![](assets/email-performance-report.png)

   >[!TIP]
   >
   >メールの名前をクリックして、メールプレビューツールで開きます。

   >[!NOTE]
   >
   >メール効果レポートには、メール配信後に削除されたリードも含まれます。アクティブなリードのアクティビティのみを表示したい場合があります。その場合は、削除したユーザーをレポートから除外する必要があります。「**スマートリスト**」タブを使用して、レポートの[スマートリストを作成](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)します。特定のフィールドに対してフィルターを適用しない場合は、「メールアドレス」フィルターを&#x200B;**空でない**&#x200B;に設定します。

   以下のレポート列から、キャンペーンメール効果レポートに含める[レポート列を選択](/help/marketo/product-docs/reporting/basic-reporting/editing-reports/select-report-columns.md)します。

   | 列 | 説明 |
   |---|---|
   | ハードバウンス | メールアドレスが存在しないなどの恒久的な状態が原因で、メールが拒否されました。 |
   | ソフトバウンス | サーバーがダウンしている、インボックスがいっぱいになっているなどの一時的な状態が原因で、メールが拒否されました。 |
   | 保留中 | この数は、送信合計数から、配信済み、バウンス、ソフトバウンスのメール数を引くことで計算されます。 |
   | クリック済みリンク | メール内のリンクをクリックしたメール受信者の数。 |
   | 配信停止完了 | メールの&#x200B;**登録解除**&#x200B;リンクをクリックし、フォームに記入したメール受信者の数。 |

   >[!NOTE]
   >
   >メールでクリックされた登録解除リンクおよびメールアドレスは、レポートの「クリックされたリンク」に登録されません。

全般的に、これらの統計を記録するには常識を使おうとしています。例えば、メールのリンクがクリックされた場合、明らかに最初にメールが開かれたことになります。メールの効果レポートでは、次の特定のルールに従います。

* **ルール 1**：各メールアクティビティレコードは、 _配信済み_、 _ハードバウンス_、 _ソフトバウンス_、 _保留中_&#x200B;のいずれか 1 つのみに設定されます。

* **ルール 2**：メールのレコードが&#x200B;*開封済み*&#x200B;を示したら、*配信済み*&#x200B;としてカウントされます。

* **ルール 3**：メールのレコードが&#x200B;_クリック済みメール_&#x200B;あるいは&#x200B;_登録解除_&#x200B;を示したら、_配信済み_&#x200B;あるいは&#x200B;_開封済み_&#x200B;としてカウントされます。

* **ルール 4**：メールが&#x200B;_開封済み_&#x200B;の場合、バウンスは無視されます。メールが開封されていない場合、_ハードバウンス_&#x200B;が&#x200B;_ソフトバウンス_&#x200B;および&#x200B;_配信_&#x200B;よりも優先されます。

>[!NOTE]
>
>メールプログラムやスマートキャンペーンから顧客に複数回同じメールアセットを送信した場合、メールの効果を測定するための本レポートでは 1 回の送信としてカウントします。

>[!MORELIKETHIS]
>
>* [キャンペーンメールレポートでアセットをフィルターする](/help/marketo/product-docs/reporting/basic-reporting/report-activity/filter-assets-in-a-campaign-email-reports.md)
>* [メールリンクパフォーマンスレポート](/help/marketo/product-docs/email-marketing/email-programs/email-program-data/email-link-performance-report.md)

