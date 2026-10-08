---
unique-page-id: 2953188
description: スマートリストの推定フィルターについて説明します。 リンクされたアセットからフィルターを推測するMarketoの仕組みを説明します。
title: 推測フィルター
exl-id: 6db4ff4d-7fab-4722-94b1-1bf92ba4651d
feature: Smart Lists
TQID: 'https://experienceleague.adobe.com/-dKeAfCxfD1ErbfBzLqARUMwFY-I9RdkWGC0b-ZtNyE'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
    internal-label: Integrations
  - id: c5f60233-d5ea-4453-a799-0ad258b4d399
    internal-label: Database
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
    internal-label: Administration
  - id: a7170d27-32ab-462b-a333-269abc654483
    internal-label: Smart Campaigns
subfeature_v2:
  - id: d0251300-e25f-466f-9856-7e11ce8fa7aa
    internal-label: Smart lists
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '218'
ht-degree: 77%
---
# 推測フィルター {#inferred-filters}

web サイトの訪問者には、[Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md){target="_blank"} Cookie が作成され、システムに格納されます。 システムは特別なデータベースでIPを検索し、あらゆる種類の情報を推測します。

>[!NOTE]
>
>推定フィールド値を最新の状態に保つために、IP アドレス検索に使用されるデータベースは定期的に更新されます。 データベースの更新によって新しい推測フィールド値が追加されることがあり、それらをスマートリストのフィルター定義に追加する必要が生じる場合があります。
>
>データベースの更新は、[Marketo Engage 製品のリリース](/help/marketo/release-notes/release-schedule.md){target="_blank"}中に行われる場合があります。 更新が行われると、[Marketo Engage リリースノート](/help/marketo/release-notes/current.md){target="_blank"}に、推測されるフィールド値の変更に関する説明が含まれます。

![](assets/inferred-filters-1.png)

![](assets/inferred-filters-2.png)

![](assets/inferred-filters-3.png)

![](assets/inferred-filters-4.png)

![](assets/inferred-filters-5.png)

![](assets/inferred-filters-6.png)

スマートリストでこれらのフィルターのいずれかを使用すると、推測される情報を持つ人物が表示されます。

>[!TIP]
>
>これらのフィルターを web アクティビティレポートで使用します。 セールス担当の担当地域を使用して、過去 24 時間以内の web サイト訪問者を含むカスタム日次レポートに登録します。 きっと気に入ることでしょう。
>
>* Web ページを訪問 - 過去 24 時間
>* 推測される都道府県／地域に、[担当地域を選択]します。

匿名の訪問者は、メールリンクをクリックしたりフォームに入力したりすると、自動的に人物に変換されます。 ただし、推測される情報はすべて保持されます。

>[!NOTE]
>
>詳しくは、[匿名のアクティビティとリード](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/understanding-anonymous-activity-and-people.md){target="_blank"}を参照してください。
