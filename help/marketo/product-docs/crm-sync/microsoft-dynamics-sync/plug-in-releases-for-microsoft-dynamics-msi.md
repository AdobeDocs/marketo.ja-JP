---
unique-page-id: 10099102
description: Microsoft Dynamics MSI 向けプラグインリリース - Marketo ドキュメント - 製品ドキュメント
title: Microsoft Dynamics MSI 向けプラグインリリース
exl-id: 830f7dc3-07fd-429b-b0fd-290ffdda88e6
feature: Microsoft Dynamics
source-git-commit: 6dcda9b86555c17b3492a02f3985db7d2acd8a32
workflow-type: tm+mt
source-wordcount: '400'
ht-degree: 42%

---

# Microsoft Dynamics MSI 向けプラグインリリース {#plug-in-releases-for-microsoft-dynamics-msi}

Microsoft Dynamics に初めて同期するときは、Marketo Sales Insight（MSI）用の最新バージョンのプラグインをダウンロードしてインストールします。Marketo Engageは定期的にこれらのプラグインを更新するので、同じ場所に戻って新しいバージョンをダウンロードできます。

Marketoのネイティブ CRM 同期ソリューションを Dynamics に使用している場合は、 [最新のプラグインのダウンロード](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md){target="_blank"} corresponding to your Dynamics release. For those who have a custom sync and have purchased Marketo Sales Insight, the [package is here](https://mktg-cdn.marketo.com/community/MarketoSalesInsight_NonNative.zip){target="_blank"}.

>[!NOTE]
>
>これらのバージョンは、Dynamics のオンプレミスバージョンとオンラインバージョンの両方で機能します。

## MSI ソリューションのアップグレード {#upgrading-your-msi-solution}

1. Dynamics の「_インポート_」ボタンを押して、Dynamics CRM の&#x200B;**[!UICONTROL 既存のバージョンに]**&#x200B;最新バージョンのソリューションをインポートします。

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-1.png)

>[!NOTE]
>
>例：Dynamics CRM のバージョンが 2.0.0.20 で、最新バージョンが 2.0.0.21 の場合は、2.0.0.20 _以降_&#x200B;のバージョンをインポートします。

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
   <td>02/14/24</td> 
   <td>2.00.31</td> 
   <td>匿名 Web アクティビティのページネーションに対する変更。
   <p>
   ユーザービューの秘密鍵情報を暗号化します。 暗号化を実行するには、新しいパッケージをインポートした後にパスワードを変更する必要があります。</td> 
  </tr>
  <tr> 
   <td>10/18/23</td> 
   <td>2.00.30</td> 
   <td>MSI エラーログを統合し、情報通知を削除してMarketo Error Entity に表示しない。</td> 
  </tr>
  <tr> 
   <td>05/19/23</td> 
   <td>2.00.29</td> 
   <td>グローバルダッシュボードの Web アクティビティと注目のアクションのページネーションの問題を修正しました。</td> 
  </tr>
  <tr> 
   <td>03/23/23</td> 
   <td>2.00.28</td> 
   <td>作成済み <a href="https://mktg-cdn.marketo.com/community/MarketoSalesInsight_NonNative.zip">新しいパッケージ</a> CRM への非ネイティブ接続用の MSI の場合。</td> 
  </tr>
  <tr> 
   <td>02/03/22</td> 
   <td>2.0.0.27</td> 
   <td>インサイトのアカウントレイアウト：注目のアクション、スコアの変更、Web アクティビティ、電子メールアクティビティ。</td> 
  </tr>
  <tr> 
   <td>01/05/22</td> 
   <td>2.0.0.26</td> 
   <td>送信メールのプログラム採用スコア。</td> 
  </tr>
  <tr> 
   <td>10/28/21</td> 
   <td>2.0.0.25</td> 
   <td>製品採用スコア指標、新しいグローバルダッシュボード（Web アクティビティ、E メール、ベストベット）。</td> 
  </tr>
  <tr> 
   <td>02/10/21</td> 
   <td>2.0.0.22</td> 
   <td>自動監査を削除し、MSI ソリューションに関するドキュメントの変更を削除します。</td> 
  </tr>
  <tr> 
   <td>10/01/20</td> 
   <td>2.0.0.21</td> 
   <td>バグ修正： Sales Insight の役割を持つユーザーに、MSI API 設定フィールドへのアクセス権を割り当てます。</td> 
  </tr> 
  <tr> 
   <td>2020/07/20</td> 
   <td>2.0.0.20</td> 
   <td>バグ修正：非同期レコードの検証メッセージを追加します。</td> 
  </tr> 
  <tr> 
   <td>2020/06/12</td> 
   <td>2.0.0.19</td> 
   <td>バグ修正： MSD API 設定で MSI シークレットパスワードを非表示にします。</td> 
  </tr> 
  <tr> 
   <td>2020/05/26</td> 
   <td>2.0.0.18</td> 
   <td>バグ修正： MSI ボタンを表示するための MSI ロール ID の検証を変更するには、次の手順を実行します。</td> 
  </tr> 
  <tr> 
   <td>2020/05/21</td> 
   <td>2.0.0.17</td> 
   <td>バグ修正：所有者フィールドの再表示と、フィールドの非必須化。</td> 
  </tr> 
  <tr> 
   <td>2020/04/28</td> 
   <td>2.0.0.16</td> 
   <td>バグ修正： MSD CRM サイトマップ設定のリンク依存関係を削除しています。</td> 
  </tr> 
 </tbody> 
</table>
