---
unique-page-id: 2359467
description: メールの効果レポート — Marketo ドキュメント — 製品ドキュメント
title: メールパフォーマンスレポート
exl-id: 327d4c0e-951f-4782-989d-4a4c6a513ebc
feature: Email Programs
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '502'
ht-degree: 100%

---

# メールパフォーマンスレポート {#email-performance-report}

配信、開封、クリックなどの統計を使用したメールの効果を確認するには、メールの効果レポートを作成します。

1. [プログラムでレポートを作成](/help/marketo/product-docs/reporting/basic-reporting/creating-reports/create-a-report-in-a-program.md)し、**[!UICONTROL メール効果]**[レポートタイプ](/help/marketo/product-docs/reporting/basic-reporting/report-types/report-type-overview.md)を選択します。
1. [レポート時間枠を変更](/help/marketo/product-docs/reporting/basic-reporting/editing-reports/change-a-report-time-frame.md)し、「**[!UICONTROL レポート]**」タブをクリックします。
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
   >メール効果レポートには、メール配信後に削除されたリードも含まれます。アクティブなリードのアクティビティのみを表示したい場合があります。その場合は、削除したユーザーをレポートから除外する必要があります。「**[!UICONTROL スマートリスト]**」タブを使用して、レポートの[スマートリストを作成](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)します。特定のフィールドに対してフィルターを適用しない場合は、「メールアドレス」フィルターを&#x200B;**[!UICONTROL 空でない]**&#x200B;に設定します。

   以下のレポート列から、キャンペーンメール効果レポートに含める[レポート列を選択](/help/marketo/product-docs/reporting/basic-reporting/editing-reports/select-report-columns.md)します。

   <table><thead>
<tr>
    <th>列</th>
    <th>説明</th>
  </tr></thead>
<tbody>
  <tr>
    <td>ハードバウンス</td>
    <td>メールアドレスが存在しないなどの恒久的な状態が原因で、メールが拒否されました。</td>
  </tr>
  <tr>
    <td>ソフトバウンス</td>
    <td>サーバーがダウンしている、インボックスがいっぱいになっているなどの一時的な状態が原因で、メールが拒否されました。</td>
  </tr>
  <tr>
    <td>保留中</td>
    <td>この数は、送信合計数から、配信済み、バウンス、ソフトバウンスのメール数を引くことで計算されます。</td>
  </tr>
  <tr>
    <td>クリック済みリンク</td>
    <td>メール内のリンクをクリックしたメール受信者の数。</td>
  </tr>
  <tr>
    <td>配信停止完了</td>
    <td>メールの登録解除リンクをクリックし、フォームに記入したメール受信者の数。</td>
  </tr>
  <tr>
    <td>中止</td>
    <td>配信できず、バウンスイベントも受信できなかったメールの数。メール送信から 3 日以内に応答が受信されない場合、メールは自動的に「中止」と判断されます。</td>
  </tr>
</tbody></table>

>[!NOTE]
>
>メールでクリックされた登録解除リンクおよびメールアドレスは、レポートの「クリックされたリンク」に登録されません。

全般的に、これらの統計を記録するには常識を使おうとしています。例えば、メールのリンクがクリックされた場合、明らかに最初にメールが開かれたことになります。メールの効果レポートでは、次の特定のルールに従います。

* **ルール 1**：各メールアクティビティレコードは、 _配信済み_、 _ハードバウンス_、 _ソフトバウンス_、 _保留中_&#x200B;のいずれか 1 つのみに設定されます。

* **ルール 2**：メールのレコードが&#x200B;*[!UICONTROL 開封済み]*&#x200B;を示したら、*配信済み*&#x200B;としてカウントされます。

* **ルール 3**：メールのレコードが&#x200B;_[!UICONTROL クリック済みメール]_&#x200B;あるいは&#x200B;_[!UICONTROL 登録解除]_&#x200B;を示したら、_配信済み_&#x200B;あるいは&#x200B;_開封済み_&#x200B;としてカウントされます。

* **ルール 4**：メールが&#x200B;_[!UICONTROL 開封済み]_&#x200B;の場合、バウンスは無視されます。メールが開封されていない場合、_ハードバウンス_&#x200B;が&#x200B;_ソフトバウンス_&#x200B;および&#x200B;_配信_&#x200B;よりも優先されます。

* **ルール 5**：送信から 3 日後にメールアクティビティを受信しなかった場合、それは「_中止_」と見なされます。

>[!NOTE]
>
>* メールプログラムやスマートキャンペーンから顧客に複数回同じメールアセットを送信した場合、メールの効果を測定するための本レポートでは 1 回の送信としてカウントします。
>
>* 様々なキャンペーンから同じ顧客に複数回メールを送信した場合、個別にカウントします。

>[!MORELIKETHIS]
>
>* [キャンペーンメールレポートでのアセットのフィルタリング](/help/marketo/product-docs/reporting/basic-reporting/report-activity/filter-assets-in-a-campaign-email-reports.md){target="_blank"}
>* [メールパフォーマンスレポートの削除／結合されたレコードのフィルタリング](/help/marketo/product-docs/reporting/basic-reporting/report-activity/filter-deleted-merged-records-email-performance-report.md){target="_blank"}
>* [メールリンクパフォーマンスレポート](/help/marketo/product-docs/email-marketing/email-programs/email-program-data/email-link-performance-report.md){target="_blank"}
