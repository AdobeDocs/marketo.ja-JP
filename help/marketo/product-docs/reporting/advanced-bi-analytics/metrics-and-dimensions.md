---
description: 指標とディメンション - Marketo ドキュメント – 製品ドキュメント
title: 指標およびディメンション
feature: Reporting
exl-id: 5f348007-ed0d-4900-ba4b-ecc9b935c6d2
source-git-commit: 90242f8b08b0c4773ae73134d67f571f66730878
workflow-type: tm+mt
source-wordcount: '1040'
ht-degree: 41%

---

# 指標およびディメンション {#metrics-and-dimensions}

以下に、収益サイクルエクスプローラーの分析レポートで使用できるすべての指標とディメンションを示します。

>[!TIP]
>
>いずれかの表が狭すぎると思われる場合は、このページの上部にある左矢印(![](assets/icon-left-arrow.png))と右矢印(![](assets/icon-right-arrow.png))をクリックして、左右のサイドバーを折りたたむことで、表示を拡大できます。

## ディメンションと測定 {#dimensions-and-measures}

<table>
 <tbody>
    <tr>
      <th>分析レポート</th>
      <th colspan="3" scope="colgroup">ディメンション</th>
      <th>測定（M）</th>
    </tr>
    <tr>
      <th> </th>
      <th>期間</th>
      <th>属性</th>
      <th>カスタム属性</th>
      <th> </th>
    </tr>
    <tr>
      <td>メール分析</td>
      <td>
        <ul>
          <li>四半期期間</li>
          <li>月時間枠</li>
          <li>週の時間枠</li>
          <li>日付期間</li>
          <li>週日</li>
          <li>日時間</li>
        </ul>
      </td>
      <td>
        <ul>
          <li>メール属性</li>
          <li>リード属性</li>
          <li>企業属性</li>
          <li>プログラムの属性</li>
          <li>ABM アカウント属性</li>
          <li>プログラムタグ</li>
        </ul>
      </td>
      <td>
        <ul>
          <li>カスタム会社属性</li>
          <li>カスタムリード属性</li>
        </ul>
      </td>
      <td>
        <ul>
          <li>測定（M）</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td>リード分析</td>
      <td>
        <ul>
          <li>リード作成期間</li>
          <li>商談作成の期間</li>
        </ul>
      </td>
      <td>
        <ul>
          <li>リード属性</li>
          <li>企業属性</li>
          <li>ABM アカウント属性</li>
        </ul>
      </td>
      <td>
        <ul>
          <li>カスタムリード属性</li>
          <li>カスタム会社属性</li>
        </ul>
      </td>
      <td>
        <ul>
          <li>測定（M）</li>
          <li>カスタムメジャー（M）</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td>モデル効果分析（会社）</td>
      <td>
        <ul>
          <li>期間</li>
        </ul>
      </td>
      <td>
        <ul>
          <li>モデル属性</li>
        </ul>
      </td>
      <td> </td>
      <td>
        <ul>
          <li>ステージに関する対策(M)</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td>モデル効果分析（リード）</td>
      <td>
        <ul>
          <li>期間</li>
        </ul>
      </td>
      <td>
        <ul>
          <li>リード属性</li>
          <li>モデル属性</li>
        </ul>
      </td>
      <td>
        <ul>
          <li>管理者/RCA のリード属性→</li>
        </ul>
      </td>
      <td>
        <ul>
          <li>ステージに関する対策（M）</li>
          <li>ステージ間のメジャー（M）</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td>商談分析</td>
      <td>
        <ul>
          <li>リード作成期間</li>
          <li>商談作成の期間</li>
          <li>商談クローズの期間</li>
        </ul>
      </td>
      <td>
        <ul>
          <li>ABM アカウント属性</li>
          <li>企業属性</li>
          <li>リード属性</li>
          <li>商談の属性</li>
          <li>商談のロール</li>
        </ul>
      </td>
      <td>
        <ul>
          <li>カスタム会社属性</li>
          <li>カスタムリード属性</li>
          <li>カスタム商談属性</li>
        </ul>
      </td>
      <td>
        <ul>
          <li>メジャー (M)</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td>プログラムコスト分析</td>
      <td>
        <ul>
          <li>プログラムコスト期間</li>
        </ul>
      </td>
      <td>
        <ul>
          <li>プログラムタグ</li>
          <li>プログラムの属性</li>
        </ul>
      </td>
      <td> </td>
      <td>
        <ul>
          <li>投資（分）</li>
          <li>メンバーシップ (M)</li>
          <li>成功 (M)</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td>プログラムメンバーシップ分析</td>
      <td>
        <ul>
          <li>プログラムメンバーシップの期間</li>
          <li>プログラム成功期間</li>
          <li>プログラム取得期間</li>
          <li>プログラムステータス時間枠</li>
        </ul>
      </td>
      <td>
        <ul>
          <li>プログラムの属性</li>
          <li>プログラムステータス属性</li>
          <li>企業属性</li>
          <li>リード属性</li>
          <li>ABM アカウント属性</li>
          <li>プログラムタグ</li>
        </ul>
      </td>
      <td>
        <ul>
          <li>カスタム会社属性</li>
          <li>カスタムリード属性</li>
        </ul>
      </td>
      <td>
        <ul>
          <li>プログラムのメンバーシップのメジャー（M）</li>
          <li>プログラムの成功指標（M）</li>
          <li>プログラムステータス測定（M）</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td>プログラム商談分析</td>
      <td>
        <ul>
          <li>商談の期間</li>
          <li>プログラムコスト期間</li>
        </ul>
      </td>
      <td>
        <ul>
          <li>プログラムの属性</li>
          <li>商談の属性</li>
          <li>プログラムタグ</li>
        </ul>
      </td>
      <td>
        <ul>
          <li>カスタム商談属性</li>
        </ul>
      </td>
      <td>
        <ul>
          <li>属性（分）</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td>プログラム売上高ステージ分析</td>
      <td>
        <ul>
          <li>プログラムコスト期間</li>
        </ul>
      </td>
      <td>
        <ul>
          <li>モデル属性</li>
          <li>プログラムの属性</li>
          <li>プログラムタグ</li>
        </ul>
      </td>
      <td> </td>
      <td>
        <ul>
          <li>ステージメンバーシップ （M）</li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

