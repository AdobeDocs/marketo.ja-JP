---
description: セールスアクティビティ用語集 - Marketo ドキュメント - 製品ドキュメント
title: セールスアクティビティ用語集
exl-id: c7805642-07b6-4697-9efe-5c673ae9ca53
feature: Marketo Sales Connect
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '585'
ht-degree: 100%

---

# セールスアクティビティ用語集 {#sales-activity-glossary}

Sales Connect で、販売者がセールスケイデンスにリードを追加したり、メールを送信したり、通話をアクティビティに送信したりすると、Marketo のアクティビティ履歴に記録されます。さらに、リードがメールに関与した場合、開封数、クリック数、返信数もログに記録されます。

以下のアクティビティは、[!DNL Sales Connect] から Marketo に記録されます。

>[!NOTE]
>
>これらのアクティビティと属性は、アドビの REST および Bulk API から使用できます。

## アクティビティ {#activities}

<table>
 <tr>
  <th>セールスアクティビティ</th>
  <th>属性</th>
 </tr>
 <tr>
  <th rowspan="9">セールスメールを送信</th>
  <td>[!UICONTROL 送信者]</td>
 </tr>
 <tr>
  <td>ソース</td>
 </tr>
 <tr>
  <td>[!UICONTROL テンプレート ID]</td>
 </tr>
 <tr>
  <td>[!UICONTROL セールステンプレート] URL</td>
 </tr>
 <tr>
  <td>[!UICONTROL セールスキャンペーン] URL</td>
 </tr>
 <tr>
  <td>[!UICONTROL セールステンプレート] 名</td>
 </tr>
 <tr>
  <td>[!UICONTROL メール件名]</td>
 </tr>
 <tr>
  <td>[!UICONTROL セールスキャンペーン名]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Marketo セールス担当者 ID]</td>
 </tr>
 <tr>
  <th rowspan="9"> セールスメールを開く</th>
  <td>[!UICONTROL 送信者]</td>
 </tr>
 <tr>
  <td>ソース</td>
 </tr>
 <tr>
  <td>[!UICONTROL テンプレート ID]</td>
 </tr>
 <tr>
  <td>[!UICONTROL セールステンプレート URL]</td>
 </tr>
 <tr>
  <td>[!UICONTROL セールスキャンペーン URL]</td>
 </tr>
 <tr>
  <td>[!UICONTROL セールステンプレート名]</td>
 </tr>
 <tr>
  <td>[!UICONTROL メール件名]</td>
 </tr>
 <tr>
  <td>[!UICONTROL セールスキャンペーン名]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Marketo セールス担当者 ID]</td>
 </tr>
 <tr>
  <th rowspan="10">セールスメールをクリック</th>
  <td>[!UICONTROL リンク]</td>
 </tr>
 <tr>
  <td>[!UICONTROL 送信者]</td>
 </tr>
 <tr>
  <td>ソース</td>
 </tr>
 <tr>
  <td>[!UICONTROL テンプレート ID]</td>
 </tr>
 <tr>
  <td>[!UICONTROL セールステンプレート URL]</td>
 </tr>
 <tr>
  <td>[!UICONTROL セールスキャンペーン URL]</td>
 </tr>
 <tr>
  <td>[!UICONTROL セールステンプレート名]</td>
 </tr>
 <tr>
  <td>[!UICONTROL メール件名]</td>
 </tr>
 <tr>
  <td>[!UICONTROL セールスキャンペーン名]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Marketo セールス担当者 ID]</td>
 </tr>
