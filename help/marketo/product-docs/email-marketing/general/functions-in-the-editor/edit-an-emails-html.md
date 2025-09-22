---
unique-page-id: 1900554
description: メールの HTML を編集する - Marketo ドキュメント - 製品ドキュメント
title: メールの HTML を編集する
exl-id: 9dc8e44d-d9da-4bc2-950f-3ffbb976f5d5
feature: Email Editor
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 100%

---

# メールの HTML を編集する {#edit-an-emails-html}

メールの基になる HTML の変更が必要になることがあります。外部システムを使用してメールのコードを設計および構築することもあります。どちらの場合も、メールエディター内から簡単にコードを読み込んだり、編集したりできます。

## HTML の編集 {#edit-html}

1. メールを選択して、「**[!UICONTROL ドラフトを編集]**」をクリックします。

   ![](assets/teamspidey.jpg)

1. 「**[!UICONTROL コードを編集]**」をクリックします。

   ![](assets/two-4.png)

1. 変更を加えます。終了したら「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/three-3.png)

   >[!NOTE]
   >
   >好きなように変更できます。HTML 全体を置き換えることも、若干の調整をおこなうこともできます。

1. **[!UICONTROL コードアクション]**&#x200B;ドロップダウンをクリックすると、コードの HTML ファイルのダウンロード、CSS のインライン化、HTML の検証のいずれかをおこなうことができます。

   ![](assets/four-2.png)

   >[!NOTE]
   >
   >メールのベストプラクティスは、すべてのスタイルをインライン化することです。複数のメールクライアントでは、`<head>` セクションでの CSS はサポートされていません。

## テンプレートからのメールの分離 {#breaking-an-email-from-its-template}

メールはこれらのコードの変更によってはテンプレートから分離&#x200B;**されません**。

* 任意のモジュールのコンテンツの編集（モジュール内への新しい要素の追加を含む）
* コンテナへの新しいモジュールの追加
* コンテナからのモジュールの削除

* モジュール外の任意の要素の mkto 固有の属性（たとえば、「mktoName」や「mktoImgUrl」）の変更
* モジュール外の任意の要素（リッチテキスト、画像、ビデオなど）のコンテンツの編集

コードエディターで次を実行すると、メールがテンプレートから分離&#x200B;**されます**。

* 要素またはモジュール外のコード内の変更
* モジュール外の任意の要素の非 mkto 属性（「id」や「style」など）の追加または変更
* モジュール外の要素の削除

## コードの検索 {#search-code}

コードを検索機能を使用すると、メールの HTML コード内のコンテンツを効率的に検索して置換することができます。

1. メールのコードで、「**[!UICONTROL コードを検索]**」をクリックします。

   ![](assets/five-2.png)

1. 検索する項目を入力し、「**[!UICONTROL 次を検索]**」をクリックして前方を検索するか、「**[!UICONTROL 前を検索]**」で逆方向に検索します。また、「**[!UICONTROL 置換]**」および「**[!UICONTROL すべてを置換]**」オプションもあります。

   ![](assets/six-1.png)

1. 終了したら「**[!UICONTROL 閉じる]**」をクリックします。

   ![](assets/seven.png)

   >[!NOTE]
   >
   >「コードを検索」は、[メールテンプレートエディター](/help/marketo/product-docs/email-marketing/general/email-editor-2/create-an-email-template.md)でも使用できます。

Marketo のビルトインの機能を使用してメールを引き続き編集することをお勧めしますが、必要に応じて、このコードエディターで柔軟にメールを編集できます。
