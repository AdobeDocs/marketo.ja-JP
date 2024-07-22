---
unique-page-id: 10095307
description: メールアドレスのカスタム同期フィルタールール - Marketo ドキュメント - 製品ドキュメント
title: メールアドレスのカスタム同期フィルタールール
exl-id: d1d51310-0c59-447c-818c-b25aa281c15c
feature: Microsoft Dynamics
source-git-commit: 2403ae0f1fdca3b8238f3f59e2a3b94129deb301
workflow-type: tm+mt
source-wordcount: '202'
ht-degree: 20%

---

# メールアドレスのカスタム同期フィルタールール {#custom-sync-filter-rules-for-an-email-address}

メールアドレスのないレコードが同期されないようにするには、次のルールに従います。

* リードを作成するとき、またはリードのメールアドレスフィールドが更新されたときに、リードにメールアドレスがあるかどうかを確認し、ある場合は「同期」を「mkto」に変更します **[!UICONTROL True]**。 それ以外の場合は **[!UICONTROL False]** に変更します。

* 連絡先が作成された場合、または連絡先の [E メール アドレス ] フィールドが更新された場合は、[ アカウント ] レコードで、[ 同期 ] を [Mkto] に **[!UICONTROL True]**、[ 同期 ] を [Mkto] に **[!UICONTROL True]** に変更します。 それ以外の場合は、**[!UICONTROL False]** に変更します。

* 連絡先の「会社名（parentcustomerid）」フィールドが更新されたら、連絡先の「Mkto に同期」フィールドが true であるかどうかを確認します。 その場合は、アカウントの「同期」を「Mkto」に変更し、**[!UICONTROL True]** に変更します。

* オポチュニティの「見込み顧客（customerid）」フィールドまたは「連絡先（parentcontactid）」が更新された場合、アカウントの「Mkto に同期」フィールドが true であるか、連絡先の「Mkto に同期」フィールドが true であるかを確認します。 その場合は、機会に **[!UICONTROL True]** にも同期を Mkto に変更します。
