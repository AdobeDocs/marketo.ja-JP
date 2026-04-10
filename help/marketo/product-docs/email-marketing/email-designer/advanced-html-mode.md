---
solution: Marketo Engage
product: marketo
title: メールコンテンツへのカスタム CSS の追加
description: E メールDesignerで、カスタム CSSをメールコンテンツに追加する方法を説明します。 Marketo Engageのカスタムコードを使用して、メールのスタイルを設定できます。
level: Intermediate
feature: Email Designer
exl-id: b030e56a-de70-4b0d-9788-04a01235cffb
source-git-commit: af89a1a1fd0246564d0904103f742230a096de04
workflow-type: tm+mt
source-wordcount: '366'
ht-degree: 2%

---

# 高度なHTMLエディターでメールテンプレートを編集できます {#advanced-html-mode}

高度なHTML モードを使用すると、[!DNL Marketo Engage] メール Designer インターフェイスから直接、メールテンプレートの生のソースコードを表示および編集できます。

この機能を使用すると、高度なエクスプレッションをソースに直接挿入できます。 ビジュアル（デスクトップ）ビューに切り替えると、コンテンツが再レンダリングされるので、どのビューでもコンテンツの外観を確認し、編集を続行できます。

## ガードレール {#guardrails}

高度なHTML エディターを使用する場合、次のガードレールはコンテンツの互換性を保護し、期待値を設定します。

* 高度なHTML エディター&#x200B;**でコードが検証されません**。 構文エラーや壊れたレイアウトはチェックしません。 保存する前に、コンテンツを注意深く確認してください。

* 今後のシステムの更新によって、デフォルトのマークアップに加えた変更が上書きされる可能性があります。 **変更が保持されない可能性があります**。

* [!DNL Adobe]のサポート **は、カスタムコードと手動での変更によって発生する**&#x200B;の問題をトラブルシューティングまたは解決できません。 元に戻す必要がある場合に備えて、コンテンツのバックアップを取っておきます。

* 高度なHTML ビューでコンテンツをシミュレートすることはできません。 デスクトップ表示に切り替えて、コンテンツをプレビューします。

* コンテンツの互換性を確保するために、高度なHTML ビューに&#x200B;**保存できません**。 変更を保存する準備ができたら、デスクトップ表示に切り替えます。

## 高度なHTML モードへのアクセス {#access-html-mode}

高度なHTML エディターを開き、テンプレートソースを編集するには、次の手順に従います。

1. 電子メール Designerで電子メールテンプレート [を開くか、](/help/marketo/product-docs/email-marketing/email-designer/email-template-authoring.md#create-an-email-template)作成します。

1. _電子メールテンプレートを編集_&#x200B;画面で、右上隅にある「HTML」ボタンをクリックします。

   ![](assets/advanced-html-mode-1.png){width="800" zoomable="yes"}

1. 高度なHTML エディタを初めて開くと、警告メッセージが表示されます。 完了したら、**[!UICONTROL OK]**&#x200B;をクリックして確認します。

   ![](assets/advanced-html-mode-2.png)

   >[!NOTE]
   >
   >この警告は、HTMLの詳細エディターを初めて開いたときに表示され、毎月更新されます。

1. 高度なHTML エディターが表示されます。

   ![](assets/advanced-html-mode-3.png){width="800" zoomable="yes"}

1. メールコンテンツに変更を加えます。

   >[!WARNING]
   >
   >構文の検証プロセスはなく、Adobe サポートはHTMLの編集を支援できないので、正しいHTMLとCSS コードを入力してください。

1. コンテンツのシミュレーションと保存は、互換性の理由により、高度なHTML ビューでは使用できません。 デスクトップビューに戻して、コンテンツをプレビューし、変更を保存します。

   ![](assets/advanced-html-mode-4.png){width="800" zoomable="yes"}

   >[!NOTE]
   >
   >ビューを切り替えると、編集内容は保持されます。
