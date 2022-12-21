---
description: Salesforce 診断 - Marketo ドキュメント - 製品ドキュメント
title: Salesforce 診断
hide: true
hidefromtoc: true
exl-id: c449f938-9615-47cb-b232-613ec29068a3
source-git-commit: d960f0ad0d944bd2e74543f3ab15b59a8040b768
workflow-type: tm+mt
source-wordcount: '1445'
ht-degree: 100%

---

# Salesforce 診断 {#salesforce-diagnostics}

Salesforce 統合の一部には、Web アプリケーション内に Salesforce の診断ページが含まれています。このページでは、失敗したデータログから Salesforce にエラーを取り込みます。エラーは役に立ちますが、常に読みやすいわけでは限りません。そのため、エラーメッセージを説明するのに役立つカンニングペーパーを作成しました。

## アクセス診断 {#access-diagnostics}

1. 歯車アイコンをクリックし、「**設定**」を選択します。

   ![](assets/salesforce-diagnostics-1.png)

1. 「統合」で、「**診断**」をクリックします。

   ![](assets/salesforce-diagnostics-2.png)

## エラーカンニングペーパー {#error-cheat-sheet}

**エラー：** API_CURRENTLY_DISABLED\
**カテゴリ：**&#x200B;アクセス/検証\
**メッセージ：** API is disabled for this user\
**状況：**&#x200B;ユーザが API にアクセスできません\
**トラブルシューティング手順：** Salesforce 管理者は、ユーザ API へのアクセス権を付与する必要があります。

**エラー：** AUTHENTICATION_FAILURE\
**カテゴリ：**&#x200B;認証\
**メッセージ：** invalid_grant: authentication failure\
**状況：**&#x200B;認証に失敗します\
**トラブルシューティング手順：** Salesforce から切断し、再接続します。

**エラー：** CANNOT_INSERT_UPDATE_ACTIVATE_ENTITY\
**カテゴリ：**&#x200B;アクセス/検証\
**メッセージ：**{&quot;errorCode&quot;:&quot;INVALID_SESSION_ID&quot;,&quot;message&quot;:&quot;Session expired or invalid&quot;}\
**状況：**

1 - トリガーコードが原因で更新に失敗します。\
2 - ユーザは、指定されたオブジェクトに対するオブジェクトレベルの書き込み権限を持っていません。

**トラブルシューティングの手順：**

1 - 失敗しているトリガーを確認します。\
2 - オブジェクトに対する書き込みアクセス権をユーザに付与するか、オブジェクトに書き込もうとする機能を無効にします。

**エラー：** CANNOT_UPDATE_CONVERTED_LEAD\
**カテゴリ：**&#x200B;その他\
**メッセージ：** cannot reference converted lead\
**状況：**&#x200B;取引先責任者およびリードの最新のアクティビティログ中に、変換済みのリードにログを記録しようとしています。また、売り口上にもこれらが 2 つありました。\
**トラブルシューティング手順：**&#x200B;インスタンスがある場合、アドビの[サポートチーム](https://nation.marketo.com/t5/Support/ct-p/Support)に報告してください。

**エラー：** ENTITY_IS_LOCKED\
**カテゴリ：**&#x200B;アクセス/検証\
**メッセージ：** the entity is locked for editing\
**状況：**&#x200B;レコードは、承認プロセス中で、承認を所有する人によって承認または拒否されるまで、追加の編集内容からロックされます。\
**トラブルシューティングの手順：**&#x200B;上記を参照してください。

**エラー：**EXPIRED_ACCESS
**カテゴリ：**認証
**メッセージ：**invalid_grant: expired access/refresh token
**状況：**&#x200B;アクセスまたは更新トークンの期限が切れています。トークンは [Salesforce のセッション設定](https://salesforce.stackexchange.com/questions/10759/invalid-grant-expired-access-refresh-token-error-when-authenticating-access-via)に基づいて期限切れになります。
**トラブルシューティング手順：**&#x200B;再認証が必要になります。Salesforce 接続を切断し、再接続します。

**エラー：** FAILED_WRITE\
**カテゴリ：**&#x200B;断続的\
**メッセージ：** end of file reached\
**状況：**&#x200B;顧客側での最適でないトリガーが原因と考えられる、Salesforce のパフォーマンスの問題。\
**トラブルシューティング手順：**&#x200B;再試行ロジックで処理する必要があります。それでも問題が解決しない場合は、Salesforce の管理者に問い合わせて、問題のあるトリガーのトラブルシューティングを依頼します。

