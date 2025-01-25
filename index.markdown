---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
title: 『国語研日本語ウェブコーパス』
permalink: /

---
## 概要
『国語研日本語ウェブコーパス』はウェブを母集団として100 億語規模を目標として構築した日本語コーパスです。 ウェブ（WWW）上の日本語テキストを利用して100億語を超える規模の現代日本語コーパスを構築することによって、稀言語現象の言語学的、心理学的および情報処理的視点からの究明の可能性を開くことを目的としています。 具体的な応用として、言語研究のための用例収集、日本語使用実態の定量的な把握などを想定しています。

## プロジェクト『超大規模コーパス』プロジェクト
『国語研日本語ウェブコーパス』および『梵天』は、国立国語研究所コーパス開発センター『超大規模コーパス』プロジェクト(2011年-2015年)により作成されました。

---


- 語彙表データ：　　　　　[https://github.com/masayu-a/NWJC/](https://github.com/masayu-a/NWJC/)
- NWJC-n-gram：　　　　　[https://www.gsk.or.jp/catalog/gsk2020-c/](https://www.gsk.or.jp/catalog/gsk2020-c/)
- NWJC2vec：　　　　　　　[https://www.gsk.or.jp/catalog/gsk2020-d/](https://www.gsk.or.jp/catalog/gsk2020-d/)
- NWJC-BERT：　　　　　　[https://www.gsk.or.jp/catalog/gsk2020-e/](https://www.gsk.or.jp/catalog/gsk2020-e/)
- chiVe（Sudachi とNWJCによる日本語単語ベクトル：ワークス社）　[https://github.com/WorksApplications/chiVe/](https://github.com/WorksApplications/chiVe/)
- chiTra（SudachiとNWJCによるTransformerモデル：ワークス社） [https://github.com/WorksApplications/SudachiTra/](https://github.com/WorksApplications/SudachiTra/)
- whole-NWJC：   『国語研日本語ウェブコーパス』全データ

----
## whole-NWJC『国語研日本語ウェブコーパス』全データについて

情報解析用途のために『国語研日本語ウェブコーパス』全データを共同研究先に共有します(2024年
8月～)。

- [whole-NWJC:『国語研日本語ウェブコーパス』全データ](https://doi.org/10.51094/jxiv.836)

| [1st 1億URL] | 2012-4Q | 2013-1Q | 2013-2Q | 2013-3Q |
|-------------|---------|---------|---------|---------|
| warcファイル数   | 910     | 878     | 910     | 906     |
| ファイルサイズ     | 842GB   | 813GB   | 844GB   | 838GB   |

| [2nd 1億URL] | 2013-4Q | 2014-1Q | 2014-2Q | 2014-3Q |
|-------------|---------|---------|---------|---------|
| warcファイル数   | 998     | 437     | 1021    | 608     |
| ファイルサイズ     | 928GB   | 407GB   | 952GB   | 562GB   |

| [3rd 1億URL] | 2014-4Q | 2015-1Q | 2015-2Q |
|-------------|---------|---------|---------|
| warcファイル数   | 907     | 874     | 20      |
| ファイルサイズ     | 845GB   | 812GB   | 19GB    |

### データの利用方法
NWJC (whole-NWJC) の利用を希望する方は、事前に利用可能性を問い合わせのうえ、
共同利用型共同研究（c）に申請をお願いいたします。
[https://www.ninjal.ac.jp/research/cfp/jupc/](https://www.ninjal.ac.jp/research/cfp/jupc/)


企業の方は共同研究契約を結ぶことで利用が可能です。

本件問い合わせ先： masayu-a@ninjal.ac.jp

----

## 『国語研日本語ウェブコーパス』(2014-4Q) データについて

### データの基礎統計

2014年10-12月収集データの基礎統計は以下のとおりです：

- 収集URL数	83,992,556
- 文数（のべ数）	3,885,889,575
- 文数（異なり数）	1,463,142,939
- 国語研短単位数	25,836,947,421

### データの構築方法

ウェブアーカイブの構築で用いられる Heritrix クローラを運用することで1年間にわたって3か月おきに、固定した約1億URLのウェブページを収集しました。 得られたウェブページはnwc-toolkitを用いて、日本語文抽出と正規化を行いました。 コピーサイトの問題を緩和するために、文単位の単一化（文の異なりをとること）を行いました。 形態素解析器MeCab-0.996 と形態素解析用辞書UniDic-2.1.2を用いて形態素解析を行い、 さらにUniDic 主辞規則に基づく係り受け解析器CaboCha-0.69により係り受け解析を行っています

### 利用できるデータ

2014年10-12月収集データにより構築した n-gram データ、単語埋め込みデータ、事前学習モデルなどを言語資源協会より公開します。

#### [NWJC-n-gram](https://github.com/masayu-a/NWJC/tree/master/NWJC-n-gram) [GSK2020-C](https://www.gsk.or.jp/catalog/gsk2020-c/)

#### [NWJC2vec](https://github.com/masayu-a/NWJC/tree/master/NWJC2vec) [GSK2020-D](https://www.gsk.or.jp/catalog/gsk2020-d)

#### [NWJC-BERT](https://github.com/masayu-a/NWJC/tree/master/NWJC-BERT) [GSK2020-E](https://www.gsk.or.jp/catalog/gsk2020-e)

___

## 参考文献について

### 『国語研日本語ウェブコーパス』
> 国際論文誌： Masayuki Asahara, Kikuo Maekawa, Mizuho Imada, Sachi Kato, Hikari Konishi (2014)'Archiving and Analysing Techniques of the Ultra-large-scale Web-based Corpus Project of NINJAL, Japan', Alexandria, Vol 26, No.1-2, pp.129-148.

> 国内論文誌・紀要： 浅原正幸, 今田水穂, 保田祥, 小西光, 前川喜久雄 (2014) 「Web を母集団とした超大規模コーパスの開発　収集と組織化」, 国立国語研究所論集, 7号, pp.1-26.

> 国際会議予稿集： Masayuki Asahara, Kikuo Maekawa (2013) 'Design of a Web-scale Japanese Corpus', Proc.of Conference of the Pacific Association for Computational Linguistics (PACLING-2013).

### 『梵天』
> 国内論文誌： 浅原正幸, 河原一哉, 大場寧子, 前川喜久雄 (2018) 「『国語研日本語ウェブコーパス』とその検索系『梵天』」情報処理学会論文誌, Vol 59, No. 2, pp.299-306.

> 国際会議予稿集： Masayuki Asahara, Kazuya Kawahara, Yuya Takei, Hideto Masuoka, Yasuko Ohba, Yuki Torii, Toru Morii, Yuki Tanaka, Kikuo Maekawa, Sachi Kato and Hikari Konishi (2016) ''BonTen' - Corpus Concordance System for 'NINJAL Web Japanese Corpus'' Proc. of COLING-2016 Demo Session.

### 『NWJC2vec』
> 国際論文誌： Masayuki Asahara (2018), `NWJC2Vec: Word embedding dataset from 'NINJAL Web Japanese Corpus'', Terminology: International Journal of Theoretical and Applied Issues in Specialized Communication, Vol. 24, No. 2. pp.7-25.

> 国内論文誌： 新納浩幸, 浅原正幸, 古宮嘉那子, 佐々木稔 (2017), 「nwjc2vec: 国語研日本語ウェブコーパスから構築した単語の分散表現データ」, 自然言語処理, Vol. 24, No. 5, pp.705-720.

### 『chiVe』
> 国内学会：真鍋陽俊, 岡照晃, 海川祥毅, 髙岡一馬, 内田佳孝, 浅原正幸 (2019), 「複数粒度の分割結果に基づく日本語単語分散表現」. 言語処理学会第 25 回年次大会発表論文集.

### 『NWJC-BERT』

> 国内学会： 浅原正幸, 西内沙恵, 加藤祥 (2020), 「NWJC-BERT: 多義語に対するヒトと文脈化単語埋め込みの類似性判断の対照分析」, 言語処理学会第26回年次大会発表論文集, pp.961-964.

### 『chiTra』

> 国内学会：勝田哲弘, 林政義, 山村崇, Tolmachev Arseny, 高岡一馬, 内田佳孝, 浅原正幸 (2022), 「単語正規化による表記ゆれに頑健な BERT モデルの構築」, 言語処理学会第28回年次大会発表論文集.

___

## 検索系『梵天』（**『梵天』は 2021年12月24日をもってサービスを停止しました。**）

『国語研日本語ウェブコーパス』は検索系『梵天』に格納して公開しています。

検索系として「文字列検索」「品詞列検索」「係り受け部分木検索」の3通りの検索機能を提供します。 一般公開版は「文字列検索」のみが利用できます。

フロンドエンドはコーパス管理ソフトウェア「ChaKi.NET」を参考にして、ウェブ上で動作するインターフェイスの開発を株式会社万葉に委託しました。 バックエンドには株式会社レトリバのSedue for Bigdataを用いています。

----

## 検索系「中納言」(** NWJC『中納言』は 2024年2月29日をもってサービスを停止しました。**)

『国語研日本語ウェブコーパス』の一部 (86,277,772語：NWJC-2014-4Qの0.33%)を検索系『中納言』に格納して公開しています。
