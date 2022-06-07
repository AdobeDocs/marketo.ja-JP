---
description: プログラムメンバーカスタムフィールド - Marketo ドキュメント - 製品ドキュメント
title: プログラムメンバーカスタムフィールド
hide: true
hidefromtoc: true
source-git-commit: a14516e0daf3b9c9b90aa0250fd654b8bbbcc391
workflow-type: tm+mt
source-wordcount: '342'
ht-degree: 20%

---

# プログラムメンバーカスタムフィールドの同期 {#program-member-custom-field-sync}

>[!PREREQUISITES]
>
>の作成 [プログラムメンバーカスタムフィールド](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/program-member-custom-fields.md){target=&quot;_blank&quot;}

>[!NOTE]
>
>プログラムメンバーオブジェクトには、最大 20 個のカスタムフィールドを持つことができます。これらのフィールドは、どのプログラムでも使用できます。

## Salesforce フィールドをプログラムメンバーフィールドにマッピング {#map-salesforce-fields-to-program-member-fields}

1. Marketo で、「**管理者**」をクリックします。

   ![](assets/program-member-custom-field-sync-1.png)

1. クリック **Salesforce**&#x200B;を選択し、「 **編集** [ プログラムメンバのカスタムフィールドの同期 ] の横に表示されます。

   ![](assets/program-member-custom-field-sync-2.png)

1. 検索ボックスを使用して、マッピングする Salesforce フィールドを見つけます。 この例では、Do Not Call を使用しています。

   ![](assets/program-member-custom-field-sync-3.png)

1. ドロップダウンをクリックします。

   ![](assets/program-member-custom-field-sync-4.png)

1. マッピングする目的のMarketoプログラムメンバーカスタムフィールドを選択します。

   ![](assets/program-member-custom-field-sync-5.png)

   >[!NOTE]
   >
   >このドロップダウンには、Salesforce フィールドのデータ型と一致するプログラムメンバカスタムフィールドのみが表示されます。

1. その他のフィールドマッピングについては、検索ボックスをオフにして、手順 3 ～ 5 を繰り返します。

1. 終了したら「**保存**」をクリックします。

   ![](assets/program-member-custom-field-sync-6.png)

   >[!IMPORTANT]
   >
   >マッピングされたフィールド上のプログラムメンバーデータの変更は、今後、Marketoと Salesforce の間で同期されます。

   >[!NOTE]
   >
   >Salesforce でフィールドのデータ型の名前を変更または変更した場合、そのフィールドとプログラムメンバーカスタムフィールドとのマッピングはすべて削除されます。 ただし、レビュー後に新しいフィールドに再マップすることができます。

## Salesforce フィールドのプログラムメンバーフィールドへのマッピング解除 {#unmap-salesforce-fields-to-program-member-fields}

フィールドを置き換えるために解放したい場合や、一般的な変更を行う場合は、まずマッピング解除を実行する必要があります。 手順は以下のとおりです。

1. Marketo で、「**管理者**」をクリックします。

   ![](assets/program-member-custom-field-sync-7.png)

1. クリック **Salesforce**&#x200B;を選択し、「 **編集** [ プログラムメンバのカスタムフィールドの同期 ] の横に表示されます。

   ![](assets/program-member-custom-field-sync-8.png)

1. 検索ボックスを使用して、マッピングを解除するフィールドを見つけます。 この例では、Do Not Call を使用しています。

   ![](assets/program-member-custom-field-sync-9.png)

   >[!TIP]
   >
   >次の項目を選択できます。 **マッピング済み** チェックボックスをオンにして、マッピングされたフィールドのみを表示します。

1. マッピングを解除するには、 **X** をクリックします。

   ![](assets/program-member-custom-field-sync-10.png)

1. これで、マッピングが削除されます。 「**保存**」をクリックします。

   ![](assets/program-member-custom-field-sync-11.png)

## データタイプマッピング {#datatype-mapping}

<table>
  <colgroup>
    <col/>
    <col/>
  </colgroup>
  <tbody>
    <tr>
      <th>SFDC データタイプ</th>
      <th>プログラムメンバーフィールドデータタイプ</th>
    </tr>
    <tr>
      <td>テキスト</td>
      <td>文字列</td>
    </tr>
    <tr>
      <td>ピックリスト</td>
      <td>文字列</td>
    </tr>
    <tr>
      <td>複数選択候補リスト</td>
      <td>文字列</td>
    </tr>
    <tr>
      <td>電話</td>
      <td>文字列</td>
    </tr>
    <tr>
      <td>メール</td>
      <td>文字列</td>
    </tr>
    <tr>
      <td>数値 (m)</td>
      <td>整数</td>
    </tr>
    <tr>
      <td>数値 (m,n)</td>
      <td>浮動</td>
    </tr>
    <tr>
      <td>チェックボックス</td>
      <td>ブール値</td>
    </tr>
    <tr>
      <td>URL</td>
      <td>URL</td>
    </tr>
    <tr>
      <td>日付</td>
      <td>日付</td>
    </tr>
    <tr>
      <td>日時</td>
      <td>日時</td>
    </tr>
    <tr>
      <td>参照（参照）</td>
      <td>文字列</td>
    </tr>
    <tr>
      <td>Base64</td>
      <td>文字列</td>
    </tr>
  </tbody>
</table>

>[!MORELIKETHIS]
>
>* [プログラムメンバーデータの変更](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/program-flow-actions/change-program-member-data.md){target=&quot;_blank&quot;}
>* [プログラムメンバーグリッドのデータを表示](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/manage-and-view-members.md){target=&quot;_blank&quot;}

