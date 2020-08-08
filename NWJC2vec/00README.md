# NWJC2vec

## Description
「国語研日本語ウェブコーパス」258億語 (2014-4Qデータ) から訓練した
word2vec および fastText による単語埋め込みデータ

## Creator
人間文化研究機構　国立国語研究所　コーパス開発センター

## Price
```
 	個人利用	団体（非営利）利用	団体（営利）利用
GSK会員	10,000円（税別）	20,000円（税別）	40,000円（税別）
非会員	20,000円（税別）	30,000円（税別）	60,000円（税別）
```

## Date
2020.9

### Format
テキストデータ

## Format.encoding
UTF-8

## Language
Japanese

## Features 

### nwjc_word_cbow_200_8_25_0_1e4_32_1_0_15.txt (GSK から公開)
word2vec による訓練 (CBOW, 200次元, 文脈長 8, 負サンプリング数 25, 階層化 softmax 0, 最低頻度閾値 1e-4, 反復回数 15)
```
word2vec -train nwjc_word.txt -output nwjc_word_1_200_8_25_0_1e4_32_0_15.txt \\ -cbow 1 -size 200 -window 8 -negative 25 -hs 0 -sample 1e-4 -threads 32 -iter 15
```

### nwjc_word_skip_200_8_25_0_1e4_6_0_15.txt.vec (GSK から公開)
fastText による訓練 (skip-gram, 200次元, 文脈長 8, 負サンプリング数 25, 階層化 softmax 0, 最低頻度閾値 1e-4, 反復回数 15)
```
fasttext skipgram -input nwjc_word.txt -output nwjc_word_skip_200_8_25_0_1e4_6_1_0_15.txt -dim 00 -ws 8 -neg 25 
```

### nwjc_word_cbow_300_8_25_0_1e4_6_1_0_15.txt.vec (GSK から公開)
fastText による訓練 (cbow, 300次元, 文脈長 8, 負サンプリング数 25, 階層化 softmax 0, 最低頻度閾値 1e-4, 反復回数 15)
```
fasttext cbow -input nwjc_word.txt -output nwjc_word_skip_300_8_25_0_1e4_6_1_0_15.txt -dim 300 -ws 8 -neg 25 
```

### nwjc_word_skip_300_8_25_0_1e4_6_1_0_15.txt.vec (GSK から公開)
fastText による訓練 (skip-gram, 300次元, 文脈長 8, 負サンプリング数 25, 階層化 softmax 0, 最低頻度閾値 1e-4, 反復回数 15)
```
fasttext skipgram -input nwjc_word.txt -output nwjc_word_skip_300_8_25_0_1e4_6_1_0_15.txt -dim 300 -ws 8 -neg 25 
```

## References 

新納 浩幸・浅原 正幸・古宮 嘉那子・佐々木 稔 (2017) nwjc2vec: 国語研日本語ウェブコーパスから構築した分散表現データ, 自然言語処理, 24(5), pp.705-720. https://doi.org/10.5715/jnlp.24.705

Masayuki Asahara (2018) NWJC2Vec: Word embedding dataset from 'NINJAL Web Japanese Corpus', Terminology:  International Journal of Theoretical and Applied Issues in Specialized Communication, 24(1), pp.7-25. https://doi.org/10.1075/term.00011.asa

## License
CC BY 4.0 https://creativecommons.org/licenses/by/4.0/deed.ja

## Credit
National Institute for Japanese Language and Linguistics (2020) NWJC2vec (2014-4Q データ)

## Contact
kotonoha@ninjal.ac.jp
