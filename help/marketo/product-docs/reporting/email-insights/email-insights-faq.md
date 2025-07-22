---
unique-page-id: 10100257
description: メールインサイトに関する FAQ — Marketo ドキュメント — 製品ドキュメント
title: メールインサイトに関する FAQ
exl-id: de3aca5a-08b4-4af8-ab92-675cb46dcbb2
feature: Reporting
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '602'
ht-degree: 71%

---

# メールインサイトに関する FAQ {#email-insights-faq}

## [!UICONTROL  メールインサイト ] と他のMarketo メールレポートとの比率指標に違いはありますか？ {#are-there-any-differences-between-ratio-metrics-with-email-insights-and-other-marketo-email-reporting}

はい。 [!UICONTROL  メールインサイト ] は、エンゲージメント指標の割合（開封率、クリックから開封までの割合、登録解除率）を計算する際に送信された同じメールに対して、エンゲージメント指標と、対応する配信指標を関連付けます。 例えば、[!UICONTROL  メールインサイト ] では、過去 1 週間の時系列グラフをクリック率と開封率の日次分類で調べると、対応する配信指標に基づいて、開封/クリック/購読解除イベントの真の相関関係を示すようになりました。 これは、単にすべてをまとめた Revenue Explorer の動作とは対照的です。[!UICONTROL  メールインサイト ] では、エンゲージメント率をより正確に表示します。

## [!UICONTROL  メールインサイト ] でサポートされるカスタムディメンションが 10 個のみなのはなぜですか？ {#why-does-email-insights-only-support-custom-dimensions}

多くの使用例では、追加のカスタムディメンションを 10 個含むデフォルトのシステムディメンションの拡張は、十分ではなく、セグメント化またはプログラムタグに基づくカスタムディメンションが含まれます。今後、顧客に許可されるカスタムディメンションの数を増やす予定です。

## 割り当て後にカスタムディメンションスロットを再利用できないのはなぜですか？ {#why-cant-i-re-use-custom-dimensions-slots-after-theyve-been-assigned}

特定のカスタムディメンションスロットが割り当てられた後、再マッピングすると、新しい意味をブレンドした場合に、以前のデータがエラーを生み出します。そのため、カスタムディメンションスロットは再利用できません。この動作は、他の指標分析ツール（Google Analytics など）と一致します。

## [!UICONTROL  メールインサイト ] はMarketo Sales Insightのメールをサポートしていますか？ {#does-email-insights-support-marketo-sales-insight-emails}

はい。 Marketo Sales Insights を介して送信されるすべてのメールは、[!UICONTROL  メールインサイト ] に含まれます。

## [!UICONTROL  メールインサイト ] は運用上のメールをサポートしていますか？ {#does-email-insights-support-operational-emails}

はい。デフォルトでは、オペレーショナルメールは表示とクエリには表示されません。ただし、個人設定パネルでこの設定を変更することはできます。

## [!UICONTROL  メールインサイト ] では、スケジュールされた繰り返しスケジュールされたメールやスマートキャンペーンのメールのフロー手順をキャプチャしますか？ {#does-email-insights-capture-recurring-scheduled-or-re-run-smart-campaign-email-flow-steps}

答えは、はいといいえの両方です。[!UICONTROL  メールインサイト ] の初回リリースでは、スケジュールに沿った定期的なキャンペーンや再実行のスマートキャンペーンについて、すべてのメールイベントがキャプチャされてアクセスできるようになります。 ただし、そのスマートキャンペーンの実行の違いを区別することはできません。次回のリリースでは、開封、クリック、登録解除の各イベントのスマートキャンペーン実行情報を区別のために取り込むサポートが追加されます。

## デバイスタイプまたはデバイス OS でフィルタリングすると、多くの指標がゼロと表示されるのはなぜですか？ {#why-do-many-metrics-show-zero-when-i-filter-by-device-type-or-device-os}

クリックして開封率、開封数、クリック数、登録解除数を除き、その他のサポートされる指標はすべて、配信イベントまたは配信イベントから導き出された比率です。デバイスタイプとデバイス OS はエンゲージメント指標にのみ適用されるので、表示する情報がありません。例えば、Marketo は基になる配信および送信イベントのエンゲージメント指標を受け取っていないので、「Device Type = mobile」でフィルタリングした場合、配信率を求めるクエリは未定義になります。エンゲージメント指標と配信指標の両方で構成される比率に対して、エンゲージメント指標からデバイスタイプとデバイス OS を適用する方法を研究中です。

## 特定のメールクライアントが画像をブロックする場合 [!UICONTROL  メールインサイト ] はどうなりますか？ {#what-does-email-insights-do-when-certain-email-clients-block-images}

業界の一般的な問題として、デフォルトで画像をオフにするメールクライアントが増えていることが挙げられます。画像の読み込みは、開封数の記録方法の基礎です。画像がブロックされているがテキストとリンクが完全に読み取り可能な状態で、ユーザーがメールを受け取る可能性があります。ユーザーがこのような状況を経験し、そのメールのリンクをクリックした場合、クリックイベントのシナリオが発生しますが、そのメールに対応する開封イベントは発生しません。Marketo メールインサイトは、見つからなかったイベントを自動的に生成します。このロジックは、Marketo がメールパフォーマンスレポートおよび Revenue Explorer のメール分析領域に対しておこなう処理と同じです。
