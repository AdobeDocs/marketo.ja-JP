---
description: 最新のリリースノート - Marketo ドキュメント - 製品ドキュメント
title: 最新のリリースノート
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
feature: Release Information
source-git-commit: dda635ffac84c76eb60ecac395707914c4902c9d
workflow-type: tm+mt
source-wordcount: '730'
ht-degree: 91%

---

# リリースノート：2025年10月 {#release-notes-oct-25}

以下に、2025年10月リリースに含まれるすべての機能を示します。利用可能な機能については、お使いの Marketo Engage のエディションをご確認ください。

Adobe Dynamic Chat 専用のリリースノートについて詳しくは、[こちらを参照](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}してください。

>[!AVAILABILITY]
>
>星印（![星印](assets/yellow-star.png)）で示す機能は有償オプションです。詳しくは、Marketo Engage 担当営業にお問い合わせください。

## 標準リリースサイクルの機能 {#standard-release-cycle-features}

以下の機能は標準リリースサイクルに従い、**2025年10月31日**（PT）からリリースを開始し、その次の週から残りの機能が段階的にロールアウトされます。リリースの機能と日付は変更される場合があります。各機能のステータスについては、各機能の隣で確認してください。

<table style="table-layout:auto">
 <tbody>
 <tr>
   <th style="width:65%">機能</th>
   <th style="width:10%">ステータス</th>
   <th style="width:25%">ドキュメント</th>
  </tr>
  <tr>
   <td><strong> メールDesigner - テンプレートインポーター </strong>：クラシックメールエディターからメールテンプレートを読み込んで、Design Studio の新規メールDesignerと互換性のあるテンプレートを作成します。</td>
   <td><i>まもなくリリース</i></td>
   <td><i>まもなくリリース</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>E メールデザイナー - 条件付きコンテンツ</strong>：新しい E メールデザイナーのパリティ機能により、トークン以外でもメールのパーソナライゼーションを実現できます。</td>
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
   <td><strong>E メールデザイナー - A/B テスト</strong>：新しい E メールデザイナーのパリティ機能により、A/B テストを実行して、最適な応答を受信するコンテンツのタイプを確認できます。</td>
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
   <td><strong>E メールデザイナー - ブランドテーマ</strong>：Marketo Engage 内でブランドテーマを定義できるようになりました。スタイル設定は、ブランドの一貫性を確保するために、メールテンプレートやその他のメールアセットをまたいで再利用および適用できます。</td>
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
   <td><strong>E メールデザイナー - 画像から HTML へのコンバーター</strong>：あるメールの互換 PNG／JPEG 画像ファイルをアップロードすると、HTML へと自動的に変換され、新しい E メールデザイナーできるようになります。</td>
   <td><i>まもなくリリース</i></td>
   <td><i>まもなくリリース</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>E メールデザイナー - メールを複製アクション</strong>：マーケティングアクティビティでメールを別のプログラムフォルダーに複製し、既存のメールをすばやく再利用できるようになりました。</td>
   <td><i>まもなくリリース</i></td>
   <td><i>まもなくリリース</i></td>
  </tr>
  </tbody>
</table>
<br/>

## お知らせ {#announcements}

* **Salesforce CRM 統合のアップグレード**：新しいバージョンのネイティブ CRM 統合が、2025 年 11 月 13 日（PT）から 7 日間、ネイティブコネクタが有効になっているアクティブなサンドボックスにデプロイされます。 詳細は [ この民族の投稿 ](https://nation.marketo.com/t5/product-blogs/salesforce-crm-integration-upgrade/ba-p/358702){target="_blank"} で確認する

* **REST API 二重スラッシュの廃止**：2025年9月16日（PT）に、アドビでは、セキュリティとスケーラビリティを追加した、新しいテクノロジーを活用した REST API URL 用のより最新のホスティングインフラストラクチャに移行しました。サブスクリプションで URL に二重スラッシュ（//）が含まれる API を使用している場合は、次の手順について[この Nation の投稿](https://nation.marketo.com/t5/product-blogs/rest-api-double-slash-deprecation/ba-p/358616){target="_blank"}を参照してください。

* **新しい E メールデザイナーでの Velocity スクリプトへのスイッチバック**：Adobe Marketo Engage は今年 6 月、新しいメールデザイナー用に&#x200B;_条件付きコンテンツ_&#x200B;と呼ばれる機能をリリースしました。この機能は、動的コンテンツの柔軟性をもう少し高めるために、Velocity スクリプトではなく Handlebar スクリプトを利用していました。しかし、一部のトークンが正しく解決されないことが判明した場合は、一時的に無効にすることにしました。[詳細情報](https://nation.marketo.com/t5/product-blogs/update-on-email-scripting-in-the-new-email-designer/ba-p/358179){target="_blank"}

* **Marketo Engage ID の提供終了**：2025年8月に、Adobe は Marketo Engage ID のサポートの段階的な廃止を開始します（`login.marketo.com` 経由でのログイン）。Marketo Engage へのアクセスが中断されないようにするには、2025年9月30日（PT）までに [Adobe ID](https://experienceleague.adobe.com/ja/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview){target="_blank"} に移行する必要があります。

   * _IP 制限の廃止_：[IP に基づく Marketo ログインの制限](https://experienceleague.adobe.com/ja/docs/marketo/using/product-docs/administration/settings/restrict-marketo-logins-based-on-ip){target="_blank"}のサポートは、2025年7月30日（PT）に終了しました。この機能は、Adobe ID への移行が完了するまで有効です。Adobe Admin Console の Adobe ID 向けの新しい場所ベースのアクセス制御機能は、近日リリース予定です。

   * _シングルサインオン（SSO）の廃止_：[Marketo ID SSO](https://experienceleague.adobe.com/ja/docs/marketo/using/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal){target="_blank"} のサポートは、2025年7月30日（PT）に終了しました。この機能は、Adobe ID への移行が完了するまで有効です。Adobe Admin Console の Adobe ID 向けのシングルサインオンは個別に設定する必要があります。 設定手順について詳しくは、[ID とシングルサインオンの設定](https://helpx.adobe.com/jp/enterprise/using/set-up-identity.html){target="_blank"}を参照してください。

* **_友達に転送_機能の廃止**：2025年9月29日（PT）に、Marketo Engage 2.0 のメール（従来のメールエディター）の&#x200B;_友達に転送_&#x200B;機能は、すべてのサブスクリプションで完全に廃止されました。この廃止は、トークンを使用して既に送信されている、または送信されるようにスケジュールされたメール内の「友達に転送」トークンと「友達に転送」リンクに影響しました。[詳細情報](https://nation.marketo.com/t5/product-blogs/deprecation-of-forward-to-a-friend/ba-p/358045#M2889){target="_blank"}

* **Rest API「access_token」パラメーターの廃止**：Marketo REST API 呼び出しの認証に使用される `access_token` クエリパラメーターは非推奨（廃止予定）となり、2026年1月31日（PT）以降は使用できなくなります。すべての新規および既存の統合では、「Authorization」ヘッダーを使用して REST API 呼び出しを認証する必要があります。[詳しくは、こちらを参照してください](https://experienceleague.adobe.com/ja/docs/marketo-developer/marketo/rest/authentication){target="_blank"}。

* **SOAP API の廃止**：Marketo SOAP API のサポートは、2026年1月31日（PT）に終了する予定です。SOAP API 機能を使用するサービスは、[REST API](https://experienceleague.adobe.com/ja/docs/marketo-developer/marketo/rest/rest-api){target="_blank"} に移行する必要があります。
