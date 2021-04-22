---
unique-page-id: 11377945
description: 監査証跡の概要 —Marketoドキュメント — 製品ドキュメント
title: 監査証跡の概要
exl-id: e8aff7b7-72ca-4d4e-9159-56ff65f6345c
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '332'
ht-degree: 0%

---

# 監査証跡の概要{#audit-trail-overview}

監査証跡を使用すると、Marketo・インスタンス内で行われた変更の完全な履歴（6ヶ月分の値）を取得できます。

>[!NOTE]
>
>監査証跡データ履歴は、2016年9月14日から開始されました。

![](assets/one.png)

## 監査証跡とは{#what-is-audit-trail}

監査証跡は、Marketo購読内で発生するアクションとイベントの包括的なリストをリアルタイムでキャプチャします。 6か月のデータ履歴にアクセスして次のような質問に答えるセルフサービスを提供します。

このアセットまたは設定はどうなりましたか。また、最後に更新したのは誰ですか。

Xが何を企んでいるか

アカウントにログインしているユーザー

## 監査対象{#what-we-audit}

Marketoは、[create, edit, and delete](/help/marketo/product-docs/administration/audit-trail/change-details-in-audit-trail.md)アクションを監査します。

* Design Studioアセット
* 全Marketoプログラム
* スマートキャンペーン
* リスト（スマート/静的）
* ユーザー(admin)
* ロールと権限(admin)
* ワークスペースとパーティション(admin)
* ユーザーログイン履歴

>[!NOTE]
>
>現在、Marketoは、Webパーソナライゼーション、予測コンテンツ、Sales Insight内で行われた監査の変更は&#x200B;_行われません_。

## 監査証跡コンポーネント{#audit-trail-components}

監査証跡は、3つのコンポーネントで構成されます。

**(1) [資産監査証跡](/help/marketo/product-docs/administration/audit-trail/change-details-in-audit-trail.md#asset-audit-trail)**

特定のアセットに対するアクティビティの実行を参照してください。

**2) [管理監査証跡](/help/marketo/product-docs/administration/audit-trail/change-details-in-audit-trail.md#admin-audit-trail)**

ユーザーベースの詳細を監視します。

**3) [ユーザログイン履歴](/help/marketo/product-docs/administration/audit-trail/user-login-history.md)**

購読にログインしているユーザーとログインしているタイミングを確認する。 失敗したログイン試行も含まれます。

>[!TIP]
>
>監査証跡を使用して監査できる量は非常に多いので、[フィルタ](/help/marketo/product-docs/administration/audit-trail/filtering-in-audit-trail.md)を必ず利用してください。

## データのエクスポート {#exporting-data}

インスタンスでは、30日分のデータのみを表示できます。 6か月分の値を取得するには、エクスポートオプションを使用します。

![](assets/two.png)

>[!NOTE]
>
>**定義**
>
>**不明：監査証跡** に、ユーザーの名前と電子メールが「不明」と表示される場合があります。これは、CRMの選択リストの値を変更した場合に発生します。 これらの値は、Marketoのフォームおよびランディングページに表示されます。 CRM側でこの更新を行うと、フォームを参照するランディングページが自動ドラフトされます。 監査証跡では、ランディングページがドラフトされたことをキャプチャしますが、CRM側からユーザー情報を取り込めないので、ユーザーの名前と電子メールには「不明」と表示されます。

>[!MORELIKETHIS]
>
>[監査証跡の有効化](/help/marketo/product-docs/administration/audit-trail/enable-audit-trail.md)
