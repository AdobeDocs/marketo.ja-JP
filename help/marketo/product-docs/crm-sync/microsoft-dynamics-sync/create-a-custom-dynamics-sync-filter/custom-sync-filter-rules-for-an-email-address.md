---
unique-page-id: 10095307
description: 電子メールアドレス用のカスタム同期フィルタールール —Marketoドキュメント — 製品ドキュメント
title: 電子メールアドレスのカスタム同期フィルター規則
exl-id: d1d51310-0c59-447c-818c-b25aa281c15c
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '202'
ht-degree: 0%

---

# 電子メールアドレス{#custom-sync-filter-rules-for-an-email-address}のカスタム同期フィルター規則

電子メールアドレスを持たないレコードを同期しないようにするには、次のルールに従います。

* リードが作成されたOR時に、リードの電子メールアドレスフィールドが更新された場合は、リードに電子メールアドレスが含まれているかどうかを確認し、含まれている場合は、Sync to Mkto **True**&#x200B;に変更します。 それ以外の場合は&#x200B;**False**&#x200B;に変更します。

* 連絡先が作成されたOR時に、連絡先の電子メールアドレスフィールドが更新された場合は、連絡先に電子メールアドレスが含まれているかどうかを確認し、含まれている場合は、SyncをMkto **True**&#x200B;に変更し、Sync to Mkto **True**&#x200B;に変更します。 それ以外の場合は、**False**&#x200B;に変更します。

* 連絡先の会社名(parentcustomerid)フィールドが更新された場合は、連絡先の「Mktoと同期」フィールドがtrueかどうかを確認します。 その場合は、アカウント上のSyncをMktoに変更して&#x200B;**True**&#x200B;にも変更します。
* オポチュニティの潜在的な顧客(customerid)フィールドまたは連絡先(parentcontactid)が更新された場合、アカウントの「Sync to Mkto」フィールドがtrueか、連絡先の「Sync to Mkto」フィールドがtrueかを確認します。 同期が有効な場合は、オポチュニティ上でSyncをMktoに変更します。**True**&#x200B;にも変更します。