## 上記の分析レポートの詳細なディメンションと指標 {#detailed-dimensions-and-metrics}

### ディメンション {#dimensions}

<table>
  <tbody>
    <tr>
      <th>メール属性</th>
      <th>リード属性</th>
      <th>企業属性</th>
      <th>商談の属性</th>
      <th>プログラムの属性</th>
      <th>プログラムステータス属性</th>
      <th>ABM アカウント属性</th>
      <th>モデル属性</th>
      <th>商談のロール</th>
    </tr>
    <tr>
      <td>
          <ul>
            <li>メール名</li>
            <li>メールの件名</li>
            <li>送信元アドレス</li>
            <li>メールテンプレート</li>
            <li>メールリンク</li>
          </ul>
      </td>
      <td>
          <ul>
            <li>新規顧客獲得プログラム</li>
            <li>ブラックリスト入り</li>
            <li>商談にコンバージョン済み</li>
            <li>電話連絡拒否</li>
            <li>氏名</li>
            <li>役職</li>
            <li>マーケティング中断</li>
            <li>参照元のソース情報</li>
            <li>参照元のソースのタイプ</li>
            <li>リードパーティション</li>
            <li>ソースのタイプを登録</li>
            <li>登録解除済み</li>
            <li>メールアドレス</li>
            <li>メール無効</li>
            <li>リード所有者のメールアドレス</li>
            <li>リード所有者の職位</li>
            <li>リード所有者名</li>
            <li>リードのソース</li>
            <li>リードのステータス</li>
            <li>ドメイン名</li>
          </ul>
      </td>
      <td>
          <ul>
            <li>年間売上高</li>
            <li>請求先住所（市区町村）</li>
            <li>請求先住所 (国)</li>
            <li>請求先住所 (都道府県)</li>
            <li>請求先住所 (郵便番号)</li>
            <li>企業名</li>
            <li>業界</li>
            <li>従業員数</li>
            <li>SIC コード</li>
          </ul>
      </td>
      <td>
          <ul>
            <li>(FT) 商談成立前</li>
            <li>(FT) 商談作成日前</li>
            <li>マーケティングの影響</li>
            <li>商談のクローズ前に（MT）</li>
            <li>商談の作成前（MT）</li>
            <li>クローズした商談</li>
            <li>商談予測のカテゴリ</li>
            <li>商談名</li>
            <li>商談のステージ</li>
            <li>商談のタイプ</li>
            <li>商談の所有者名</li>
            <li>成立した商談</li>
            <li>商談確率（%）</li>
          </ul>
      </td>
      <td>
          <ul>
            <li>プログラムチャネル</li>
            <li>プログラム名</li>
          </ul>
      </td>
      <td>
          <ul>
            <li>チャネルステータスステップ</li>
            <li>ステータスが成功</li>
            <li>プログラムステータス</li>
          </ul>
      </td>
      <td>
          <ul>
            <li>ABM 国</li>
            <li>ABM CRM ID</li>
            <li>重点顧客</li>
          </ul>
      </td>
      <td>MPA_C
        <ul>
            <li>モデルはアクティブか</li>
            <li>ステージはアクティブか</li>
            <li>成功パス上</li>
            <li>トラック会社です</li>
            <li>モデル</li>
            <li>ステージ</li>
            <li>ステージタイプ</li>
         </ul>
          <p>
          MPA_L
          <ul>
            <li>上記のすべて、およびいくつかの追加</li>
            <li>直接遷移</li>
            <li>ステージがアクティブです（ステージへ）
            <li>成功パス時（ステージへ）</li>
            <li>ステージタイプ （ステージへ）</li>
          </ul>
      </td>
      <td>
          <ul>
            <li>商談に追加</li>
            <li>第一</li>
            <li>ロール</li>
          </ul>
      </td>
    </tr>
  </tbody>
