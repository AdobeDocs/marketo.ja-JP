---
unique-page-id: 11378812
description: 顧客の選択 - Marketo ドキュメント - 製品ドキュメント
title: 顧客の選択
exl-id: 90da4ae0-0a12-48bd-8bae-a7431d2cf4f4
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: ht
source-wordcount: '585'
ht-degree: 100%

---

# 顧客の選択 {#discover-accounts}

「選択」オプションを使用して、ターゲットとなる可能性のある顧客を特定します。

## CRM 内の顧客から選択 {#discover-crm-accounts}

CRM からターゲットとなる可能性のある顧客を特定します。

>[!NOTE]
>
>CRM を Marketo TAM に接続した後、**CRM 内の顧客から選択**&#x200B;は、すべての CRM 顧客と関連情報を表示し、適切な重点顧客を選択するのに役立ちます。Marketo は、CRM から受け取った情報に加えて、情報を追加します。

**リード**（CRM 内の顧客から選択と Marketo 内の企業から選択）：連絡先とリードの両方が含まれます。リードは、Marketo の[リードと顧客の照合](/help/marketo/product-docs/target-account-management/target/named-accounts/lead-to-account-matching.md)を使用して検出できます。

**見込み顧客**（CRM 内の顧客から選択と Marketo 内の企業から選択）：CRM アカウントに属している可能性のある Marketo が見つけたリードの数を示します。

**カスタム CRM フィールド**（CRM 内の顧客から選択のみ）：これは、正しいターゲット顧客を選択するために、セールスとマーケティング組織を調整するのに役立ちます。[カスタム CRM フィールドを Marketo TAM とマッピング](/help/marketo/product-docs/target-account-management/setup-tam/create-a-custom-field-for-crm-discovery.md)すると、マッピングされたデータを表示して、ターゲット顧客を特定しやすくします。

1. 「重点顧客」で、「**新規作成**」ドロップダウンをクリックし、「**CRM 内の顧客から選択**」を選択します。

   ![](assets/disc-crm-one.png)

1. 新しいウィンドウ／タブが開きます。重点顧客に追加する CRM 顧客を選択し、「**次へ**」をクリックします。

   ![](assets/disc-crm-two.png)

1. プレビュー画面で、選択の量が確認されます。「**作成**」をクリックします。

   ![](assets/disc-three.png)

   以上です。

   ![](assets/disc-four.png)

## Marketo 内の企業から選択 {#discover-marketo-companies}

ターゲティングに適した会社を特定します。

>[!NOTE]
>
>Marketo 内の企業から選択では、CRM からではない Marketo 内の会社が表示されます。

1. 「重点顧客」で、**新規**&#x200B;ドロップダウンをクリックして、「**Marketo 内の企業から選択**」を選択します。

   ![](assets/one-1.png)

1. 新しいウィンドウ／タブが開きます。重点顧客に追加する会社を選択し、「**次へ**」をクリックします。

   ![](assets/disc-comp-two.png)

   >[!NOTE]
   >
   >Marketo 内の企業から選択と CRM 内の顧客から選択では、Marketo は自動的に次をおこないます。
   >
   >* Marketo データベースから、その会社がレコードに登録されているリードを検索します。一部の属性（業界など）に複数の値が表示される場合は、Marketo が個々のユーザーに対して異なる値のリストを見つけたことが原因です。ヒット数が最も多い属性が優先されます
   >
   >**CRM 内の顧客から選択**&#x200B;のみで、Marketo は自動的に次をおこないます。
   >
   >* CRM 連絡先を重点顧客と同期して関連付けます
   >
   >**Marketo 内の企業から選択**&#x200B;のみで、Marketo は自動的に次をおこないます。
   >
   >* ほとんどのインターネットサービスプロバイダーとパブリックドメイン（yahoo.com、gmail.com など）を会社名として除外します
   >
   >* CRM アカウントを重複排除します。1 つのレコードに「Acme」と「Acme Inc」（または Co、Corp、Corporation、Gmbh、Inc,、Incorporated、LLC、LLP、Ltd、PA、PC、PLLC、PLLC のサフィックスのいずれかが含まれる場合），TAM に単に「Acme」として統合します

   >
   >会社名ではなく CRM ID または顧客所有者で顧客の重複除外をおこないたい場合は、[Marketo サポート](https://nation.marketo.com/t5/Support/ct-p/Support)にお問い合わせください。

1. 重点顧客列の下にある下向き矢印をクリックすると、ドロップダウンが表示されます。

   ![](assets/disc-comp-three.png)

   >[!CAUTION]
   >
   >今後、選択した会社の新規リードは、それぞれの重点顧客に自動的に割り当てられます。これらの会社を再度確認し、正しい重点顧客に割り当てられていることを確認してください。

1. 既存のリードを選択するには、**重点顧客**&#x200B;ドロップダウンから目的の顧客を選択し、「**次へ**」をクリックします。

   ![](assets/disc-comp-four.png)

   また、ドロップダウンボックスに直接名前を入力して、重点顧客を新規作成することもできます。終了したらボックスから離れてクリックすると、

   ![](assets/disc-comp-five.png)

   新しい重点顧客が表示されます。その時点で、手順 4 のとおり、「**次へ**」をクリックします。

   ![](assets/disc-comp-six.png)

1. 「**作成**」をクリックします。

   ![](assets/disc-comp-seven.png)

   お疲れさまでした。

   ![](assets/disc-co-six.png)

>[!NOTE]
>
>選択した CRM アカウントと「CRM 内の顧客から選択」グリッドにある CRM 顧客の間に不一致がある場合は、次の 1 つ以上が原因である可能性があります。
>
>* 同様の名前を持つ異なる CRM 個王座が重複解除された
>* 次のスケジュールされた同期がまだ実行されていない


>[!MORELIKETHIS]
>
>[リードと顧客の照合](/help/marketo/product-docs/target-account-management/target/named-accounts/lead-to-account-matching.md)
