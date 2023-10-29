
# ECOSNAP(エコスナップ)

<img width="521" alt="web" src="https://github.com/jphacks/OL_2316/assets/105538719/36b80003-3357-43b7-89a0-755cd59c7394">




## 製品概要

ECOSNAPは、
__ゴミの画像から瞬時にリサイクル方法を教えてくれる革新的なエコシステムサービス__
です。

ゴミのリサイクル方法がわからないというユーザーの課題を解決し、持続可能な社会への一歩を踏み出します。
### 背景(製品開発のきっかけ、課題等）

皆さんは、日常生活で家の掃除やゴミの処理をしていて、

__「このゴミってどうやって処理するんだっけ？」__

__「このゴミってリサイクルできるのかな？」__


と困った経験はありますか？

<br>

<br>



 その際
__「ゴミの処理方法やリサイクル方法をその都度ネットで調べるのが面倒だ」__
という課題があります。

ゴミの処理方法がわからないと以下のようなデメリットがあります。

* __ゴミの処理方法がわからずに家に置きっぱなしにしてしまう__

* __誤ったゴミの分別をしてしまい、環境に悪影響を及ぼす__

* __リサイクルできる製品を捨ててしまう__



<br>


<ins>__ゴミにはさまざまな種類があり、処分方法は非常に複雑なのです。__</ins>


<br>


そこで私たちは、上記の悩みを解決し、
ゴミの処理・リサイクル方法をより手軽に判別する

__「ECOSNAP(エコスナップ)」__

を開発しました。


### 製品説明（具体的な製品の説明）
ECOSNAPには、YOLOv8にオリジナルデータを使って学習モデルを構築し、
__ゴミに特化した物体検知システム__
を使用しています！

ゴミの種類を
__「瞬時に」__
判別し、リサイクル方法を表示します!

さらに、ゴミの分別やリサイクル方法だけでなく、正しい処理方法によるCO2削減量も表示しています！

### 使い方
使い方は簡単で2つのステップでゴミの判別結果を見ることができます！
1. ゴミの写真をアップロードします。
<img width="560" alt="uplode" src="https://github.com/jphacks/OL_2316/assets/105538719/5e7c52ef-81e4-4cf7-858f-b543314eecc3">

2. 判別されたゴミの分類、リサイクル方法、CO2削減量を確認します。
<img width="1364" alt="result" src="https://github.com/jphacks/OL_2316/assets/105538719/7c3c1716-b177-4c35-87a8-1a9e3fd230c0">


これらの手順は非常に
__シンプル__
で、ユーザーの目線に立って、単純な作業だけで結果が見られるように設計しました！

### 特長
#### 1. 特長1　

文字で調べることなく、
__「画像のみ」__
でゴミを判別することができます。

ゴミの名前を検索するとそのリサイクル方法が出てきますが、

__画像を読み込むだけでリサイクル方法を表示するシステム__
はまだ世にリリースされていません！

#### 2. 特長2 

ゴミに特化したオリジナルの物体検知モデルを使用しています。

YOLOはデフォルトのモデルだと、ゴミのジャンルを区別することが難しいため、

今回は自分たちでゴミの写真を集め、実際にモデルを作ってみました。

#### 3. 特長3

### 解決出来ること
* ゴミの種類がわからないという問題を
__簡単かつスムーズに__
解決できる！
* ゴミのリサイクル方法が簡単に分かることで、
__環境にやさしい社会づくり__
に貢献できる！
### 今後の展望
私たちが開発したECOSNAPは、
__「ゴミの処理方法やリサイクル方法を調べることが面倒」__
という問題を解決しました。

次の目標は、
__より多くのユーザーを対象としたサービス提供__
です。

具体的な以下の機能を実装します。
1. カメラで直接読み取れる機能
2. 判別できるゴミの種類を追加
3. スマートフォン版の実装
4. ゴミのリサイクル辞書の追加

### 注力したこと（こだわり等）
*  自分たちのチームで物体検知用のゴミの画像を集め、
    __オリジナルの物体検知モデル__
   を作成しました。
* ユーザー目線に立ってデザインをシンプル化し、ページ遷移も最小限に抑えました。
  

## 開発技術
### 活用した技術
#### API・データ
*  チームのペットボトル撮影データ

#### フレームワーク・ライブラリ・モジュール
*  フロントエンド
*    HTML, CSS
* バックエンド
*   Django(Django~=3.2.10)
* 機械学習
*   Google Colab
*   YOLOv8n(ultralytics)
* 環境開発整備
*   VSCode
  

#### デバイス
* デバイス: PC (Windows, MacBook)
* 

### 独自技術
#### ハッカソンで開発した独自機能・技術
#### 画像検知を使ったリサイクル方法の表示
現在世に出ているゴミの処理方法は文章で調べるシステムしかありません。

そこでゴミの名前がわからないシーンや調べる作業が面倒なシーンを想定して、画像をアップロードするだけで検知するサービスを開発しました。

これによりゴミの処理を調べる手間を省きました！
#### オリジナル物体検出モデル
YOLOの通常の物体検知モデルはゴミの画像を詳細に検知することはできません。

そこでゴミの判別ができるように独自で学習用データを用意し、オリジナル物体検知モデルを作成しました。
これにより、さまざまなゴミを検知して表示することができます。

<br>

(例)通常のYOLOではペットボトルを読み込むと、「bottle」としか表示されませんが、

私たちのチームで開発したオリジナルモデルでは、「petbottle」と表示できるようになっています！

<br>

![petbottle](https://github.com/jphacks/OL_2316/assets/105538719/42a78e37-d7ba-4605-8294-c5afd97138c1)




#### プロダクト開発
私たちのチームはFigmaで事前に新規性や独創性を持ったアイデアをチームで発散し、新規性あふれるアイデアを設定することができました。

また、開発にあたって必要な機能をFigmaでチームに書き出すことで、開発をスムーズに進めることができました
<img width="441" alt="idea" src="https://github.com/jphacks/OL_2316/assets/105538719/89aac5ac-4d32-41bd-b1d9-866e5c62a730">


#### デザイン
私たちはFigmaでデザインを行い、チーム内でプロダクトのデザインや画面遷移の共通認識を持つことで、開発をスムーズに進めました。
<img width="561" alt="design" src="https://github.com/jphacks/OL_2316/assets/105538719/a256bd34-d8a3-44b2-a7b0-50d529b3f343">

#### タスク管理
また、タスクはFigmaで書き出して管理し、Slackでタスクに関する不明点や新たなタスクを共有しました。
<img width="818" alt="task" src="https://github.com/jphacks/OL_2316/assets/105538719/04dd7d3d-4727-4ea2-af9c-90bc514ae4bd">



#### 作業・進捗管理
Zoomを使用して一定時間ごとに進捗管理と連絡事項の確認を行いました。

