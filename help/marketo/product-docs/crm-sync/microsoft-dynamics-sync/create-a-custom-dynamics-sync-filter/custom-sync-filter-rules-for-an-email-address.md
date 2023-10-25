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

* リードが作成されたとき、またはリードの電子メールアドレスフィールドが更新されたときに、リードに電子メールアドレスがあるかどうかを確認し、ある場合は「Mkto に同期」をに変更します。 **[!UICONTROL True]**. それ以外の場合は、 **[!UICONTROL False]**.

* 連絡先が作成されたとき、または連絡先の電子メールアドレスフィールドが更新されたときに、連絡先に電子メールアドレスがあるかどうかを確認し、ある場合は Mkto に同期を変更します **[!UICONTROL True]** Mkto に同期を変更します。 **[!UICONTROL True]** をアカウントレコードに追加します。 それ以外の場合は、 **[!UICONTROL False]**.

* 連絡先の「会社名 (parentcustomerid)」フィールドが更新された場合、その連絡先の「Mkto との同期」フィールドが true かどうかを確認します。 該当する場合は、アカウントの Mkto に同期を変更します。 **[!UICONTROL True]** また、

* 商談の [ 見込み顧客 (customerid)] フィールドまたは [ 取引先責任者 (parentcontactid)] が更新された場合、アカウントの [Mkto に同期 ] フィールドが true か、または取引先責任者の [Mkto に同期 ] フィールドが true かを確認します。 該当する場合は、商談の Mkto に同期を変更します。 **[!UICONTROL True]** また、