</table>

<br/>

<table>
  <tbody>
    <tr>
      <th>四半期期間</th>
      <th>月期間</th>
      <th>週の期間</th>
      <th>日付期間</th>
      <th>曜日</th>
      <th>日時間</th>
    </tr>
    <tr>
      <td>
        <ul>
          <li>送信済み(四半期)</li>
          <li>配信済み（四半期）</li>
          <li>ハードバウンス（四半期）</li>
          <li>開封済み（四半期）</li>
          <li>クリック数 (四半期)</li>
          <li>登録解除済み (四半期)</li>
          <li>苦情（四半期）</li>
        </ul>
      </td>
      <td>
          <ul>
            <li>送信済み（月）</li>
            <li>配信済み (月)</li>
            <li>ハードバウンス(月)</li>
            <li>開封済み (月)</li>
            <li>クリック （月）</li>
            <li>購読解除済み（月）</li>
            <li>苦情（月）</li>
          </ul>
      </td>
      <td>
          <ul>
            <li>送信済み（週）</li>
            <li>配信済み（週）</li>
            <li>ハードバウンス (週)</li>
            <li>開封済み (週)</li>
            <li>クリック （週）</li>
            <li>購読解除済み（週）</li>
            <li>苦情（週）</li>
          </ul>
      </td>
      <td>
          <ul>
            <li>送信済み (日付)</li>
            <li>配信済み (日付)</li>
            <li>ハードバウンス(日付)</li>
            <li>開封済み (日付)</li>
            <li>クリック済み (日付)</li>
            <li>登録解除（日付）</li>
            <li>苦情（日付）</li>
          </ul>
      </td>
      <td>
          <ul>
            <li>送信済み（曜日）</li>
            <li>配信済み（曜日）</li>
            <li>ハードバウンス（曜日）</li>
            <li>開封済み（曜日）</li>
            <li>クリック （曜日）</li>
            <li>購読解除済み（曜日）</li>
            <li>苦情（曜日）</li>
          </ul>
      </td>
      <td>
          <ul>
            <li>送信済み（時刻）</li>
            <li>配信済み（時刻）</li>
            <li>ハードバウンス （1 日の時間）</li>
            <li>開封済み（時刻）</li>
            <li>クリック済み（時刻）</li>
            <li>登録解除（時刻）</li>
            <li>苦情（時刻）</li>
          </ul>
      </td>
    </tr>
  </tbody>
