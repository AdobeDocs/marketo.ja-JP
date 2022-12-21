---
description: MSI ビューの設定 - Marketo ドキュメント - 製品ドキュメント
title: MSI ビューの設定
exl-id: 8a45c006-73d4-4af8-ad62-b084056d1f7d
source-git-commit: fda1bf51d4016a61c41be9acba4771db1797a552
workflow-type: tm+mt
source-wordcount: '260'
ht-degree: 100%

---

# MSI ビューの設定 {#setting-up-msi-views}

Dynamics に Sales Insight プラグインをインストールすると、サイトマップに「最優先」と関連するダッシュボードが自動的に追加されます。何らかの理由でダッシュボードが追加されない場合に手動で追加する方法を次に示します。

1. Dynamics で、歯車アイコンをクリックし、ドロップダウンから「**詳細設定**」をクリックします。

1. 画面の左上で、「**設定**」をクリックします。「カスタマイズ」で、「**カスタマイズ**」を選択します。

1. 「**システムをカスタマイズ**」をクリックします。

1. 左側のツリーで、「**クライアントエクステンション**」をクリックして「**サイトマップ**」をダブルクリックします。

1. 右向き矢印をクリックして次のページに移動します。「セールス」の下に、「Marketo」が表示されます。表示されない場合は、パッケージが正しく読み込まれていることを確認してください。

   >[!NOTE]
   >
   >Marketo には、最優先、マイメール、Web アクティビティ、匿名 Web アクティビティが表示されているはずです。これらのダッシュボードが見つからない場合は、「セールス」の上の「+」記号をクリックし、サブ領域として追加します。

1. ダッシュボードをクリックして選択します。右側の列に、それぞれの情報を以下に入力します。一覧に表示されていないカテゴリは無視できます。

   **最優先**</br>
URL:MainviewBestbets.html</br>
アイコン：/WebResources/mkt_/_MainView/_imgs/icons/bestbets.svg</br>
ID：marketo_bestbets</br>
タイトル：最優先

   **マイメール**</br>
URL：mkt_/MainViewMyEmail.html</br>
アイコン：/WebResources/mkt_/_MainView/_imgs/icons/email.svg</br>
ID：marketo_myemail</br>
タイトル：マイメール

   **Web アクティビティ**</br>
URL：mkt_/MainViewWebActivity.html</br>
アイコン：/WebResources/mkt_/_MainView/_imgs/icons/web_activity.svg</br>
ID：marketo_webactivity</br>
タイトル：Web アクティビティ

   **匿名の Web アクティビティ**</br>
URL：mkt_/MainViewWebActivity.html</br>
アイコン：/WebResources/mkt_/_MainView/_imgs/icons/anonymous_web_activity.svg</br>
ID：marketo_anonymous_webactivity</br>
タイトル：匿名の Web アクティビティ

1. 終了したら「**保存**」をクリックします。
