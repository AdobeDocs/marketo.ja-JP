---
description: 最新のリリースノート - Marketo ドキュメント - 製品ドキュメント
title: 最新のリリースノート
hide: true
hidefromtoc: true
feature: Release Information
exl-id: 0ca5e844-c30b-4c86-a23d-d8f2c1bdddf5
source-git-commit: 29c1b59c9d2598626f546554a8bdc1b26b9e1590
workflow-type: tm+mt
source-wordcount: '494'
ht-degree: 51%

---

# リリースノート：2025年9月 {#release-notes-sep-25}

以下に、2025 年 9 月リリースに含まれるすべての機能を示します。 利用可能な機能については、お使いの Marketo Engage のエディションをご確認ください。

Adobe Dynamic Chat 専用のリリースノートについて詳しくは、[こちらを参照](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}してください。

>[!AVAILABILITY]
>
>星印（![星印](assets/yellow-star.png)）で示す機能は有償オプションです。詳しくは、Marketo Engage 担当営業にお問い合わせください。

## 標準リリースサイクルの機能 {#standard-release-cycle-features}

次の機能は標準リリースサイクルに従っており、**2025年9月19日（PT）**&#x200B;からリリースが開始され、その次の週から残りの機能が段階的にロールアウトされます。 リリースの機能と日付は変更される場合があります。各機能のステータスについては、各機能の隣で確認してください。

<table style="table-layout:auto">
 <tbody>
 <tr>
   <th style="width:65%">機能</th>
   <th style="width:10%">ステータス</th>
   <th style="width:25%">ドキュメント</th>
  </tr>
  <tr>
   <td><strong> オンデマンドのウェビナーアクティビティの保持 </strong>：インタラクティブウェビナーのユーザーは、30 日以上オンデマンドのウェビナーダッシュボードのデータを使用できるようになりました（以前は、ウェビナーの日から最大 30 日でした）。</td>
   <td><i>まもなくリリース</i></td>
   <td><i>まもなくリリース</i></td>
  </tr>
  </tbody>
</table>
<br/>

## お知らせ {#announcements}

* **新しいメールDesignerでの Velocity スクリプティングへの戻り**:Adobe Marketo Engageは今年 6 月、新しいメールDesigner用に _条件付きコンテンツ_ と呼ばれる機能をリリースしました。 この機能は、動的コンテンツの柔軟性をもう少し高めるために、Velocity スクリプティングではなく Handlebar スクリプティングを利用していました。 しかし、一部のトークンが正しく解決されないことが判明した場合は、一時的に無効にすることにしました。 [詳細情報](https://nation.marketo.com/t5/product-blogs/update-on-email-scripting-in-the-new-email-designer/ba-p/358179){target="_blank"}

* **Marketo Engage ID のサポート終了**: 2025 年 8 月、AdobeはMarketo Engage ID のサポートを段階的に廃止し始めました（`login.marketo.com` 経由でログイン）。 Marketo Engage へのアクセスが中断されないようにするには、2025年9月30日（PT）までに [Adobe ID](https://experienceleague.adobe.com/ja/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview){target="_blank"} に移行する必要があります。

   * _IP 制限の廃止_:[IP に基づくMarketo ログインの制限 ](https://experienceleague.adobe.com/ja/docs/marketo/using/product-docs/administration/settings/restrict-marketo-logins-based-on-ip){target="_blank"} のサポートは 2025 年 7 月 30 日（PT）に終了しました。 この機能は、Adobe ID への移行が完了するまで有効です。 Adobe Admin ConsoleのAdobe ID 用の新しい場所ベースのアクセス制御機能は、近日中に提供されます。

   * _シングルサインオン（SSO）の廃止_:[Marketo Identity SSO](https://experienceleague.adobe.com/ja/docs/marketo/using/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal){target="_blank"} のサポートは 2025 年 7 月 30 日（PT）に終了しました。 この機能は、Adobe ID への移行が完了するまで有効です。 Adobe Admin Console の Adobe ID 向けのシングルサインオンは個別に設定する必要があります。 設定手順について詳しくは、[ID とシングルサインオンの設定](https://helpx.adobe.com/jp/enterprise/using/set-up-identity.html){target="_blank"}を参照してください。

* **_フレンドに転送_ 機能の廃止**:2025 年 9 月 29 日（PT）に、Marketo Engage 2.0 のメール（従来のメールエディター）の _フレンドに転送_ 機能は、すべてのサブスクリプションで完全に廃止されます。 これは、既にトークンを使用して送信されている、または送信される予定のメール内の「友達に転送」トークンと「友達に転送」リンクに影響します。 [詳細情報](https://nation.marketo.com/t5/product-blogs/deprecation-of-forward-to-a-friend/ba-p/358045#M2889){target="_blank"}

* **Rest API「access_token」パラメーターの廃止**：Marketo REST API 呼び出しの認証に使用される `access_token` クエリパラメーターは非推奨（廃止予定）となり、2026年1月31日（PT）以降は使用できなくなります。すべての新規および既存の統合では、「Authorization」ヘッダーを使用して REST API 呼び出しを認証する必要があります。[詳しくは、こちらを参照してください](https://experienceleague.adobe.com/ja/docs/marketo-developer/marketo/rest/authentication){target="_blank"}。

* **SOAP API の廃止**：Marketo SOAP API のサポートは、2026年1月31日（PT）に終了する予定です。SOAP API 機能を使用するサービスは、[REST API](https://experienceleague.adobe.com/ja/docs/marketo-developer/marketo/rest/rest-api){target="_blank"} に移行する必要があります。
