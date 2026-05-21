---
unique-page-id: 2360219
description: Marketoでドメインのカスタム DKIM署名を設定する方法について説明します。 管理者でドメインを追加し、IT部門と協力してDNS レコードを公開します。
title: カスタム DKIM 署名の設定
exl-id: a7c6429e-14ee-439e-9f47-1b25b98d41e7
feature: Deliverability
TQID: https://experienceleague.adobe.com/ln23WoloRVzBoC8CXFsm90LqYV5FDJzbII8UItp3xDc
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
topic_v2:
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
source-git-commit: 39b6fecdc7aa16ab1205582d3bf372a8538a2d35
workflow-type: tm+mt
source-wordcount: 434
ht-degree: 49%

---

# カスタム DKIM 署名の設定 {#set-up-a-custom-dkim-signature}

最適な配信品質を確保するために、Marketoでは、すべての送信メールにDKIMの共有署名を自動的に割り当てます。

>[!NOTE]
>
>この記事の手順の一部を完了するには、IT チームの支援が必要になる場合があります。

DKIM 署名をパーソナライズして、選択したドメインを反映させることができます。

1. 「**[!UICONTROL 管理者]**」セクションに移動します。

   ![](assets/set-up-a-custom-dkim-signature-1.png)

   >[!NOTE]
   >
   >従来の方法を使用してカスタム DKIM署名を設定した場合、その署名は引き続き機能し、ここに表示されます。

1. 「**メール**」をクリックします。

   ![](assets/set-up-a-custom-dkim-signature-2.png)

1. 「**SPF/DKIM**」タブ、「**ドメインを追加** の順にクリックします。

   ![](assets/set-up-a-custom-dkim-signature-3.png)

1. Marketoの電子メールで使用するドメインを送信元アドレスとして入力します。 セレクターとキーサイズを選択します。 終了したら「**追加**」をクリックします。

   ![](assets/set-up-a-custom-dkim-signature-4.png)

   <table>
   <tr>
   <td width="20%"><b>セレクター</b></td>
   <td>DKIM レコードの公開鍵部分の検索に使用される一意の文字列/識別子。 任意の文字列、またはそのDKIM キー/レコードの目的を分離して識別する一意のIDを指定できます。</td>
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
   >* キーサイズは2048をお勧めします。
   >* 差出人アドレスで別のドメインを使用する場合、Marketoは共有DKIM署名を使用します。

   >[!IMPORTANT]
   >
   >ドメインの DKIM セレクターまたは DKIM 暗号化サイズを更新する必要がある場合は、既存のレコードを削除し、新しい値を使用して新しく生成されたレコードを再公開する必要があります。
   >
   >その場合、新しいレコードが公開され、アドビのシステムで検証されるまで、DKIMはお客様のドメイン用に署名されません。 新しい DKIM レコードがインターネット全体に完全に反映されるまでに 24～48 時間かかる場合があるので、それに応じて変更を計画します。

1. IT に&#x200B;**[!UICONTROL ホストレコード]**&#x200B;および&#x200B;**[!UICONTROL 文字列の値]**&#x200B;を送信します。 レコードを作成し、送信元ドメインに関連付けられたすべてのネームサーバーに反映するように依頼します。 Marketo の DKIM 検証では、DKIM 鍵が DKIM 署名済みのドメインに関連付けられているすべてのネームサーバーに伝播される必要があります。

   ![](assets/set-up-a-custom-dkim-signature-5.png)

1. レコードを作成したことを確認したら、Marketoに戻り、ドメインを選択して、**[!UICONTROL DNSを確認]**&#x200B;をクリックします。

   ![](assets/set-up-a-custom-dkim-signature-6.png)

   >[!NOTE]
   >
   >確認に失敗したが IT はレコードを正しく作成している場合は、DNS の伝播が問題になっている可能性があります。 後でもう一度お試しください。

   >[!CAUTION]
   >
   >対応する DNS レコードを変更または削除すると、到達率が低下します。 DNSを変更する前に、Marketoのエントリを削除します。

   これにより、メールの到達性が向上します。 レコードが存在し、正しいことを確認する必要があります。
