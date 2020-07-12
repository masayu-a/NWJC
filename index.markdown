---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
---
# 『国語研日本語ウェブコーパス』

## 概要
『国語研日本語ウェブコーパス』はウェブを母集団として100 億語規模を目標として構築した日本語コーパスです。 ウェブ（WWW）上の日本語テキストを利用して100億語を超える規模の現代日本語コーパスを構築することによって、稀言語現象の言語学的、心理学的および情報処理的視点からの究明の可能性を開くことを目的としています。 具体的な応用として、言語研究のための用例収集、日本語使用実態の定量的な把握などを想定しています。

## プロジェクト『超大規模コーパス』プロジェクト
『国語研日本語ウェブコーパス』および『梵天』は、国立国語研究所コーパス開発センター『超大規模コーパス』プロジェクト(2011年-2015年)により作成されました。

## 検索系『梵天』

『国語研日本語ウェブコーパス』は検索系『梵天』に格納して公開しています。

https://bonten.ninjal.ac.jp/

検索系として「文字列検索」「品詞列検索」「係り受け部分木検索」の3通りの検索機能を提供します。 一般公開版は「文字列検索」のみが利用できます。

フロンドエンドはコーパス管理ソフトウェア「ChaKi.NET」を参考にして、ウェブ上で動作するインターフェイスの開発を株式会社万葉に委託しました。 バックエンドには株式会社レトリバのSedue for Bigdataを用いています。

なお、『梵天』は 2021年9月末を持ってサービスを停止します。

## データについて

### データの基礎統計

2014年10-12月収集データを『梵天』に格納しています。格納データの基礎統計は以下のとおりです：

- 収集URL数	83,992,556
- 文数（のべ数）	3,885,889,575
- 文数（異なり数）	1,463,142,939
- 国語研短単位数	25,836,947,421

### データの構築方法

ウェブアーカイブの構築で用いられる Heritrix クローラを運用することで1年間にわたって3か月おきに、固定した約1億URLのウェブページを収集しました。 得られたウェブページはnwc-toolkitを用いて、日本語文抽出と正規化を行いました。 コピーサイトの問題を緩和するために、文単位の単一化（文の異なりをとること）を行いました。 形態素解析器MeCab-0.996 と形態素解析用辞書UniDic-2.1.2を用いて形態素解析を行い、 さらにUniDic 主辞規則に基づく係り受け解析器CaboCha-0.69により係り受け解析を行っています

### 利用できるデータ

2014年10-12月収集データにより構築した n-gram データ、単語埋め込みデータ、事前学習モデルなどを言語資源協会より公開します。

#### [NWJC-n-gram](https://github.com/masayu-a/NWJC/tree/master/NWJC-n-gram)

#### [NWJC2vec](https://github.com/masayu-a/NWJC/tree/master/NWJC2vec)

#### [NWJC-BERT](https://github.com/masayu-a/NWJC/tree/master/NWJC-BERT)

## 参考文献について

### 『国語研日本語ウェブコーパス』
- 国際論文誌： Masayuki Asahara, Kikuo Maekawa, Mizuho Imada, Sachi Kato, Hikari Konishi (2014)'Archiving and Analysing Techniques of the Ultra-large-scale Web-based Corpus Project of NINJAL, Japan', Alexandria, Vol 26, No.1-2, pp.129-148.

- 国内論文誌・紀要： 浅原正幸, 今田水穂, 保田祥, 小西光, 前川喜久雄 (2014) 「Web を母集団とした超大規模コーパスの開発　収集と組織化」, 国立国語研究所論集, 7号, pp.1-26.

- 国際会議予稿集： Masayuki Asahara, Kikuo Maekawa (2013) 'Design of a Web-scale Japanese Corpus', Proc.of Conference of the Pacific Association for Computational Linguistics (PACLING-2013).

### 『梵天』
- 国内論文誌・紀要： 浅原正幸, 河原一哉, 大場寧子, 前川喜久雄 (2018) 「『国語研日本語ウェブコーパス』とその検索系『梵天』」情報処理学会論文誌, Vol 59, No. 2, pp.299-306.

- 国際会議予稿集： Masayuki Asahara, Kazuya Kawahara, Yuya Takei, Hideto Masuoka, Yasuko Ohba, Yuki Torii, Toru Morii, Yuki Tanaka, Kikuo Maekawa, Sachi Kato and Hikari Konishi (2016) ''BonTen' - Corpus Concordance System for 'NINJAL Web Japanese Corpus'' Proc. of COLING-2016 Demo Session.

### 『NWJC2vec』
- Masayuki Asahara (2018), `NWJC2Vec: Word embedding dataset from 'NINJAL Web Japanese Corpus'', Terminology: International Journal of Theoretical and Applied Issues in Specialized Communication, Vol. 24, No. 2. pp.7-25.

### 『NWJC-BERT』