**エラー：** FIELD_CUSTOM_VALIDATION_EXCEPTION
**カテゴリ：**アクセス/検証
**メッセージ：**&#x200B;顧客によって異なります。**状況：**&#x200B;オブジェクトのカスタム検証ルールが失敗します。**トラブルシューティング手順：** このエラーを引き起こしているカスタム検証ルールを確認します。これは慣習的な規則なので、エラーは 1 回限りで対処する必要があります。

**エラー：** FIELD_FILTER_VALIDATION_EXCEPTION\
**カテゴリ：**&#x200B;アクセス/検証\
**メッセージ：** Value does not exist or does not match filter criteria\
**状況：** Salesforce の既存の不正なデータが更新時に強制されます。\
**トラブルシューティングの手順：**&#x200B;上記を参照してください。

**エラー：** FIELD_INTEGRITY_EXCEPTION\
**カテゴリ：**&#x200B;アクセス/検証\
**メッセージ：** The existing country/territory doesn&#39;t recognize the state value for field: State/Province Code\
**状況：** Salesforce の既存の不正なデータが更新時に強制されます。\
**トラブルシューティングの手順：**&#x200B;上記を参照してください。

**エラー：** INACTIVE_ORGANIZATION\
**カテゴリ：**&#x200B;認証\
**メッセージ：** invalid_grant: inactive organization\
**状況：** Salesforce 組織がアクティブではなくなりました。**トラブルシューティング手順：** Salesforce から切断し、再接続します。

**エラー：**INACTIVE_USER
**カテゴリ：**認証
**メッセージ：**invalid_grant: inactive user
**状況：**Salesforce ユーザがアクティブでなくなっています
**トラブルシューティング手順：** Salesforce から切断し、再接続します。

**エラー：** INSERT_UPDATE_EXPERIENCE_NOT_ALLOWED_DURING_MAINTENANCE\
**カテゴリ：**&#x200B;断続的\
**メッセージ：**（追加のメッセージはありません）\
**状況：** Salesforce インスタンスはメンテナンスモードです。\
**トラブルシューティング手順：**&#x200B;システムメンテナンスが完了するまで待ってから、ログを再試行します。

**エラー：**INSUFFICIENT_ACCESS_ON_CROSS_REFERENCE_ENTITY
**カテゴリ：**アクセス／検証
**メッセージ：**insufficient access rights on object id
**状況：**&#x200B;タスクの親レコードにアクセスできません。**トラブルシューティングの手順：**&#x200B;上記を参照してください。

**エラー：** INSUFFICIENT_ACCESS_OR_READONLY\
**カテゴリ：**アクセス／検証
**メッセージ：**insufficient access rights on object id
**状況：**&#x200B;最新のアクティビティログは、書き込みアクセス権を持たないので、特定のレコードを編集できません。\
**トラブルシューティング手順：** Salesforce でのユーザアクセスを許可するか、そのユーザのオブジェクトに対する最新のアクティビティログを無効にします。

**エラー：** INVALID_FIELD\
**カテゴリ：**&#x200B;断続的\
**メッセージ：** Net::ReadTimeout\
**状況：**&#x200B;リクエストがタイムアウトになっています。これは、多くの低速トランザクションの結果である可能性が高いです。\
**トラブルシューティング手順：**&#x200B;遅延の問題に関する潜在的な原因について既存のカスタマイズを確認し、1 つまたはすべてのオブジェクトの最新のアクティビティログを無効にして負荷を軽減します。

**エラー：** INVALID_FIELD_FOR_INSERT_UPDATE\
**カテゴリ：**&#x200B;アクセス/検証\
**メッセージ：** Unable to create/update fields: MSE_Replied__c. Please check the security settings of this field.**状況：**&#x200B;最新のアクティビティログトランザクションの実行に必要な Sales Insight Actions カスタムフィールドへの書き込みアクセス権がユーザに与えられていません。チームがパッケージをインストールしたが、ユーザに対して正しいフィールドが有効になっていない可能性があります。\
**トラブルシューティング手順：** Salesforce 管理者は、カスタムフィールドへのアクセス権を付与するか、最新のアクティビティのログを無効にする必要があります。

**エラー：** INVALID_GRANT\
**カテゴリ：**&#x200B;認証\
**メッセージ：** invalid_grant: ip restricted\
**状況：** Salesforce にアクセスしようとしていますが、IP 制限が設定されているので、アドビではアクセスできません。\
**トラブルシューティング手順：** Salesforce 管理者がアドビの IP を許可リストに登録する必要があります。IP アドレスを取得するには、サポートに問い合わせる必要があります。

