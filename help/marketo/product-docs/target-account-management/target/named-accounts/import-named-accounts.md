---
unique-page-id: 12615800
description: '[!UICONTROL &#x200B; 指定アカウント &#x200B;] の読み込み – Marketo ドキュメント – 製品ドキュメント'
title: インポート [!UICONTROL &#x200B; 重点顧客 &#x200B;]
exl-id: 3f40e567-9256-4efd-beea-4e818770759f
feature: Target Account Management
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '479'
ht-degree: 57%

---

# インポート [!UICONTROL &#x200B; 重点顧客 &#x200B;] {#import-named-accounts}

ターゲット顧客の候補がいっぱいの CSV を既にお持ちの場合、TAM に直接読み込むことができます。

1. **[!UICONTROL 新規作成]**&#x200B;ドロップダウンをクリックして「**[!UICONTROL 重点顧客を読み込む]**」を選択します。

   ![](assets/inaone.png)

1. 新しいウィンドウが開きます。「**[!UICONTROL 参照]**」をクリックし、読み込む重点顧客ファイルを選択します。

   ![](assets/inatwo.png)

   >[!TIP]
   >
   >ファイルで、[可能な限り多くの情報](/help/marketo/product-docs/target-account-management/target/named-accounts/named-account-overview.md#named-account-attributes)を提供します。追加できるのはファーモグラフィック情報のみです。Marketo が計算するもの（パイプライン）は追加できません。CRM 顧客に基づく重点顧客を作成するには、CRM から顧客名と CRM ID を CSV ファイルに書き出し、「顧客名」オプションを使用して、読み込みプロセス中に CRM ID をマッピングします。CRM 顧客を特定の顧客に適切にリンクするには、CRM 顧客の正確な名前を指定する必要があります。

1. 顧客名またはドメイン名の 2 つの重複解除モードから選択します。この例では、顧客を選択します。**[!UICONTROL モード]**&#x200B;ドロップダウンをクリックして、「**[!UICONTROL 顧客名別]**」を選択します。

   ![](assets/inathree.png)

   >[!NOTE]
   >
   >**[!UICONTROL ドメイン名別]** を選択する場合は、指定アカウントとドメインの両方のフィールドを含める必要があります。

1. 重点顧客を追加する顧客リストを選択するには、**[!UICONTROL 顧客リスト]**&#x200B;ドロップダウンリストから選択します。

   ![](assets/inafour.png)

   >[!NOTE]
   >
   >また、ドロップダウンボックスに名前を入力するだけで、新しい [!UICONTROL &#x200B; アカウントリスト &#x200B;] を作成できます。

1. 読み込みの通知を送信するには、**[!UICONTROL アラートの送信先]**&#x200B;ドロップダウンリストから、Marketo ユーザーを選択します。メールアドレスを手動で入力することは&#x200B;_できません_。

   ![](assets/inafive-2.png)

1. 「**[!UICONTROL 次へ]**」をクリックします。

   ![](assets/inasix-2.png)

1. 各フィールドをマッピングするには、**[!UICONTROL Marketo フィールド]**&#x200B;ドロップダウンから、適切なフィールドを選択します。終了したら「**[!UICONTROL 次へ]**」をクリックします。

   ![](assets/inaseven.png)

   成功

   ![](assets/inanine.png)

   >[!NOTE]
   >
   >「インポートステータスを確認」では、最近の 3 日間のアクティビティのみが表示されます。

[!UICONTROL &#x200B; アカウント名 &#x200B;] による重複排除のシナリオ：

<table> 
 <tbody> 
  <tr> 
   <td><strong>既存の <span class="uicontrol"> 名前付きアカウント </span> 名を使用したレコードのインポート</strong></td> 
   <td><p>既存のレコードをアップデート</p></td> 
  </tr> 
  <tr> 
   <td><strong>新しい <span class="uicontrol"> 指定顧客 </span> 名でのレコードのインポート</strong></td> 
   <td>新しいレコードを作成</td> 
  </tr> 
 </tbody> 
</table>

[!UICONTROL &#x200B; ドメイン名 &#x200B;] による重複排除のシナリオ：

<table> 
 <tbody> 
  <tr> 
   <td><strong>新しい顧客名と新しいドメイン名を持つレコードの読み込み</strong></td> 
   <td>指定した情報で新しい <span class="uicontrol"> 指定アカウント </span> が作成されます</td> 
  </tr> 
  <tr> 
   <td><strong>既存の顧客名と既存のドメイン名を持つレコードの読み込み</strong></td> 
   <td>既存の <span class="uicontrol"> 指定アカウント </span> を更新します</td> 
  </tr> 
   <tr> 
   <td><strong>新しい顧客名と既存のドメイン名を持つレコードの読み込み</strong></td> 
   <td>ドメイン名と一致する既存の <span class="uicontrol"> 指定アカウント </span> に新しいアカウント名を追加し、その他の情報（業界、州など）を更新します</td> 
  </tr> 
  <tr> 
   <td><strong>既存の <span class="uicontrol"> 名前付きアカウント </span> 名および新しいドメイン名を持つレコードのインポート</strong></td> 
   <td>アカウント名と一致する既存の <span class="uicontrol"> 指定アカウント </span> に新しいドメイン名を追加し、その他の情報（業界、州など）を更新します</td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Marketoが名前付きアカウントを追加する際に、その [!UICONTROL &#x200B; 名前付きアカウント &#x200B;] の一部である必要があるユーザーを特定できるようにするルールを（バックグラウンドで）更新しています。 例：「IBM」を「IBM, USA」に更新すると、どちらかの会社名を持つ人物が [!UICONTROL &#x200B; 特定のアカウント &#x200B;] に関連付けられます。

Marketo が重複と見なすレコードを検出した場合は、最初のレコードのみが処理されます。
