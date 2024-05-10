---
description: 質問の生成 – Marketo ドキュメント – 製品ドキュメント
title: 質問の生成
hide: true
hidefromtoc: true
feature: Dynamic Chat
source-git-commit: a6745e4a5321000bc1c91ef99c5f265b4c6c5760
workflow-type: tm+mt
source-wordcount: '409'
ht-degree: 0%

---

# 質問の生成 {#question-generation}

すべてのタスクとその有効期限の詳細（生成日時、質問の合計数、承認ステータスなど）を表示します。

## 質問の生成 {#generate-questions}

1. 「生成 AI」で、 **支援応答**.

   ![](assets/question-generation-1.png)

1. クリック **質問の生成**.

   ![](assets/question-generation-2.png)

1. タスクに名前を付け、すべてのコンテンツが抽出されるソース URL （最大 50）を入力します。 目的のトピック/キーワードを入力し、キーボードの Enter キーを押します。 完了したら、 **Generate**.

   ![](assets/question-generation-3.png)

   >[!IMPORTANT]
   >
   >Marketo Engageが指定された URL からコンテンツを削除できるようにするには、まず複数の IP アドレスを許可リストに加えるする必要があります。 [詳しくは、以下を参照してください](#ip-addresses-to-allowlist).

1. コンテンツに基づいて、質問と応答の生成には、最大 30 分かかる場合があります。 「**OK**」をクリックします。

   ![](assets/question-generation-4.png)

>[!TIP]
>
>ページ上のステータスはリアルタイムでは更新されません。 「処理中」から「完了」に変わるタイミングを確認するには、更新をクリックします。

![](assets/question-generation-5.png)

## 質問と回答のダウンロード {#download-questions-and-responses}

>[!NOTE]
>
>生成された質問と回答は、でも表示できます [応答ライブラリ](/help/marketo/product-docs/demand-generation/dynamic-chat/generative-ai/response-library.md).

1. 目的のタスクを見つけて、名前の横にあるダウンロードアイコンをクリックします。

   ![](assets/question-generation-6.png)

1. ブラウザーでダウンロードフォルダーを見つけて、ファイルを選択します。 ブラウザーによって表示が異なる場合があります。

   ![](assets/question-generation-7.png)

1. Excel ファイルで、 **タスクの詳細** 質問や回答を追加/編集する方法を含む、タスクに関する様々な詳細を示します。

   ![](assets/question-generation-8.png)

   >[!NOTE]
   >
   >質問や回答を一括編集する場合、 [再アップロードする方法については、こちらを参照してください。](/help/marketo/product-docs/demand-generation/dynamic-chat/generative-ai/response-library.md).

1. この **質疑応答（&amp;R）** タブには、生成された質問や回答など、追加の詳細が表示されます。

   ![](assets/question-generation-9.png)

## 許可リストへの IP アドレス {#ip-addresses-to-allowlist}

質疑応答の際に URL からコンテンツを抽出できるようにするには、以下のすべての IP アドレスが Web チームによって許可リストに加えるされていることを確認してください。

<table width="150">
  <tr>
    <td>20.167.0.149</td>
  </tr>
  <tr>
    <td>20.248.129.111</td>
  </tr>
  <tr>
    <td>20.167.0.146</td>
  </tr>
  <tr>
    <td>20.167.0.205</td>
  </tr>
  <tr>
    <td>20.248.135.80</td>
  </tr>
  <tr>
    <td>20.92.173.115</td>
  </tr>
  <tr>
    <td>20.167.0.195</td>
  </tr>
  <tr>
    <td>20.248.128.31</td>
  </tr>
  <tr>
    <td>20.167.1.48</td>
  </tr>
  <tr>
    <td>20.167.1.63</td>
  </tr>
  <tr>
    <td>20.167.1.92</td>
  </tr>
  <tr>
    <td>20.167.1.155</td>
  </tr>
  <tr>
    <td>20.248.135.132</td>
  </tr>
  <tr>
    <td>20.248.135.108</td>
  </tr>
  <tr>
    <td>20.248.134.140</td>
  </tr>
  <tr>
    <td>20.167.1.242</td>
  </tr>
  <tr>
    <td>20.167.0.198</td>
  </tr>
  <tr>
    <td>20.248.133.185</td>
  </tr>
  <tr>
    <td>20.248.134.190</td>
  </tr>
  <tr>
    <td>20.167.1.254</td>
  </tr>
  <tr>
    <td>20.248.128.118</td>
  </tr>
  <tr>
    <td>20.248.131.252</td>
  </tr>
  <tr>
    <td>20.167.0.188</td>
  </tr>
  <tr>
    <td>20.167.0.201</td>
  </tr>
  <tr>
    <td>20.211.64.11</td>
  </tr>
  <tr>
    <td>20.76.243.87</td>
  </tr>
  <tr>
    <td>20.76.244.212</td>
  </tr>
  <tr>
    <td>20.76.245.48</td>
  </tr>
  <tr>
    <td>20.76.245.76</td>
  </tr>
  <tr>
    <td>20.76.246.63</td>
  </tr>
  <tr>
    <td>20.76.246.146</td>
  </tr>
  <tr>
    <td>20.76.246.248</td>
  </tr>
  <tr>
    <td>20.76.247.92</td>
  </tr>
  <tr>
    <td>20.76.247.134</td>
  </tr>
  <tr>
    <td>20.76.247.244</td>
  </tr>
  <tr>
    <td>20.93.168.10</td>
  </tr>
  <tr>
    <td>20.93.168.44</td>
  </tr>
  <tr>
    <td>20.93.168.137</td>
  </tr>
  <tr>
    <td>20.93.169.20</td>
  </tr>
  <tr>
    <td>20.93.169.115</td>
  </tr>
  <tr>
    <td>20.93.169.214</td>
  </tr>
  <tr>
    <td>20.93.170.130</td>
  </tr>
  <tr>
    <td>20.93.170.138</td>
  </tr>
  <tr>
    <td>20.93.170.149</td>
  </tr>
  <tr>
    <td>20.93.172.63</td>
  </tr>
  <tr>
    <td>20.93.173.217</td>
  </tr>
  <tr>
    <td>20.93.173.243</td>
  </tr>
  <tr>
    <td>20.93.174.120</td>
  </tr>
  <tr>
    <td>20.93.174.159</td>
  </tr>
  <tr>
    <td>20.105.224.16</td>
  </tr>
  <tr>
    <td>20.10.235.102</td>
  </tr>
  <tr>
    <td>20.10.235.103</td>
  </tr>
  <tr>
    <td>20.10.235.143</td>
  </tr>
  <tr>
    <td>20.10.235.146</td>
  </tr>
  <tr>
    <td>20.10.235.147</td>
  </tr>
  <tr>
    <td>20.10.235.148</td>
  </tr>
  <tr>
    <td>20.10.235.188</td>
  </tr>
  <tr>
    <td>20.10.235.189</td>
  </tr>
  <tr>
    <td>20.10.235.246</td>
  </tr>
  <tr>
    <td>20.10.235.248</td>
  </tr>
  <tr>
    <td>20.10.235.255</td>
  </tr>
  <tr>
    <td>20.10.236.96</td>
  </tr>
  <tr>
    <td>20.10.236.97</td>
  </tr>
  <tr>
    <td>20.10.236.110</td>
  </tr>
  <tr>
    <td>20.10.236.111</td>
  </tr>
  <tr>
    <td>20.10.235.254</td>
  </tr>
  <tr>
    <td>20.10.236.138</td>
  </tr>
  <tr>
    <td>20.10.236.139</td>
  </tr>
  <tr>
    <td>20.10.236.140</td>
  </tr>
  <tr>
    <td>20.10.236.141</td>
  </tr>
  <tr>
    <td>20.10.236.84</td>
  </tr>
  <tr>
    <td>20.10.236.85</td>
  </tr>
  <tr>
    <td>20.10.236.86</td>
  </tr>
  <tr>
    <td>20.10.236.87</td>
  </tr>
  <tr>
    <td>20.119.144.14</td>
  </tr>
  <tr>
    <td>20.75.41.107</td>
  </tr>
  <tr>
    <td>20.75.43.104</td>
  </tr>
  <tr>
    <td>20.75.43.107</td>
  </tr>
  <tr>
    <td>20.75.43.113</td>
  </tr>
  <tr>
    <td>20.75.43.124</td>
  </tr>
  <tr>
    <td>20.75.43.204</td>
  </tr>
  <tr>
    <td>20.75.43.207</td>
  </tr>
  <tr>
    <td>20.75.43.214</td>
  </tr>
  <tr>
    <td>20.75.43.220</td>
  </tr>
  <tr>
    <td>20.75.44.0</td>
  </tr>
  <tr>
    <td>20.75.44.9</td>
  </tr>
  <tr>
    <td>20.75.44.52</td>
  </tr>
  <tr>
    <td>20.75.44.66</td>
  </tr>
  <tr>
    <td>20.75.44.82</td>
  </tr>
  <tr>
    <td>20.75.44.105</td>
  </tr>
  <tr>
    <td>20.75.44.108</td>
  </tr>
  <tr>
    <td>20.75.44.133</td>
  </tr>
  <tr>
    <td>20.75.44.135</td>
  </tr>
  <tr>
    <td>20.75.44.137</td>
  </tr>
  <tr>
    <td>20.75.44.147</td>
  </tr>
  <tr>
    <td>20.75.44.154</td>
  </tr>
  <tr>
    <td>20.75.44.195</td>
  </tr>
  <tr>
    <td>20.75.44.198</td>
  </tr>
  <tr>
    <td>20.75.45.32</td>
  </tr>
  <tr>
    <td>20.119.136.14</td>
  </tr>
  <tr>
    <td>172.177.93.157</td>
  </tr>
  <tr>
    <td>52.252.22.155</td>
  </tr>
  <tr>
    <td>20.62.18.64</td>
  </tr>
  <tr>
    <td>52.179.234.0</td>
  </tr>
  <tr>
    <td>52.179.234.1</td>
  </tr>
  <tr>
    <td>52.179.237.99</td>
  </tr>
  <tr>
    <td>52.179.237.148</td>
  </tr>
  <tr>
    <td>52.252.23.246</td>
  </tr>
  <tr>
    <td>52.253.64.47</td>
  </tr>
  <tr>
    <td>52.253.64.124</td>
  </tr>
  <tr>
    <td>52.253.64.125</td>
  </tr>
  <tr>
    <td>52.253.65.84</td>
  </tr>
  <tr>
    <td>52.253.65.85</td>
  </tr>
  <tr>
    <td>52.254.103.240</td>
  </tr>
  <tr>
    <td>52.253.65.92</td>
  </tr>
  <tr>
    <td>52.253.65.93</td>
  </tr>
  <tr>
    <td>52.177.89.135</td>
  </tr>
  <tr>
    <td>52.253.69.207</td>
  </tr>
  <tr>
    <td>52.253.69.240</td>
  </tr>
  <tr>
    <td>52.167.19.211</td>
  </tr>
  <tr>
    <td>52.177.147.229</td>
  </tr>
  <tr>
    <td>40.65.238.53</td>
  </tr>
  <tr>
    <td>52.177.147.249</td>
  </tr>
  <tr>
    <td>20.44.83.102</td>
  </tr>
  <tr>
    <td>52.177.148.19</td>
  </tr>
  <tr>
    <td>20.49.97.17</td>
  </tr>
  <tr>
    <td>20.14.171.7</td>
  </tr>
  <tr>
    <td>172.177.93.157</td>
  </tr>
  <tr>
    <td>20.213.91.77</td>
  </tr>
  <tr>
    <td>20.105.150.224</td>
  </tr>
  <tr>
    <td>13.68.17.252</td>
  </tr>
</table>