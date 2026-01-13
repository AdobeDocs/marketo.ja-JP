---
description: 最新のリリースノート - Marketo ドキュメント - 製品ドキュメント
title: 最新のリリースノート
hide: true
hidefromtoc: true
feature: Release Information
exl-id: 0ca5e844-c30b-4c86-a23d-d8f2c1bdddf5
source-git-commit: c6b8dd17c4337b32c6bb4f0a1b9ce22c1e3b8715
workflow-type: tm+mt
source-wordcount: '452'
ht-degree: 62%

---

# リリースノート：2026年1月 {#release-notes-jan-26}

以下に、2026 年 1 月リリースに含まれるすべての機能を示します。 利用可能な機能については、お使いの Marketo Engage のエディションをご確認ください。

Adobe Dynamic Chat 専用のリリースノートについて詳しくは、[こちらを参照](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}してください。

>[!AVAILABILITY]
>
>星印（![星印](assets/yellow-star.png)）で示す機能は有償オプションです。詳しくは、Marketo Engage 担当営業にお問い合わせください。

## 標準リリースサイクルの機能 {#standard-release-cycle-features}

次の機能は標準リリースサイクルに該当し、リリースは **2026年1月30日（PT）**&#x200B;から開始し、その次の週から残りの機能が段階的にロールアウトされます。リリースの機能と日付は変更される場合があります。各機能のステータスについては、各機能の隣で確認してください。

<table style="table-layout:auto">
 <tbody>
 <tr>
   <th style="width:65%">機能</th>
   <th style="width:10%">ステータス</th>
   <th style="width:25%">ドキュメント</th>
  </tr>
  <tr>
   <td><strong> 機能タイトル </strong>：機能の説明。</td>
   <td><i>まもなくリリース</i></td>
   <td><i>まもなくリリース</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong> 機能タイトル </strong>：機能の説明。</td>
   <td><i>まもなくリリース</i></td>
   <td><i>まもなくリリース</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong> 機能タイトル </strong>：機能の説明。</td>
   <td><i>まもなくリリース</i></td>
   <td><i>まもなくリリース</i></td>
  </tr>
  </tbody>
</table>
<br/>

## Adobe Connectの機能 {#adobe-connect-features}

これらの機能は、Adobe Connect チームによって既にリリースされています。 Marketo Engage[&#x200B; インタラクティブウェビナー &#x200B;](https://experienceleague.adobe.com/ja/docs/marketo/using/product-docs/demand-generation/events/interactive-webinars/interactive-webinars-overview){target="_blank"} は、Adobe Connectを活用しています。 したがって、以下の機能は、インタラクティブウェビナーのユーザーにのみ適用されます。

* **調査ポッド**:Adobe Connect 12.11 では、構造化されたフィードバックフォームをホストがライブセッション内で直接設計して配信できる新しい調査ポッドが導入されました。

* **リソースポッド**：新しいリソースポッドは、以前の「ファイル」ポッドと「web リンク」ポッドに代わるものであり、ライブセッション中にリソースを共有するための単一の統一された方法を提供します。

* **Enhanced Room Interface Experience**:Adobe Connect 12.11 は、Creative CloudやExperience Cloudなどの他のAdobe製品で使用されているビジュアル言語と連携して、Adobeの最新の Spectrum 2 デザインフレームワークに基づいて構築された、新しくより現代的なルームインターフェイスを導入しました。

詳しくは、[Adobe Connect 12.11 リリースノート &#x200B;](https://helpx.adobe.com/jp/adobe-connect/release-note/adobe-connect-12-11-release-notes.html){target="_blank"} を参照してください。

## お知らせ {#announcements}

* **Rest API「access_token」パラメーターの廃止**：Marketo REST API 呼び出しの認証に使用される `access_token` クエリパラメーターは非推奨（廃止予定）となり、2026年3月31日（PT）以降は使用できなくなります。すべての新規および既存の統合では、「Authorization」ヘッダーを使用して REST API 呼び出しを認証する必要があります。[詳しくは、こちらを参照してください](https://experienceleague.adobe.com/ja/docs/marketo-developer/marketo/rest/authentication){target="_blank"}。

* **SOAP API の廃止**：Marketo SOAP API のサポートは、2026年3月31日（PT）に終了する予定です。SOAP API 機能を使用するサービスは、[REST API](https://experienceleague.adobe.com/ja/docs/marketo-developer/marketo/rest/rest-api){target="_blank"} に移行する必要があります。

* **Marketo Engage Id の提供終了**:

   * _IP 制限の廃止_：[IP に基づく Marketo ログインの制限](https://experienceleague.adobe.com/ja/docs/marketo/using/product-docs/administration/settings/restrict-marketo-logins-based-on-ip){target="_blank"}のサポートは、2025年7月30日（PT）に終了しました。この機能は、Adobe ID への移行が完了するまで有効です。Adobe Admin Console の Adobe ID 向けの新しい場所ベースのアクセス制御機能は、近日リリース予定です。

   * _シングルサインオン（SSO）の廃止_：[Marketo ID SSO](https://experienceleague.adobe.com/ja/docs/marketo/using/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal){target="_blank"} のサポートは、2025年7月30日（PT）に終了しました。この機能は、Adobe ID への移行が完了するまで有効です。Adobe Admin Console の Adobe ID 向けのシングルサインオンは個別に設定する必要があります。 設定手順について詳しくは、[ID とシングルサインオンの設定](https://helpx.adobe.com/jp/enterprise/using/set-up-identity.html){target="_blank"}を参照してください。
