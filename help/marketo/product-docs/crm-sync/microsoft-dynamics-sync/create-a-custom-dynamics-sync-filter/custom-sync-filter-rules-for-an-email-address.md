---
unique-page-id: 10095307
description: Dynamics でメールアドレスのカスタム同期フィルタールールを設定する方法を説明します。 ワークフローを使用して、リードまたは連絡先にメールがあるかどうかに基づいて、Mkto に同期を設定します。
title: メールアドレスのカスタム同期フィルタールール
exl-id: d1d51310-0c59-447c-818c-b25aa281c15c
feature: Microsoft Dynamics
source-git-commit: 2b29f05a27f847184e0968442012d443e9e0597d
workflow-type: tm+mt
source-wordcount: '220'
ht-degree: 86%

---

# メールアドレスのカスタム同期フィルタールール {#custom-sync-filter-rules-for-an-email-address}

メールアドレスのないレコードが同期されないようにするには、次のルールに従います。

* リードが作成されたとき、またはリードのメールアドレスフィールドが更新されたときは、リードにメールアドレスが含まれているかどうかを確認して、ある場合は「同期」を「**[!UICONTROL True]**」に変更します。それ以外の場合は、「**[!UICONTROL False]**」に変更します。

* 取引先責任者が作成された場合、また取引先責任者先のメールアドレスフィールドが更新された場合は、取引先責任者にメールアドレスが含まれているかどうかを確認し、存在する場合は「Mkto に同期」を **[!UICONTROL True]** にし、アカウントレコードで「Mkto に同期」を **[!UICONTROL True]** に変更します。それ以外の場合は、「**[!UICONTROL False]**」に、変更します。

* 取引先責任者の「会社名 (parentcustomerid)」フィールドが更新されたら、その取引先責任者の「Mkto と同期」フィールドが true かどうかを確認します。その場合は、アカウント上の「Mkto と同期」も「**[!UICONTROL True]**」に変更します。
* 商談の「見込み客（customerid）」フィールドまたは「取引先責任者（parentcontactid）」が更新されたら、アカウントの「Mkto に同期」フィールドが true か、または取引先責任者の「Mkto に同期」フィールドが true かを確認します。その場合は、商談でも「Mkto に同期」を **[!UICONTROL True]** に変更します。
