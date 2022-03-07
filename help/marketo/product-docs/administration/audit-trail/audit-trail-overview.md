---
unique-page-id: 11377945
description: 監査証跡の概要 - Marketo ドキュメント - 製品ドキュメント
title: 監査証跡の概要
exl-id: e8aff7b7-72ca-4d4e-9159-56ff65f6345c
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: ht
source-wordcount: '332'
ht-degree: 100%

---

# 監査証跡の概要 {#audit-trail-overview}

監査証跡は、Marketo インスタンスで行った変更の詳細な履歴（6 か月分）を取得する機能です。

>[!NOTE]
>
>監査証跡のデータ履歴は、2016年9月14日（PT）に始まります。

![](assets/one.png)

## 監査証跡とは {#what-is-audit-trail}

監査証跡は、Marketo サブスクリプションで発生するアクションとイベントの総合的なリストをリアルタイムで取得します。セルフサービス方式で、6 か月の履歴データにアクセスし、以下のような質問に答えることに役立ちます。

このアセットまたは設定に何が起きたか、最後に更新したのは誰か。

ユーザー X は何をしているか。

アカウントにログインしているのは誰か。

## 監査の対象 {#what-we-audit}

Marketo は、次のものについて[作成、編集、削除](/help/marketo/product-docs/administration/audit-trail/change-details-in-audit-trail.md)のアクションを監査します。

* デザインスタジオのアセット
* すべての Marketo プログラム
* スマートキャンペーン
* リスト（スマート／静的）
* ユーザー（管理）
* 役割と権限（管理）
* ワークスペースとパーティション（管理）
* ユーザーログイン履歴

>[!NOTE]
>
>Marketo は、現時点で web パーソナライズ機能、予測コンテンツ、Sales Insight 内で行われた変更を監査するのには&#x200B;_役立ちません_。

## 監査証跡のコンポーネント {#audit-trail-components}

監査証跡は、次の 3 つのコンポーネントで構成されます。

**1) [アセット監査証跡](/help/marketo/product-docs/administration/audit-trail/change-details-in-audit-trail.md#asset-audit-trail)**

特定のアセットに対して実行されたアクティビティを確認します。

**2）[管理監査証跡](/help/marketo/product-docs/administration/audit-trail/change-details-in-audit-trail.md#admin-audit-trail)**

ユーザーベースの詳細を監視します。

**3）[ユーザーログイン履歴](/help/marketo/product-docs/administration/audit-trail/user-login-history.md)**

自分のサブスクリプションに誰が、いつログインしたのかを確認します。ログイン試行の失敗も含まれます。

>[!TIP]
>
>監査証跡を使って監査できることはたくさんあります。必ず[フィルター](/help/marketo/product-docs/administration/audit-trail/filtering-in-audit-trail.md)を使用してください。

## データのエクスポート {#exporting-data}

表示できるのは、インスタンスの 30 日分のデータだけです。最大で 6 か月分のデータを取得するには、エクスポートオプションを使用してください。

![](assets/two.png)

>[!NOTE]
>
>**定義**
>
>**不明**：監査記録に、ユーザーの名前とメールが「不明」と表示される場合があります。これは、CRM の選択リスト値を変更すると発生します。これらの値は、Marketo フォームとランディングページに表示されます。CRM 側でこの更新を行うと、フォームを参照するランディングページが自動的にドラフト化されます。監査記録では、ランディングページが作成されたことを捕捉しますが、CRM 側からユーザー情報を取り込めないので、ユーザー名とメールは「不明」と表示されます。

>[!MORELIKETHIS]
>
>[監査記録の有効化](/help/marketo/product-docs/administration/audit-trail/enable-audit-trail.md)
