---
unique-page-id: 10099102
description: ' [!DNL Microsoft Dynamics]  MSI 向けプラグインリリース - Marketo ドキュメント - 製品ドキュメント'
title: ' [!DNL Microsoft Dynamics]  MSI 向けプラグインリリース'
exl-id: 830f7dc3-07fd-429b-b0fd-290ffdda88e6
feature: Microsoft Dynamics
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '403'
ht-degree: 100%

---

# [!DNL Microsoft Dynamics] MSI 向けプラグインリリース {#plug-in-releases-for-microsoft-dynamics-msi}

[!DNL Microsoft Dynamics] に初めて同期するときは、Marketo セールスインサイト（MSI）用の最新バージョンのプラグインをダウンロードしてインストールします。Marketo は定期的にこれらのプラグインを更新するので、同じ場所に戻って新しいバージョンをダウンロードできます。

Marketo のネイティブ CRM 同期ソリューションを [!DNL Dynamics] に使用している場合は、お使いの [!DNL Dynamics] リリースに対応した、[最新のプラグインをダウンロード](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md){target="_blank"}してください。カスタム同期を持ち、Marketo セールスインサイトを購入しているユーザの場合、[パッケージはこちらです](https://mktg-cdn.marketo.com/community/MarketoSalesInsight_NonNative.zip){target="_blank"}。

>[!NOTE]
>
>これらのバージョンは、[!DNL Dynamics] のオンプレミスバージョンとオンラインバージョンの両方で機能します。

## MSI ソリューションのアップグレード {#upgrading-your-msi-solution}

1. [!DNL Dynamics] の「**[!UICONTROL インポート]**」ボタンを押して、[!DNL Dynamics] CRM の&#x200B;_既存のバージョンに対して_&#x200B;ソリューションの最新バージョンを読み込みます。

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-1.png)

>[!NOTE]
>
>例：[!DNL Dynamics] CRM のバージョンが 2.0.0.20 で、最新バージョンが 2.0.0.21 の場合は、2.0.0.20 _以降_&#x200B;のバージョンを読み込みます。

1. 「**[!UICONTROL 次へ]**」をクリックします。

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-2.png)

1. 「**[!UICONTROL アップグレードのステージ]**」および「**[!UICONTROL カスタマイズを維持]**」を選択し、「**[!UICONTROL インポート]**」をクリックします。

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-3.png)

1. 「**[!UICONTROL 次へ]**」をクリックします。

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-4.png)

1. インポートが正常に完了すると、MarketoSalesInsight と MarketoSalesInsight_Upgrade の 2 つの MSI ソリューションが表示されます。古いソリューションを選択し、「ソリューションアップグレードを適用」をクリックします。

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-5.png)

これで完了です。アップグレード後は、1 つの MSI ソリューションのみが表示されます。

## バージョンの更新 {#version-updates}

<table>
 <tbody>
  <tr>
   <th>リリース日</th>
   <th>バージョン</th>
   <th>注意</th>
  </tr>
  <tr>
   <td>2024年2月14日（PT）</td>
   <td>2.00.31</td>
   <td>匿名 web アクティビティのページネーションに変更します。
   <p>
   ユーザビューから秘密鍵の情報を暗号化します。暗号化を実行するには、新しいパッケージの読み込み後にパスワードを変更する必要があります。</td>
  </tr>
  <tr>
   <td>2023年10月18日（PT）</td>
   <td>2.00.30</td>
   <td>MSI エラーログを統合し、情報通知を削除すると、Marketo エラーエンティティに表示されません。</td>
  </tr>
  <tr>
   <td>2023年5月19日（PT）</td>
   <td>2.00.29</td>
   <td>グローバルダッシュボードの web アクティビティと注目のアクションのページネーションの問題を修正しました。</td>
  </tr>
  <tr>
   <td>2023年3月23日（PT）</td>
   <td>2.00.28</td>
   <td>CRM への非ネイティブ接続用に MSI 用の<a href="https://mktg-cdn.marketo.com/community/MarketoSalesInsight_NonNative.zip">新しいパッケージ</a>を作成しました。</td>
  </tr>
  <tr>
   <td>2022年2月3日（PT）</td>
   <td>2.0.0.27</td>
   <td>インサイトのアカウントレイアウト：注目のアクション、スコアの変更、web アクティビティ、メールアクティビティ。</td>
  </tr>
  <tr>
   <td>2022年1月5日（PT）</td>
   <td>2.0.0.26</td>
   <td>メール送信用のプログラム採用スコア。</td>
  </tr>
  <tr>
   <td>2021年10月28日（PT）</td>
   <td>2.0.0.25</td>
   <td>製品採用スコア指標、新しいグローバルダッシュボード（web アクティビティ、メール、最有望見込客）。</td>
  </tr>
  <tr>
   <td>2021年2月10日（PT）</td>
   <td>2.0.0.22</td>
   <td>MSI ソリューションの自動監査の有効化とドキュメントの変更を削除します。</td>
  </tr>
  <tr>
   <td>2020年10月1日（PT）</td>
   <td>2.0.0.21</td>
   <td>バグ修正：セールスインサイトのロールを持つユーザの MSI API 設定フィールドへのアクセスの割り当て。</td>
  </tr>
  <tr>
   <td>2020/07/20</td>
   <td>2.0.0.20</td>
   <td>バグ修正：非同期レコードの検証メッセージを追加。</td>
  </tr>
  <tr>
   <td>2020/06/12</td>
   <td>2.0.0.19</td>
   <td>バグ修正：MSD API 設定で MSI 秘密鍵パスワードを非表示に。</td>
  </tr>
  <tr>
   <td>2020/05/26</td>
   <td>2.0.0.18</td>
   <td>バグ修正：「MSI」ボタンを表示するために MSI ロール ID の検証を変更。</td>
  </tr>
  <tr>
   <td>2020/05/21</td>
   <td>2.0.0.17</td>
   <td>バグ修正：所有者フィールドを再表示し、フィールドを必須にしないように設定。</td>
  </tr>
  <tr>
   <td>2020/04/28</td>
   <td>2.0.0.16</td>
   <td>バグ修正：MSD CRM サイトマップ設定のリンク依存関係を削除。</td>
  </tr>
 </tbody>
</table>
