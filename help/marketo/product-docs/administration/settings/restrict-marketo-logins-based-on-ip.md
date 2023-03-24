---
unique-page-id: 2360297
description: IP に基づく Marketo ログインの制限 - Marketo ドキュメント - 製品ドキュメント
title: IP に基づく Marketo ログインの制限
exl-id: 5d9d0b88-b4bc-4e1b-b70c-2c2e7b4269f5
source-git-commit: bd6f049d5959356a99314e81bb6cfe517c2efdfa
workflow-type: ht
source-wordcount: '183'
ht-degree: 100%

---

# IP に基づく Marketo ログインの制限 {#restrict-marketo-logins-based-on-ip}

IP アドレスに基づいて、ユーザの Marketo へのアクセスを制限または有効にできます。手順は以下のとおりです。

>[!NOTE]
>
>**管理者権限が必要**

>[!NOTE]
>
>この記事の情報は、login.marketo.com での直接ログインにのみ適用されます。現時点では、シングルサインオン（SSO）ログインに IP 制限を適用することはできません。

1. 「**管理者**」領域に移動します。

   ![](assets/restrict-marketo-logins-based-on-ip-1.png)

1. 「**ログイン設定**」をクリックします。

   ![](assets/restrict-marketo-logins-based-on-ip-2.png)

1. 「**IP 制限を編集**」をクリックします。

   ![](assets/restrict-marketo-logins-based-on-ip-3.png)

1. 特定のアドレスを「**許可**」するまたは「**ブロック**」するかを選択し、「**保存**」をクリックします。

   >[!NOTE]
   >
   >**定義**
   >
   >* **許可済み IP アドレス**：許可済み IP アドレスの追加は包含的です。指定したすべての IP アドレスが含まれ、その他すべてが除外されます。
   >* **ブロック済み IP アドレス**：特定の IP が Marketo にアクセスするのを防ぎます。
   >* **IP 制限の無効化**：これをオンにすると、すべての制限ルールが機能を停止します。これはテスト目的で使用します。


   >[!NOTE]
   >
   >複数の制限を追加できますが、すべて許可されるか、すべてブロックされるかのいずれかとなります。許可済みとブロック済みを混在させて適合させることはできません。

   ![](assets/restrict-marketo-logins-based-on-ip-4.png)

   これで、マーケティングデータの安全性が今まで以上に向上しました。