</table>

<br/>

<table>
  <tbody>
    <tr>
      <th>期間</th>
      <th>リード作成期間</th>
      <th>商談作成の期間</th>
      <th>商談クローズの期間</th>
      <th>プログラムコスト期間</th>
      <th>プログラムメンバーシップの期間</th>
      <th>プログラム成功期間</th>
      <th>プログラム取得期間</th>
      <th>プログラムステータスの期間</th>
    </tr>
    <tr>
      <td>
          <ul>
            <li>年</li>
            <li>四半期</li>
            <li>月</li>
            <li>週</li>
            <li>日付</li>
          </ul>
      </td>
      <td>
          <ul>
            <li>リード作成年</li>
            <li>リード作成四半期</li>
            <li>リード作成月</li>
            <li>リード作成週</li>
            <li>リード作成日</li>
          </ul>
      </td>
      <td>
          <ul>
            <li>商談作成年</li>
            <li>商談作成四半期</li>
            <li>商談作成月</li>
            <li>商談作成週</li>
            <li>商談作成日</li>
          </ul>
      </td>
      <td>
          <ul>
            <li>商談クローズ年</li>
            <li>商談クローズ四半期</li>
            <li>商談クローズ月</li>
            <li>商談クローズ週</li>
            <li>商談クローズ日</li>
          </ul>
      </td>
      <td>
          <ul>
            <li>コスト年</li>
            <li>コスト四半期</li>
            <li>コスト月</li>
          </ul>
      </td>
      <td>
          <ul>
            <li>メンバーシップ年</li>
            <li>メンバーシップ四半期</li>
            <li>メンバーシップ月</li>
            <li>メンバーシップウィーク</li>
            <li>メンバーシップ日付</li>
          </ul>
      </td>
      <td>
          <ul>
            <li>成功年</li>
            <li>成功四半期</li>
            <li>成功月</li>
            <li>成功週間</li>
            <li>成功日</li>
          </ul>
      </td>
      <td>
        <ul>
            <li>獲得年</li>
            <li>買収四半期</li>
            <li>獲得月</li>
            <li>獲得週</li>
            <li>取得日</li>
        </ul>
      </td>
      <td>
          <ul>
            <li>ステータス年</li>
            <li>ステータス四半期</li>
            <li>ステータス月</li>
            <li>ステータス週</li>
            <li>ステータス日</li>
          </ul>
       </td>
    </tr>
  </tbody>
</table>

<br/>

### 測定 {#measures}

