---
unique-page-id: 5472678
description: 非ラテン文字リストの読み込み — Marketo ドキュメント — 製品ドキュメント
title: 非ラテン文字リストの読み込み
exl-id: 11519e2c-ab01-4164-8ce3-0717e4c13ae6
feature: Email Programs
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '308'
ht-degree: 85%

---

# 非ラテン文字リストの読み込み {#import-a-non-latin-characters-list}

英語以外のファイルをインポートしようとしている場合、Excel で開くと、リストが完璧に表示されます。

![](assets/image2015-2-10-9-3a34-3a57.png)

ただし、Marketo に読み込むと、英語以外の文字が正しく取り出されていないことがあります。

![](assets/image2015-2-10-9-3a35-3a49.png)

これは、ファイルが Marketo で正しく保存されず、非ラテン文字が認識されないためです。幸い、これは簡単な手順を実行して修正できます。

1. Excel の **[!UICONTROL ファイル &#x200B;] メニューから「** 名前を付けて保存 **[!UICONTROL ...]**」を選択します。

   ![](assets/image2015-2-10-9-3a46-3a44.png)

1. 「**[!UICONTROL 形式]**」オプションとして「**[!UICONTROL UTF-16 Unicode テキスト（.txt）]**」を選択します。これにより、Marketo で表示できるようにファイルがエンコードされます。

   ![](assets/image2015-2-10-9-3a48-3a7.png)

   >[!NOTE]
   >
   >Marketo では、UTF-8、Shift-JIS、EUC-JP もサポートしています。

1. 新しいファイルは、.txt 拡張子を持つテキストファイルとして保存されます。また、ファイル内のすべてのコンマがタブに変換されるので、これを元に戻す必要があります。

   >[!TIP]
   >
   >Windows を使用している場合は **[!DNL Notepad]** を使用し、Macを使用している場合は **[!DNL TextEdit]** を使用して、テキストファイルを開くことができます。

   ![](assets/image2015-2-10-9-3a51-3a41.png)

1. ドキュメントからタブを選択してコピーします。

   ![](assets/image2015-2-10-9-3a55-3a53.png)

1. **[!UICONTROL 編集 &#x200B;] メニューから「** 検索と置換 **[!UICONTROL ...]**」を選択します。

   ![](assets/image2015-2-10-9-3a59-3a8.png)

   >[!TIP]
   >
   >Windows ユーザーに対する同等のアクションは、**[!UICONTROL 編集 &#x200B;]/[!UICONTROL &#x200B; 置換 &#x200B;]...** です。

1. 手順 4 でコピーしたタブを最初の（検索）ボックスに貼り付け、2 番目の（置換後）ボックスにコンマを入力します。次に、「**[!UICONTROL すべて]**」をクリックします。

   ![](assets/image2015-2-10-10-3a8-3a53.png)

1. コンマがすべて戻ったので、先に進みます。

   ![](assets/image2015-2-10-10-3a14-3a45.png)

1. 新しいファイルを Marketo にインポートします。この時点で、情報が正しく表示されます。

   ![](assets/image2015-2-10-10-3a16-3a9.png)

   >[!NOTE]
   >
   >読み込まれる日時フィールドは、すべて米中央時間として扱われます。日時フィールドのタイムゾーンが異なる場合、Excel の数式を使用して、中央時刻（米国／シカゴ）に変換できます。

奇妙な事は分かっていますがうまくいきます。お疲れさまでした。
