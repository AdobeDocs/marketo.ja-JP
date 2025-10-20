---
description: 最新のリリースノート - Marketo ドキュメント - 製品ドキュメント
title: 最新のリリースノート
hide: true
hidefromtoc: true
feature: Release Information
exl-id: 0ca5e844-c30b-4c86-a23d-d8f2c1bdddf5
source-git-commit: 7234082102356fc05c760f359ef19ca8cff375b5
workflow-type: tm+mt
source-wordcount: '538'
ht-degree: 86%

---

# リリースノート：2025年10月 {#release-notes-oct-25}

以下に、2025 年 10 月リリースに含まれるすべての機能を示します。 利用可能な機能については、お使いの Marketo Engage のエディションをご確認ください。

Adobe Dynamic Chat 専用のリリースノートについて詳しくは、[こちらを参照](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}してください。

>[!AVAILABILITY]
>
>星印（![星印](assets/yellow-star.png)）で示す機能は有償オプションです。詳しくは、Marketo Engage 担当営業にお問い合わせください。

## 標準リリースサイクルの機能 {#standard-release-cycle-features}

以下の機能は標準リリースサイクルに該当し、リリースは **2025年10月31日**（PT）から開始し、その次の週から残りの機能が段階的にロールアウトされます。リリースの機能と日付は変更される場合があります。各機能のステータスについては、各機能の隣で確認してください。

<table style="table-layout:auto">
 <tbody>
 <tr>
   <th style="width:65%">機能</th>
   <th style="width:10%">ステータス</th>
   <th style="width:25%">ドキュメント</th>
  </tr>
  <tr>
   <td><strong> タイトル </strong>：テキスト</td>
   <td><i>まもなくリリース</i></td>
   <td><i>まもなくリリース</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong> タイトル </strong>：テキスト</td>
   <td><i>まもなくリリース</i></td>
   <td><i>まもなくリリース</i></td>
  </tr>
  <tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong> タイトル </strong>：テキスト</td>
   <td><i>まもなくリリース</i></td>
   <td><i>まもなくリリース</i></td>
  </tr>
  <tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong> タイトル </strong>：テキスト</td>
   <td><i>まもなくリリース</i></td>
   <td><i>まもなくリリース</i></td>
  </tr>
  <tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
 <tr>
   <td><strong> タイトル </strong>：テキスト</td>
   <td><i>まもなくリリース</i></td>
   <td><i>まもなくリリース</i></td>
  </tr>
  <tr>
  </tbody>
</table>
<br/>

## お知らせ {#announcements}

* **REST API のダブルスラッシュの廃止**: 2025 年 9 月 16 日（PT）に、Adobeは、新しいテクノロジーを活用し、セキュリティと拡張性を強化した REST API URL 用のより新しいホスティングインフラストラクチャに移行しました。 サブスクリプションで、URL に 2 つのスラッシュ（//）を含む API を使用している場合は、次の手順について [ この国の POST](https://nation.marketo.com/t5/product-blogs/rest-api-double-slash-deprecation/ba-p/358616){target="_blank"} を参照してください。

* **新しい E メールデザイナーでの Velocity スクリプトへのスイッチバック**：Adobe Marketo Engage は今年 6 月、新しいメールデザイナー用に&#x200B;_条件付きコンテンツ_&#x200B;と呼ばれる機能をリリースしました。この機能は、動的コンテンツの柔軟性をもう少し高めるために、Velocity スクリプトではなく Handlebar スクリプトを利用していました。しかし、一部のトークンが正しく解決されないことが判明した場合は、一時的に無効にすることにしました。[詳細情報](https://nation.marketo.com/t5/product-blogs/update-on-email-scripting-in-the-new-email-designer/ba-p/358179){target="_blank"}

* **Marketo Engage ID の提供終了**：2025年8月に、Adobe は Marketo Engage ID のサポートの段階的な廃止を開始します（`login.marketo.com` 経由でのログイン）。Marketo Engage へのアクセスが中断されないようにするには、2025年9月30日（PT）までに [Adobe ID](https://experienceleague.adobe.com/ja/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview){target="_blank"} に移行する必要があります。

   * _IP 制限の廃止_：[IP に基づく Marketo ログインの制限](https://experienceleague.adobe.com/ja/docs/marketo/using/product-docs/administration/settings/restrict-marketo-logins-based-on-ip){target="_blank"}のサポートは、2025年7月30日（PT）に終了しました。この機能は、Adobe ID への移行が完了するまで有効です。Adobe Admin Console の Adobe ID 向けの新しい場所ベースのアクセス制御機能は、近日リリース予定です。

   * _シングルサインオン（SSO）の廃止_：[Marketo ID SSO](https://experienceleague.adobe.com/ja/docs/marketo/using/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal){target="_blank"} のサポートは、2025年7月30日（PT）に終了しました。この機能は、Adobe ID への移行が完了するまで有効です。Adobe Admin Console の Adobe ID 向けのシングルサインオンは個別に設定する必要があります。 設定手順について詳しくは、[ID とシングルサインオンの設定](https://helpx.adobe.com/jp/enterprise/using/set-up-identity.html){target="_blank"}を参照してください。

* **_友達に転送_機能の廃止**：2025年9月29日（PT）に、Marketo Engage 2.0 のメール（従来のメールエディター）の&#x200B;_友達に転送_&#x200B;機能は、すべてのサブスクリプションで完全に廃止されます。これは、トークンを使用して既に送信されている、または送信される予定のメール内の「友達に転送」トークンと「友達に転送」リンクに影響します。[詳細情報](https://nation.marketo.com/t5/product-blogs/deprecation-of-forward-to-a-friend/ba-p/358045#M2889){target="_blank"}

* **Rest API「access_token」パラメーターの廃止**：Marketo REST API 呼び出しの認証に使用される `access_token` クエリパラメーターは非推奨（廃止予定）となり、2026年1月31日（PT）以降は使用できなくなります。すべての新規および既存の統合では、「Authorization」ヘッダーを使用して REST API 呼び出しを認証する必要があります。[詳しくは、こちらを参照してください](https://experienceleague.adobe.com/ja/docs/marketo-developer/marketo/rest/authentication){target="_blank"}。

* **SOAP API の廃止**：Marketo SOAP API のサポートは、2026年1月31日（PT）に終了する予定です。SOAP API 機能を使用するサービスは、[REST API](https://experienceleague.adobe.com/ja/docs/marketo-developer/marketo/rest/rest-api){target="_blank"} に移行する必要があります。
