---
solution: Marketo Engage
product: marketo
title: 高度なHTMLエディターでメールテンプレートを編集できます
description: ガードレール、アクセス手順、主要な制限事項など、Marketo Engage メールDesignerで生のHTML ソースコードを表示および編集する方法について説明します。
level: Intermediate
feature: Email Designer
exl-id: b030e56a-de70-4b0d-9788-04a01235cffb
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: c2dbad80-0f5c-4d96-a798-2a65f93b8721
    internal-label: Assets
subfeature_v2:
  - id: f8f7d99a-f455-45bb-8028-428a55a7130b
    internal-label: Email Designer
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
    internal-label: Intermediate
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '369'
ht-degree: 49%
---
# 高度なHTMLエディターでメールテンプレートを編集できます {#advanced-html-mode}

高度なHTML モードを使用すると、[!DNL Marketo Engage] メール Designer インターフェイスから直接、メールテンプレートの生のソースコードを表示および編集できます。

この機能を使用すると、高度なエクスプレッションをソースに直接挿入できます。 視覚的な（デスクトップ）表示に戻すと、コンテンツが再レンダリングされるので、どちらの表示でも、外観を確認し、編集を続行できます。

## ガードレール {#guardrails}

高度なHTML エディターを使用する場合、次のガードレールにより、コンテンツの互換性が保護され、期待値が設定されます。

* 高度な HTML エディターでは、コードを&#x200B;**検証しません**。 構文エラーやレイアウトの崩れをチェックしません。 保存する前に、コンテンツを慎重に確認してください。

* 今後のシステムアップデートにより、デフォルトのマークアップに行った変更が上書きされる場合があります。 **変更が保持されない場合があります**。

* [!DNL Adobe]のサポート **は、カスタムコードと手動での変更によって発生する**&#x200B;の問題をトラブルシューティングまたは解決できません。 元に戻す必要がある場合に備えて、コンテンツのバックアップを保持しておいてください。

* 高度な HTML 表示では、コンテンツをシミュレートできません。 デスクトップ表示に切り替えて、コンテンツをプレビューしてください。

* コンテンツの互換性を確保するために、高度な HTML 表示では&#x200B;**保存できません**。 変更を保存する準備が整ったら、デスクトップ表示に戻してください。

## 高度なHTML モードへのアクセス {#access-html-mode}

高度なHTML エディターを開き、テンプレートソースを編集するには、次の手順に従います。

1. 電子メール Designerで電子メールテンプレート [&#128279;](/help/marketo/product-docs/email-marketing/email-designer/email-template-authoring.md#create-an-email-template)を開くか、作成します。

1. _電子メールテンプレートを編集_&#x200B;画面で、右上隅にある「HTML」ボタンをクリックします。

   ![](assets/advanced-html-mode-1.png){width="800" zoomable="yes"}

1. 高度なHTML エディタを初めて開くと、警告メッセージが表示されます。 完了したら、**[!UICONTROL OK]**&#x200B;をクリックして確認します。

   ![](assets/advanced-html-mode-2.png)

   >[!NOTE]
   >
   >この警告は、HTMLの詳細エディターを初めて開いたときに表示され、毎月更新されます。

1. 高度な HTML エディターが表示されます。

   ![](assets/advanced-html-mode-3.png){width="800" zoomable="yes"}

1. メールコンテンツに目的の変更を追加します。

   >[!WARNING]
   >
   >構文の検証プロセスはなく、Adobe サポートはHTMLの編集を支援できないので、正しいHTMLとCSS コードを入力してください。

1. コンテンツのシミュレーションと保存は、互換性の理由により、高度な HTML 表示では使用できません。 デスクトップ表示に戻して、コンテンツをプレビューし、変更を保存します。

   ![](assets/advanced-html-mode-4.png){width="800" zoomable="yes"}

   >[!NOTE]
   >
   >ビューを切り替えると、編集は保持されます。