**エラー：** INVALID_TYPE\
**カテゴリ：**&#x200B;アクセス/検証\
**メッセージ：** CreatedDate, (SELECT Id FROM Tasks) FROM Lead WHERE Email=&#39;emailid&#39;^ERROR at Row:1:Column:53sObject type &#39;Lead&#39; is not supported.カスタムオブジェクトを使用する場合、必ずエンティティ名の後に &#39;__c&#39; を添付してください。Please reference your WSDL or the describe call for the appropriate names
**状況：**&#x200B;ユーザがアクセスできない Salesforce のオブジェクトタイプをクエリしようとしています。これは、ユーザがリードオブジェクトに対する権限を持っていないことが原因である可能性が高いです。\
**トラブルシューティング手順：** Salesforce のリードオブジェクトに対して読み取りおよび更新アクセス権を付与するか、リードレコードへのメールログと最新のアクティビティのログをオフにします。

**エラー：** QUERY_TIMEOUT\
**カテゴリ：**&#x200B;断続的\
**メッセージ：** Your query request was running too long\
**状況：**&#x200B;上記を参照してください。\
**トラブルシューティング手順：**&#x200B;再試行ロジックで処理する必要があります。それでも問題が解決しない場合は、Salesforce 管理者に問い合わせて、問題のあるトリガーのトラブルシューティングを依頼します。

**エラー：** REQUEST_LIMIT_EXCEEDED\
**カテゴリ：**&#x200B;断続的\
**メッセージ：**
1 - ConcurrentPerOrgLongTxn Limit exceeded\
2 - TotalRequests Limit exceeded\
3 - ConcurrentRequest\
**状況：**
1 - トリガーコードが非効率なため、同時リクエストの制限を超えています。\
2 - 統合が多すぎるため、組織が 24 時間周期の期間を超えています。\
**トラブルシューティング手順：**
1 - 影響を受けたオブジェクトの既存のトリガーを確認します。1 つ以上のオブジェクトのロールアップログを無効にする可能性があります。\
2 - Salesforce からさらに API 呼び出しを購入します。1 つ以上のオブジェクトのロールアップログを無効にする可能性があります。

**エラー：** REQUIRED_FIELD_MISSING\
**カテゴリ：**&#x200B;アクセス/検証\
**メッセージ：** Required fields are missing: `[Amount_Committed_Private_Capital__c]`
**状況：**&#x200B;これは通常、最新のアクティビティログで発生します。カスタムフィールドは必須として設定されていますが、値が空です。これは、レコードがカスタムフィールドの空の値で作成され、その後必須に設定された場合に発生する可能性があります。レコードを更新しようとすると、カスタムフィールドに触れなくても、要件が適用されます。\
**トラブルシューティングの手順：**&#x200B;見つからないフィールドの値を手動で更新します。その後、Sales Insight Actions からのメッセージを再試行できます。

**エラー：** SERVER_UNAVAILABLE\
**カテゴリ：**&#x200B;断続的\
**メッセージ：** server too busy\
**状況：**&#x200B;顧客による最適でないトリガーが原因と考えられる、Salesforce のパフォーマンスの問題\
**トラブルシューティング手順：**&#x200B;再試行ロジックで処理する必要があります。まだ機能しない場合は、Salesforce 管理者と協力して、問題のあるトリガーをトラブルシューティングします。

**エラー：** TXN_SECURITY_NO_ACCESS\
**カテゴリ：**&#x200B;アクセス/検証\
**メッセージ：** The operation you requested isn&#39;t allowed due to a security policy in your organization.システム管理者にお問い合わせください。**状況：**&#x200B;何らかのセキュリティ制限が設定されています。 https://developer.salesforce.com/forums/?id= 「レコード ID」を参照してください。\
**トラブルシューティング手順：** Salesforce の管理者に問い合わせて、特定の制限事項を確認します。

**エラー：** UNABLE_TO_LOCK_ROW\
**カテゴリ：**&#x200B;断続的\
**メッセージ：** unable to obtain exclusive access to this record or 1 records: 「レコード ID」\
**状況：**&#x200B;トリガーが発生し、グループメールの場合など、同じレコードに複数回アクセスしようとする可能性があります。\
**トラブルシューティング手順：**&#x200B;再試行ロジックで処理する必要があります。それでも問題が解決しない場合は、Salesforce 管理者に問い合わせて、問題のあるトリガーのトラブルシューティングを依頼します。

**エラー：**UNKNOWN_EXCEPTION
**カテゴリ：**&#x200B;その他\
**メッセージ：** Unknown Exception occurred\
**状況：** Salesforce での未処理の例外。\
**トラブルシューティング手順：** Salesforce でケースを作成し、エラーメッセージに数値をコピーします。これは、Salesforce コードがエラーを適切に処理しないためです。
