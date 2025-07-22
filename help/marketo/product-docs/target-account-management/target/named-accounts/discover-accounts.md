---
unique-page-id: 11378812
description: 顧客の選択 - Marketo ドキュメント - 製品ドキュメント
title: 顧客の選択
exl-id: 90da4ae0-0a12-48bd-8bae-a7431d2cf4f4
feature: Target Account Management
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '558'
ht-degree: 66%

---

# 顧客の選択 {#discover-accounts}

「選択」オプションを使用して、ターゲットとなる可能性のある顧客を特定します。

## [!UICONTROL CRM アカウントの検出 &#x200B;] {#discover-crm-accounts}

CRM からターゲットとなる可能性のある顧客を特定します。

>[!NOTE]
>
>CRM を Marketo TAM に接続した後、**[!UICONTROL CRM 内の顧客から選択]**&#x200B;は、すべての CRM 顧客と関連情報を表示し、適切な重点顧客を選択するのに役立ちます。Marketo は、CRM から受け取った情報に加えて、情報を追加します。

**[!UICONTROL 人物]** （[!UICONTROL CRM アカウントを検出 &#x200B;] および [!UICONTROL Marketo会社を検出 &#x200B;]）：連絡先とリードの両方が含まれます。 リードは、Marketo の[リードと顧客の照合](/help/marketo/product-docs/target-account-management/target/named-accounts/lead-to-account-matching.md)を使用して検出できます。

**[!UICONTROL 見込み客]** （[!UICONTROL CRM アカウントを見つける &#x200B;] および [!UICONTROL Marketoの会社を見つける &#x200B;]）:CRM アカウントに属している可能性のある見込み客をMarketoが見つけた数を示します。

**カスタム CRM フィールド**（CRM 内の顧客から選択のみ）：これは、正しいターゲット顧客を選択するために、セールスとマーケティング組織を調整するのに役立ちます。[カスタム CRM フィールドを Marketo TAM とマッピング](/help/marketo/product-docs/target-account-management/setup-tam/create-a-custom-field-for-crm-discovery.md)すると、マッピングされたデータを表示して、ターゲット顧客を特定しやすくします。

1. [!UICONTROL &#x200B; 重点顧客 &#x200B;] で「**[!UICONTROL 新規]**」ドロップダウンをクリックし、「**[!UICONTROL CRM アカウントを検出]**」を選択します。

   ![](assets/disc-crm-one.png)

1. 新しいウィンドウ／タブが開きます。[!UICONTROL &#x200B; 重点顧客 &#x200B;] に追加する CRM アカウントを選択し、「次へ **[!UICONTROL をクリックし]** す。

   ![](assets/disc-crm-two.png)

1. プレビュー画面で、選択の量が確認されます。「**[!UICONTROL 作成]**」をクリックします。

   ![](assets/disc-three.png)

   以上です。

   ![](assets/disc-four.png)

## [!UICONTROL Marketoの会社を見つける &#x200B;] {#discover-marketo-companies}

ターゲティングに適した会社を特定します。

>[!NOTE]
>
>[!UICONTROL Marketo会社を確認 &#x200B;] には、CRM から来ていないMarketo会社が表示されます。

1. [!UICONTROL &#x200B; 重点顧客 &#x200B;] で「**[!UICONTROL 新規]**」ドロップダウンをクリックし、「**[!UICONTROL Marketo企業を確認]**」を選択します。

   ![](assets/one-1.png)

1. 新しいウィンドウ／タブが開きます。[!UICONTROL &#x200B; 重点顧客 &#x200B;] に追加する会社を選択し、**[!UICONTROL 次へ]** をクリックします。

   ![](assets/disc-comp-two.png)

   >[!NOTE]
   >
   >[!UICONTROL Marketoの会社を確認 &#x200B;] および CRM とMarketoを自動検出：
   >
   >* Marketo データベースから、その会社がレコードに登録されているリードを検索します。一部の属性（業界など）に複数の値が表示される場合は、Marketo が個々のユーザーに対して異なる値のリストを見つけたことが原因です。ヒット数が最も多い属性が優先されます
   >
   >**CRM 内の顧客から選択**&#x200B;のみで、Marketo は自動的に次をおこないます。
   >
   >* CRM 連絡先を同期して [!UICONTROL &#x200B; 指定アカウント &#x200B;] と関連付けます
   >
   >**[!UICONTROL Marketo 内の企業から選択]**&#x200B;のみで、Marketo は自動的に次をおこないます。
   >
   >* ほとんどのインターネットサービスプロバイダーとパブリックドメイン（yahoo.com、gmail.com など）を会社名として除外します
   >
   >* CRM アカウントを重複排除します。1 つのレコードに「Acme」と「Acme Inc」（または Co、Corp、Corporation、Gmbh、Inc,、Incorporated、LLC、LLP、Ltd、PA、PC、PLLC、PLLC のサフィックスのいずれかが含まれる場合），TAM に単に「Acme」として統合します

1. [!UICONTROL &#x200B; 名前付きアカウント &#x200B;] 列の下にある下向き矢印をクリックして、ドロップダウンを表示します。

   ![](assets/disc-comp-three.png)

   >[!CAUTION]
   >
   >今後、選択した会社の新規リードは、それぞれの重点顧客に自動的に割り当てられます。これらの会社を再確認し、正しい [!UICONTROL &#x200B; 指定アカウント &#x200B;] に割り当てられていることを確認してください。

1. 既存のリードを選択するには、**[!UICONTROL 重点顧客]**&#x200B;ドロップダウンから目的の顧客を選択し、「**[!UICONTROL 次へ]**」をクリックします。

   ![](assets/disc-comp-four.png)

   また、ドロップダウンボックスに目的の名前を直接入力して、新しい [!UICONTROL &#x200B; 名前付きアカウント &#x200B;] を作成するオプションもあります。 終了したらボックスから離れてクリックすると、

   ![](assets/disc-comp-five.png)

   新しい [!UICONTROL &#x200B; 指定アカウント &#x200B;] が表示されます。 その時点で、手順 4 のとおり、「**[!UICONTROL 次へ]**」をクリックします。

   ![](assets/disc-comp-six.png)

1. 「**[!UICONTROL 作成]**」をクリックします。

   ![](assets/disc-comp-seven.png)

   お疲れさまでした。

   ![](assets/disc-co-six.png)

>[!NOTE]
>
>選択した CRM アカウントと「CRM 内の顧客から選択」グリッドにある CRM 顧客の間に不一致がある場合は、次の 1 つ以上が原因である可能性があります。
>
>* 同様の名前を持つ異なる CRM アカウントが重複解除された
>* 次のスケジュールされた同期がまだ実行されていない

>[!MORELIKETHIS]
>
>[リードと顧客の照合](/help/marketo/product-docs/target-account-management/target/named-accounts/lead-to-account-matching.md)
