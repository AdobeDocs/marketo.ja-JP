---
unique-page-id: 2360219
description: カスタム DKIM 署名の設定 - Marketo ドキュメント - 製品ドキュメント
title: カスタム DKIM 署名の設定
exl-id: a7c6429e-14ee-439e-9f47-1b25b98d41e7
feature: Deliverability
source-git-commit: 47bc93665a7efa0d64cd4d5f34b868895d407527
workflow-type: tm+mt
source-wordcount: '345'
ht-degree: 69%

---

# カスタム DKIM 署名の設定 {#set-up-a-custom-dkim-signature}

最高の到達率を確保するために、すべてのアウトバウンドメールに共有 Marketo DKIM 署名を使用して自動的に署名します。

>[!NOTE]
>
>この記事の手順の一部を完了するには、IT チームの支援が必要になる場合があります。

DKIM 署名をパーソナライズして、選択したドメインを反映させることができます。手順は以下のとおりです。

1. 「**管理者**」セクションに移動します。

   ![](assets/set-up-a-custom-dkim-signature-1.png)

   >[!NOTE]
   >
   >古い方法でカスタム DKIM 署名を設定した場合、その署名は引き続き機能し、ここに表示されます。

1. 「**メール**」をクリックします。

   ![](assets/set-up-a-custom-dkim-signature-2.png)

1. 次をクリック： **SPF/DKIM** タブ、 **ドメインを追加**.

   ![](assets/set-up-a-custom-dkim-signature-3.png)

1. Marketo E メールで使用するドメインを、送信元アドレスとして入力します。 「セレクター」と「キーサイズ」を選択します。 終了したら「**追加**」をクリックします。

   ![](assets/set-up-a-custom-dkim-signature-4.png)

   >[!TIP]
   >
   >* 2048 のキーサイズをお勧めします。
   >* 送信元アドレスに別のドメインを使用している場合、Marketoの共有 DKIM 署名を使用します。

   <table> 
   <tr>
   <td width="20%"><b>セレクター</b></td>
   <td>DKIM レコードの公開鍵部分を見つけるために使用される一意の文字列/識別子。 任意の文字列を指定することも、DKIM キー/レコードの目的を区別して識別する一意の ID を指定することもできます。</td>
   </tr>
   <tr> 
   <td width="20%"><b>キーサイズ</b></td>
   <td>DKIM 署名を暗号化する際のセキュリティレベルです。</td>
   </tr>
   </tbody>
   </table>

   <p>

1. IT に&#x200B;**ホストレコード**&#x200B;および&#x200B;**文字列の値**&#x200B;を送信します。レコードを作成して、送信元ドメインに関連付けられているすべてのネームサーバーに反映させるように依頼します。Marketo の DKIM 検証では、DKIM 鍵が DKIM 署名済みのドメインに関連付けられているすべてのネームサーバーに伝播される必要があります。

   ![](assets/set-up-a-custom-dkim-signature-5.png)

1. レコードの作成を確認したら、Marketo に戻り、ドメインを選択して、「**DNS を確認**」をクリックします。

   ![](assets/set-up-a-custom-dkim-signature-6.png)

   >[!NOTE]
   >
   >確認に失敗したが IT はレコードを正しく作成している場合は、DNS の伝播が問題になっている可能性があります。後でもう一度お試しください。

   >[!CAUTION]
   >
   >対応する DNS レコードを変更または削除すると、到達率が低下します。DNS を変更する前に、必ず Marketo のエントリを削除してください。

   これは、メールの到達率に絶対に役立ちます。レコードが存在し、正しいことを確認する必要があります。