<table>
  <tbody>
    <tr>
      <th>E メール測定</th>
      <th>リード測定</th>
      <th>ステージに関するメジャー</th>
      <th>ステージ間のメジャー</th>
      <th>投資</th>
      <th>メンバーシップ/プログラムメンバーシップの測定</th>
      <th>成功/プログラムの成功測定</th>
    </tr>
    <tr>
      <td>
        <ul>
            <li>% クリック済み</li>
            <li>クリックして開封（%）</li>
            <li>% の苦情数</li>
            <li>% 配信済み</li>
            <li>開封済み (%)</li>
            <li>% 配信停止済み</li>
            <li>クリック済み</li>
            <li>苦情</li>
            <li>配信済み</li>
            <li>ハードバウンス</li>
            <li>開封済み</li>
            <li>送信済み</li>
            <li>重複なしのクリック数</li>
            <li>登録解除済み</li>
          </ul>
      </td>
      <td>
         <ul>
            <li>コンバージョンに至っていないリードの平均年齢</li>
            <li>リードを商談にコンバージョンするまでの平均日数</li>
            <li>平均スコア</li>
            <li>リードから商談へのコンバージョン率</li>
            <li>会社から商談へのコンバージョン率</li>
            <li>企業数</li>
            <li>会社の数（商談に変換）</li>
            <li>会社の数（商談に変換されていません）</li>
            <li>リード数</li>
            <li>リードの数（商談にコンバート済み）</li>
            <li>リード数（オポチュニティに変換されていない）</li>
          </ul>
      </td>
      <td>MPA_C
        <ul>
            <li>期首残高</li>
            <li>期末残高</li>
            <li>流入</li>
            <li>流出</li>
          </ul>
        </ul>
        <p>
        MPA_L
        <ul>
            <li>平均経過時間</li>
            <li>結合/削除</li>
            <li>SLA 期限</li>
            <li>SLA 期限超過</li>
        </ul>
      </td>
      <td>
          <ul>
            <li>平均トランジション日数</li>
            <li>会話比率(すべてを選択種類)</li>
            <li>会話の割合（既存）</li>
            <li>会話率（新規）</li>
            <li>フロー</li>
            <li>流量(既存)</li>
            <li>流量(新規のみ)</li>
        </ul>
      </td>
      <td>
          <ul>
            <li>メンバーあたりのコスト</li>
            <li>新規名あたりのコスト</li>
            <li>成功あたりのコスト</li>
            <li>成功あたりのコスト（新しい名前）</li>
            <li>プログラムのコスト</li>
          </ul>
      </td>
      <td>
          <ul>
            <li>新しい名前の割合</li>
            <li>メンバー</li>
            <li>新しい名前</li>
          </ul>
      </td>
      <td>
          <ul>
            <li>成功の割合（新しい名前）</li>
            <li>成功の割合（合計）</li>
            <li>成功（新しい名前）</li>
            <li>成功（合計）</li>
          </ul>
      </td>
    </tr>
  </tbody>
</table>

<br/>

<table>
  <tbody>
    <tr>
      <th>ステージメンバーシップ （M）</th>
      <th>属性</th>
      <th>プログラムステータス測定</th>
    </tr>
    <tr>
      <td>
          <ul>
            <li>% 新しい名前（現在）</li>
            <li>% の新しい名前（今まで）</li>
            <li>ステージングまでの平均日数</li>
            <li>新しい名前あたりのコスト</li>
            <li>新規名前(現在)</li>
            <li>新規名前(これまで)</li>
          </ul>
      </td>
      <td>
          <ul>
            <li>プログラムに関連付けられた商談数</li>
            <li>（FT）商談のコスト</li>
            <li>（FT）商談作成</li>
            <li>（FT）獲得した商談</li>
            <li>（FT）創出されたパイプライン</li>
            <li>（FT）創出されたパイプライン - 進行中</li>
            <li>（FT）期待収益</li>
            <li>（FT）収益対投資</li>
            <li>（FT）獲得した売上高</li>
            <li>（MT）商談コスト</li>
            <li>（MT）商談作成</li>
            <li>（MT）獲得した商談</li>
            <li>（MT）創出されたパイプライン</li>
            <li>（MT）創出されたパイプライン - 進行中</li>
            <li>（MT）期待収益</li>
            <li>（MT）収益対投資</li>
            <li>（MT）獲得した売上高</li>
            <li>クローズした商談あたりの平均成功数</li>
            <li>作成された商談あたりの平均成功数</li>
            <li>新しい名前</li>
            <li>プログラムのコスト</li>
            <li>成功（合計）</li>
          </ul>
      </td>
      <td>
          <ul>
            <li>ステータス数（現在）</li>
            <li>ステータス数（エバー）</li>
          </ul>
      </td>
    </tr>
  </tbody>
</table>
