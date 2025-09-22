---
unique-page-id: 12615800
description: '[!UICONTROL 重点顧客]の読み込み - Marketo ドキュメント - 製品ドキュメント'
title: '[!UICONTROL 重点顧客]の読み込み'
exl-id: 3f40e567-9256-4efd-beea-4e818770759f
feature: Target Account Management
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '479'
ht-degree: 100%

---

# [!UICONTROL 重点顧客]の読み込み {#import-named-accounts}

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
   >「**[!UICONTROL ドメイン名別]**」を選択した場合は、「重点顧客」フィールドと「ドメイン」フィールドの両方を含める必要があります。

1. 重点顧客を追加するアカウントリストを選択するには、**[!UICONTROL アカウントリスト]**&#x200B;ドロップダウンリストから選択します。

   ![](assets/inafour.png)

   >[!NOTE]
   >
   >また、ドロップダウンボックスに名前を入力するだけで、新しい[!UICONTROL アカウントリスト]を作成することもできます。

1. 読み込みの通知を送信するには、**[!UICONTROL アラートの送信先]**&#x200B;ドロップダウンリストから、Marketo ユーザを選択します。メールアドレスを手動で入力することは&#x200B;_できません_。

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

[!UICONTROL アカウント名]で重複解除する場合のシナリオは、次のとおりです。

<table>
 <tbody>
  <tr>
   <td><strong>既存の<span class="uicontrol">重点顧客</span>名を持つレコードの読み込み</strong></td>
   <td><p>既存のレコードを更新</p></td>
  </tr>
  <tr>
   <td><strong>新しい<span class="uicontrol">重点顧客</span>名を持つレコードの読み込み</strong></td>
   <td>新しいレコードを作成</td>
  </tr>
 </tbody>
</table>

[!UICONTROL ドメイン名で]重複解除する場合のシナリオは、次のとおりです。

<table>
 <tbody>
  <tr>
   <td><strong>新しいアカウント名と新しいドメイン名を持つレコードの読み込み</strong></td>
   <td>提供された情報を使用して新しい<span class="uicontrol">重点顧客</span>を作成</td>
  </tr>
  <tr>
   <td><strong>既存のアカウント名と既存のドメイン名を持つレコードの読み込み</strong></td>
   <td>既存の<span class="uicontrol">重点顧客</span>を更新</td>
  </tr>
   <tr>
   <td><strong>新しいアカウント名と既存のドメイン名を持つレコードの読み込み</strong></td>
   <td>ドメイン名に一致する既存の<span class="uicontrol">重点顧客</span>に新しいアカウント名を付加し、その他の情報（業種、都道府県など）を更新</td>
  </tr>
  <tr>
   <td><strong>既存の<span class="uicontrol">重点顧客</span>名と新しいドメイン名を含むレコードの読み込み</strong></td>
   <td>アカウント名に一致する既存の<span class="uicontrol">重点顧客</span>に新しいドメイン名を付加し、その他の情報（業種、都道府県など）を更新</td>
  </tr>
 </tbody>
</table>

>[!NOTE]
>
>Marketo が重点顧客を付加する際、[!UICONTROL 重点顧客]に含まれる必要のある人物を識別できるルールが（バックグラウンドで）更新されます。例：「IBM」を「米国 IBM」に更新すると、どちらの会社名を持つ人物が[!UICONTROL 重点顧客]に関連付けられます。

Marketo が重複と見なすレコードを検出した場合は、最初のレコードのみが処理されます。