<tr>
  <th rowspan="3">セールスメールに返信</th>
  <td>[!UICONTROL 受信者]</td>
 </tr>
 <tr>
  <td>ソース</td>
 </tr>
 <tr>
  <td>[!UICONTROL Marketo セールス担当者 ID]</td>
 </tr>
 <tr>
  <th rowspan="11">セールス電話を受信</th>
  <td>[!UICONTROL セールス電話発信者]</td>
 </tr>
 <tr>
  <td>[!UICONTROL セールス電話ステータス]</td>
 </tr>
 <tr>
  <td>[!UICONTROL セールス電話件名]</td>
 </tr>
 <tr>
  <td>[!UICONTROL セールスキャンペーン名]</td>
 </tr>
 <tr>
  <td>[!UICONTROL セールスキャンペーン URL]</td>
 </tr>
 <tr>
  <td>[!UICONTROL セールス電話の発信先電話番号]</td>
 </tr>
 <tr>
  <td>ソース</td>
 </tr>
 <tr>
  <td>[!UICONTROL セールス電話の長さ]</td>
 </tr>
 <tr>
  <td>[!UICONTROL セールス電話録音 URL]</td>
 </tr>
  <tr>
  <td>[!UICONTROL セールス電話対応者]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Marketo セールス担当者 ID]</td>
 </tr>
 <tr>
  <th rowspan="6">セールスキャンペーンに追加</th>
  <td>[!UICONTROL セールスキャンペーン名]</td>
 </tr>
 <tr>
  <td>[!UICONTROL セールス電話ステータス]</td>
 </tr>
 <tr>
  <td>[!UICONTROL セールスキャンペーン URL]</td>
 </tr>
 <tr>
  <td>[!UICONTROL 送信者]</td>
 </tr>
 <tr>
  <td>ソース</td>
 </tr>
 <tr>
  <td>[!UICONTROL セールスキャンペーン ID]</td>
 </tr>
 <tr>
  <th rowspan="6">セールスキャンペーンから削除</th>
  <td>[!UICONTROL セールスキャンペーン名]</td>
 </tr>
 <tr>
  <td>[!UICONTROL セールス電話ステータス]</td>
 </tr>
 <tr>
  <td>[!UICONTROL セールスキャンペーン URL]</td>
 </tr>
 <tr>
  <td>[!UICONTROL 送信者]</td>
 </tr>
 <tr>
  <td>ソース</td>
 </tr>
 <tr>
  <td>[!UICONTROL セールスキャンペーン ID]</td>
 </tr>
 <tr>
  <th rowspan="5">セールスメールバウンス</th>
  <td>詳細</td>
 </tr>
 <tr>
  <td>メール</td>
 </tr>
 <tr>
  <td>送信者</td>
 </tr>
 <tr>
  <td>Marketo セールス担当者 ID</td>
 </tr>
 <tr>
  <td>テンプレート ID</td>
 </tr>
</table>

## 説明 {#descriptions}

<table>
 <tr>
  <th>属性</th>
  <th>説明</th>
 </tr>
 <tbody>
 <tr>
   <td><strong>[!UICONTROL 詳細]</strong></td>
   <td>バウンスエラーメッセージの詳細。</td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL メール]</strong></td>
   <td>バウンスしたメールアドレス。</td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL リンク]</strong></td>
   <td>クリックされた URL。</td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL Marketo セールス担当者 ID]</strong></td>
   <td>[!DNL Sales Connect] の人物レコードの一意の ID。</td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL 受信者]</strong></td>
   <td>メール送信者のメールアドレス。</td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL セールス電話対応者]</strong></td>
   <td>電話に出た人の名前。</td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL セールス電話の長さ]</strong></td>
   <td>電話の長さ（秒）。</td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL セールス電話発信者]</strong></td>
   <td>電話をかけた人のメールアドレス。</td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL セールス電話録音 URL]</strong></td>
   <td>通話記録の URL。</td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL セールス電話ステータス]</strong></td>
   <td>電話の最終的な電話ステータスを保存します。このステータスには、完了、応答なし、キャンセル、失敗が含まれます。</td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL セールス電話件名]</strong></td>
   <td>ダイヤラー内でセールスユーザによって選択された電話の結果。</td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL セールスキャンペーン ID]</strong></td>
   <td>[!DNL Sales Connect] のセールスキャンペーンアセットの一意の ID。</td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL セールスキャンペーン名]</strong></td>
   <td>セールスキャンペーンの名前。</td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL セールスキャンペーン URL]</strong></td>
   <td>[!DNL Sales Connect] セールスキャンペーンの URL。</td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL セールスメール件名]</strong></td>
   <td>メールの件名行と一意の ID（例：件名（MSC-12345678）</td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL セールス電話の発信先電話番号]</strong></td>
   <td>セールスが発信した電話番号。</td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL セールステンプレート名]</strong></td>
   <td>[!DNL Sales Connect] のメールテンプレートの名前。</td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL セールステンプレート URL]</strong></td>
   <td>[!DNL Sales Connect] メールテンプレートの URL。</td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL 送信者]</strong></td>
   <td>メール送信者のメールアドレス。</td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL ソース]</strong></td>
   <td>アクティビティのソース。2021年10月のリリースより前では [!DNL Sales Connect] アクティビティは「Tout」に設定されます。2021年10月のリリースより後では [!DNL Sales Connect] アクティビティは「Sales App」に設定されます。</td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL テンプレート ID]</strong></td>
   <td>ソースが Tout の場合、テンプレート ID は [!DNL Marketo Sales Connect] テンプレート ID になります。複数のテンプレートに存在する可能性のある件名の代わりに、特定のテンプレートをターゲットにする場合に使用します。
</td>
  </tr>
 </tbody>
</table>
