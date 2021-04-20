---
unique-page-id: 11378812
description: Discoverアカウント —Marketoドキュメント — 製品ドキュメント
title: Discoverアカウント
exl-id: 90da4ae0-0a12-48bd-8bae-a7431d2cf4f4
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# アカウントの検出{#discover-accounts}

潜在的なターゲットアカウントを特定するには、Discoverオプションを使用します。

## CRM 内の顧客から選択 {#discover-crm-accounts}

CRMから潜在的なターゲットアカウントを特定します。

>[!NOTE]
>
>CRMをMarketoTAMに接続すると、**Discover CRM Accounts**&#x200B;にすべてのCRMアカウントと関連情報が表示され、適切な名前のアカウントを選択するのに役立ちます。 Marketoは、CRMから受け取った情報の上に追加情報を追加します。

**人** (Discover CRMアカウントおよびDiscoverMarketo会社内):連絡先とリードの両方が含まれます。リードは、Marketoの[リード対アカウントの照合](/help/marketo/product-docs/target-account-management/target/named-accounts/lead-to-account-matching.md)を使用して検出できます。

**推定ユーザー** (Discover CRMアカウントおよびDiscoverMarketo会社):MarketoがCRMアカウントに属している可能性があるリードを見つけた数を示します。

**カスタムCRMフィールド** （Discover CRMアカウントのみ）:これは、正しいターゲットアカウントを選択するために、販売およびマーケティング組織を調整するのに役立ちます。[カスタムCRMフィールド](/help/marketo/product-docs/target-account-management/setup-tam/create-a-custom-field-for-crm-discovery.md)をMarketoTAMとマッピングしたら、マッピングされたデータを表示して、ターゲットアカウントの特定に役立てます。

1. 「名前付きアカウント」で、**新規**&#x200B;ドロップダウンをクリックし、**CRMアカウントの検出**&#x200B;を選択します。

   ![](assets/disc-crm-one.png)

1. 新しいウィンドウ/タブが開きます。 指定したアカウントに追加するCRMアカウントを選択し、「**次へ**」をクリックします。

   ![](assets/disc-crm-two.png)

1. プレビュー画面で選択範囲の量が確認されます。 「**作成**」をクリックします。

   ![](assets/disc-three.png)

   それだけだ！

   ![](assets/disc-four.png)

## Marketo 内の企業から選択 {#discover-marketo-companies}

ターゲット設定に適した会社を特定する。

>[!NOTE]
>
>DiscoverのMarketo会社では、CRMに属していないMarketo会社が表示されます。

1. 「名前付きアカウント」で、「**新規**」ドロップダウンをクリックし、「**Marketo会社を検出**」を選択します。

   ![](assets/one-1.png)

1. 新しいウィンドウ/タブが開きます。 指定したアカウントに追加する会社を選択し、「**次へ**」をクリックします。

   ![](assets/disc-comp-two.png)

   >[!NOTE]
   >
   >DiscoverMarketo会社およびDiscover CRMでは、Marketoは自動的に次の処理を行います。
   >
   >* その会社をレコードに含むMarketoデータベースのユーザーを検索します。 一部の属性（業種など）に対して複数の値が表示される場合は、Marketoが個々の人に対して異なる値を見つけたためです。 ヒット数が最も多い属性が優先されます。
   >
   >**Discover CRM**&#x200B;のみで、Marketoは自動的に次の処理を行います。
   >
   >* CRM連絡先を指定されたアカウントと同期して関連付けます
   >
   >**Marketo会社**&#x200B;のみを発見すると、Marketoは自動的に次のように言う。
   >
   >* ほとんどのインターネットサービスプロバイダーとパブリックドメイン（yahoo.com、gmail.comなど）を会社名としてフィルター
      >
      >
   * CRMアカウントを重複排除しました。 1つのレコードに「Acme」と「Acme Inc」（または次のサフィックスのいずれか）が含まれる場合Co, Corp, Corporation, Gmbh, Inc, Incorporated, LLC, LLP, Ltd, PA, PC, PLC, PLLC)，単に「Acme」としてTAMに統合します。
   >
   >Marketoに会社名ではなくCRM IDまたはアカウント所有者による重複除外アカウントをお願いする場合は、[Marketoサポート](https://nation.marketo.com/t5/Support/ct-p/Support)にお問い合わせください。

1. 「アカウント名」列の下にある下向き矢印をクリックして、ドロップダウンを表示します。

   ![](assets/disc-comp-three.png)

   >[!CAUTION]
   >
   >今後、これらの選択した会社の新しいユーザーは、それぞれの名前付きアカウントに自動的に割り当てられます。 これらの会社を重複確認し、正しい名前付きアカウントに割り当てられていることを確認してください。

1. 既存のアカウントを選択するには、**名前付きアカウント**&#x200B;ドロップダウンをクリックし、目的のアカウントを選択して、**次へ**&#x200B;をクリックします。

   ![](assets/disc-comp-four.png)

   また、ドロップダウンボックスに目的の名前を直接入力して、新しい名前付きアカウントを作成することもできます。 終了したらボックスから離れる場所をクリックします。

   ![](assets/disc-comp-five.png)

   ...新しい指定されたアカウントが表示されます。 その時点で、手順4の「**次へ**」をクリックします。

   ![](assets/disc-comp-six.png)

1. 「**作成**」をクリックします。

   ![](assets/disc-comp-seven.png)

   お疲れさま！

   ![](assets/disc-co-six.png)

>[!NOTE]
>
>選択したCRMアカウントとDiscover CRMグリッド内のアカウントが一致しない場合は、次の原因と考えられます。
>
>* 重複を排除された類似の名前を持つ異なるCRMアカウントを持つ
>* 次のスケジュール済み同期はまだ実行されていません


>[!MORELIKETHIS]
>
>[顧客との照合を引き出す](/help/marketo/product-docs/target-account-management/target/named-accounts/lead-to-account-matching.md)
