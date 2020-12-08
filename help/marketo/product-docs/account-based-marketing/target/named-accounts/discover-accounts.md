---
unique-page-id: 11378812
description: Discoverアカウント — Marketto Docs — 製品ドキュメント
title: Discoverアカウント
translation-type: tm+mt
source-git-commit: c8a77dc84c023e05fbb442f575269aac108ffb29
workflow-type: tm+mt
source-wordcount: '601'
ht-degree: 0%

---


# Discoverアカウント {#discover-accounts}

潜在的なターゲットアカウントを特定するには、Discoverオプションを使用します。

## CRMアカウントの検出 {#discover-crm-accounts}

CRMから潜在的なターゲットアカウントを特定します。

>[!NOTE]
>
>CRMをMarketto ABMに接続すると、 **Discover CRMアカウント** には、すべてのCRMアカウントと関連情報が表示され、適切な名前のアカウントを選択するのに役立ちます。 Marketorは、CRMから受け取った情報の上に、追加情報を追加します。

**人** (Discover CRMアカウントおよびDiscover Marketto会社):連絡先とリードの両方が含まれます。 リードは、Marketoのリード・ト [ー・アカウントの照合を使用して検出できます](http://docs.marketo.com/display/DOCS/Lead+to+Account+Matching)。 **推定ユーザー** (Discover CRMアカウントおよびDiscover Marketto会社):CRMアカウントに属している可能性があるリードを見つけたリード数を示します。

**カスタムCRMフィールド** （Discover CRMアカウントのみ）:これは、正しいターゲットアカウントを選択するために、販売およびマーケティング組織を調整するのに役立ちます。 Marketo ABMでカスタムCRMフィールド [を](http://docs.marketo.com/x/1wnG) マッピングしたら、マッピングされたデータを表示して、ターゲットアカウントの特定に役立てます。

1. 「固有のアカウント」で、 **新規** 」ドロップダウンをクリックし、「 **Discover CRM Accounts**」を選択します。

   ![](assets/disc-crm-one.png)

1. 新しいウィンドウ/タブが開きます。 指定されたアカウントに追加するCRMアカウントを選択し、「 **次へ**」をクリックします。

   ![](assets/disc-crm-two.png)

1. プレビュー画面で選択範囲の量が確認されます。 「 **作成**」をクリックします。

   ![](assets/disc-three.png)

   それだけだ！

   ![](assets/disc-four.png)

## Discover Marketto会社 {#discover-marketo-companies}

ターゲット設定に適した会社を特定する。

>[!NOTE]
>
>Discover Marketto会社には、CRMから来ていないマーケティング会社が表示されます。

1. 「固有のアカウント」で、 **新規** 」ドロップダウンをクリックし、「 **Discover Markettor会社**」を選択します。

   ![](assets/one-1.png)

1. 新しいウィンドウ/タブが開きます。 指定したアカウントに追加する会社を選択し、「 **次へ**」をクリックします。

   ![](assets/disc-comp-two.png)

   >[!NOTE]
   >
   >Discover Marketto会社とDiscover CRMでは、Marketorは自動的に次のように処理します。
   >
   > * レコードにその会社が含まれているユーザーを、Marketoデータベースから検索します。 一部の属性（業界など）に複数の値が表示される場合は、それらの個々の訪問者に対して異なる値がリストに表示されていたためです。 ヒット数が最も多い属性が優先されます。
   >
   >Discover **CRMのみ** 、Marketorは自動的に次の操作を行います。
   >
   > * CRM連絡先を指定されたアカウントと同期して関連付けます
   >
   >Discover Markettor会社 **のみ** 、Marketorは自動的に次の操作を行います。
   >
   > * ほとんどのインターネットサービスプロバイダーとパブリックドメイン( [Yahoo.com](https://yahoo.com)、 [Gmail.comなど](https://gmail.com))を会社名としてフィルター
      >
      > 
   * CRMアカウントを重複排除しました。 1つのレコードに「Acme」と「Acme Inc」（または次のサフィックスのいずれか）が含まれる場合Co, Corp, Corporation, Gmbh, Inc, Incorporated, LLC, LLP, Ltd, PA, PC, PLC, PLLC)の場合、ABM内で単に「Acme」として統合します。
   >
   >会社名ではなくCRM IDまたはアカウント所有者によってアカウントの重複除外を行う場合は、 [マーケティング担当者にお問い合わせください](https://nation.marketo.com/t5/Support/ct-p/Support)。

1. 「アカウント名」列の下にある下向き矢印をクリックして、ドロップダウンを表示します。

   ![](assets/disc-comp-three.png)

   >[!CAUTION]
   >
   >今後、これらの選択した会社の新しいユーザーは、それぞれの名前付きアカウントに自動的に割り当てられます。 これらの会社を重複確認し、正しい名前付きアカウントに割り当てられていることを確認してください。

1. 既存のアカウントを選択するには、「 **指定アカウント** 」ドロップダウンをクリックし、目的のアカウントを選択して「 **次へ**」をクリックします。

   ![](assets/disc-comp-four.png)

   また、ドロップダウンボックスに目的の名前を直接入力して、新しい名前付きアカウントを作成することもできます。 終了したらボックスから離れる場所をクリックします。

   ![](assets/disc-comp-five.png)

   ...新しい指定されたアカウントが表示されます。 その時点で、手順4の **「次へ** 」をクリックします。

   ![](assets/disc-comp-six.png)

1. 「 **作成**」をクリックします。

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
>* [顧客との照合を引き出す](/help/marketo/product-docs/account-based-marketing/target/named-accounts/lead-to-account-matching.md)

