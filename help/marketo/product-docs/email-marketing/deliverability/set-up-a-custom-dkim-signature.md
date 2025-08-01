---
unique-page-id: 2360219
description: カスタム DKIM 署名の設定 - Marketo ドキュメント - 製品ドキュメント
title: カスタム DKIM 署名の設定
exl-id: a7c6429e-14ee-439e-9f47-1b25b98d41e7
feature: Deliverability
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '426'
ht-degree: 100%

---

# カスタム DKIM 署名の設定 {#set-up-a-custom-dkim-signature}

最高の到達率を確保するために、すべてのアウトバウンドメールに共有 Marketo DKIM 署名を使用して自動的に署名します。

>[!NOTE]
>
>この記事の手順の一部を完了するには、IT チームの支援が必要になる場合があります。

DKIM 署名をパーソナライズして、選択したドメインを反映させることができます。手順は以下のとおりです。

1. 「**[!UICONTROL 管理者]**」セクションに移動します。

   ![](assets/set-up-a-custom-dkim-signature-1.png)

   >[!NOTE]
   >
   >古い方法でカスタム DKIM 署名を設定した場合、その署名は引き続き機能し、ここに表示されます。

1. 「**メール**」をクリックします。

   ![](assets/set-up-a-custom-dkim-signature-2.png)

1. 「**SPF/DKIM**」タブ、「**ドメインを追加** の順にクリックします。

   ![](assets/set-up-a-custom-dkim-signature-3.png)

1. Marketoのメールで使用するドメインを送信元アドレスとして入力します。 セレクターとキーサイズを選択します。 終了したら「**追加**」をクリックします。

   ![](assets/set-up-a-custom-dkim-signature-4.png)

   <table>
   <tr>
   <td width="20%"><b>セレクター</b></td>
   <td>DKIM レコードの公開鍵部分を検索するために使用される一意の文字列/識別子。 任意の文字列を指定するか、その DKIM キー/レコードの目的を分離して識別する一意の ID を指定できます。</td>
   </tr>
   <tr>
   <td width="20%"><b>キーサイズ</b></td>
   <td>DKIM 署名の暗号化に使用するセキュリティのレベル。</td>
   </tr>
   </tbody>
   </table>

   <p>

   >[!TIP]
   >
   >* 2048 の鍵サイズを推奨します。
   >* 送信元アドレスに別のドメインを使用している場合は、Marketoの共有 DKIM 署名が使用されます。

   >[!IMPORTANT]
   >
   >ドメインの DKIM セレクターまたは DKIM 暗号化サイズを更新する必要がある場合は、既存のレコードを削除し、新しい値を使用して新しく生成されたレコードを再公開する必要があります。
   >
   >その際は、新しいレコードが公開され、システムによって検証されるまで、DKIM はドメインに対して署名されないことに注意してください。 新しい DKIM レコードがインターネット全体に完全に反映されるまでに 24～48 時間かかる場合があるので、それに応じて変更を計画します。

1. IT に&#x200B;**[!UICONTROL ホストレコード]**&#x200B;および&#x200B;**[!UICONTROL 文字列の値]**&#x200B;を送信します。レコードを作成して、送信元ドメインに関連付けられているすべてのネームサーバーに反映させるように依頼します。Marketo の DKIM 検証では、DKIM 鍵が DKIM 署名済みのドメインに関連付けられているすべてのネームサーバーに伝播される必要があります。

   ![](assets/set-up-a-custom-dkim-signature-5.png)

1. レコードの作成を確認したら、Marketo に戻り、ドメインを選択して、「**[!UICONTROL DNS を確認]**」をクリックします。

   ![](assets/set-up-a-custom-dkim-signature-6.png)

   >[!NOTE]
   >
   >確認に失敗したが IT はレコードを正しく作成している場合は、DNS の伝播が問題になっている可能性があります。後でもう一度お試しください。

   >[!CAUTION]
   >
   >対応する DNS レコードを変更または削除すると、到達率が低下します。DNS を変更する前に、必ず Marketo のエントリを削除してください。

   これは、メールの到達率に絶対に役立ちます。レコードが存在し、正しいことを確認する必要があります。
