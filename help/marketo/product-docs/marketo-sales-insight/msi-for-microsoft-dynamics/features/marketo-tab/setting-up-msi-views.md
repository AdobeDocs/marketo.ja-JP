---
description: MSI ビューの設定 — Marketoドキュメント — 製品ドキュメント
title: MSI ビューの設定
source-git-commit: 8227648ce67bf0f9f8b3b2fea7445850d8e154d5
workflow-type: tm+mt
source-wordcount: '260'
ht-degree: 3%

---

# MSI ビューの設定 {#setting-up-msi-views}

Dynamics に Sales Insight プラグインをインストールすると、サイトマップに Best Bets と関連するダッシュボードが自動的に追加されます。 何らかの理由でダッシュボードが追加されない場合は、手動で追加する方法を次に示します。

1. Dynamics で、歯車アイコンをクリックし、 **詳細設定** 」をクリックします。

1. 画面の左上で、 **設定**. 「カスタマイズ」で、 **カスタマイズ**.

1. 「**システムをカスタマイズ**」をクリックします。

1. 左側のツリーで、 **クライアント拡張** をクリックし、ダブルクリックします。 **サイトマップ**.

1. 右向き矢印をクリックして次のページに移動します。 「Sales」の下に、「Marketo」が表示されます。 表示されない場合は、パッケージが正しく読み込まれていることを確認してください。

   >[!NOTE]
   >
   >Marketoでは、次の操作をおこなう必要があります。最優先、マイメール、ウェブアクティビティ、匿名ウェブアクティビティ。 これらのダッシュボードが見つからない場合は、「Sales」の上の「+」記号をクリックし、サブ領域として追加します。

1. ダッシュボードをクリックして選択します。 右側の列に、それぞれの情報を以下に入力します。 一覧に表示されていないカテゴリは無視できます。

   **最優先**</br>
URL:MainviewBestbets.html</br>
アイコン：/WebResources/mkt_/_MainView/_imgs/icons/bestbets.svg</br>
ID:marketo_bestbets</br>
タイトル：最優先

   **マイメール**</br>
URL:mkt_/MainViewMyEmail.html</br>
アイコン：/WebResources/mkt_/_MainView/_imgs/icons/email.svg</br>
ID:marketo_myemail</br>
タイトル：マイメール

   **ウェブアクティビティ**</br>
URL:mkt_/MainViewWebActivity.html</br>
アイコン：/WebResources/mkt_/_MainView/_imgs/icons/web_activity.svg</br>
ID:marketo_webactivity</br>
タイトル：ウェブアクティビティ

   **匿名のウェブアクティビティ**</br>
URL:mkt_/MainViewWebActivity.html</br>
アイコン：/WebResources/mkt_/_MainView/_imgs/icons/anonymous_web_activity.svg</br>
ID:marketo_anonymous_webactivity</br>
タイトル：匿名のウェブアクティビティ

1. 終了したら「**保存**」をクリックします。
