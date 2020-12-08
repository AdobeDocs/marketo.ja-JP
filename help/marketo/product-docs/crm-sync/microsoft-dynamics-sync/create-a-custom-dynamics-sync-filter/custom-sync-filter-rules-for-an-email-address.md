---
unique-page-id: 10095307
description: 電子メールアドレスのカスタム同期フィルタールール — Marketto Docs — 製品ドキュメント
title: 電子メールアドレスのカスタム同期フィルター規則
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '202'
ht-degree: 0%

---


# 電子メールアドレスのカスタム同期フィルター規則 {#custom-sync-filter-rules-for-an-email-address}

電子メールアドレスを持たないレコードを同期しないようにするには、次のルールに従います。

* リードが作成された場合、またはリードの電子メールアドレスフィールドが更新された場合、リードに電子メールアドレスが含まれているかどうかを確認し、含まれている場合は、Sync to Mktoを **True**&#x200B;に変更します。 それ以外の場合は **Falseに変更します**

* 連絡先が作成された場合、または連絡先の電子メールアドレスフィールドが更新された場合は、連絡先に電子メールアドレスがあるかどうかを確認し、ある場合は、アカウントレコードで **SyncをMkto** に変更し、SyncをMkto **True** に変更します。 それ以外の場合は、 **Falseに変更します。**

* 連絡先の会社名(parentcustomerid)フィールドが更新された場合は、連絡先の「Mktoと同期」フィールドがtrueかどうかを確認します。 同期されている場合は、アカウントのSyncをMktoに変更し **ます** 。
* オポチュニティの潜在的な顧客(customerid)フィールドまたは連絡先(parentcontactid)が更新された場合、アカウントの「Sync to Mkto」フィールドがtrueか、連絡先の「Sync to Mkto」フィールドがtrueかを確認します。 同期が有効な場合は、オポチュニティ上でSyncをMktoに変更し **ます** 。

