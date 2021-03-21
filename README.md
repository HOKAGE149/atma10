# atmaCup10 HOKAGE's solution

[atmaCup10](https://www.guruguru.science/competitions/16/)における[HOKAGE](https://www.guruguru.science/HOKAGE149)の再現コードです.

## 概略
* モデルはLGBM
* pallete情報を画像にしてXception

## ディレクトリ構成
third_takeを例にディレクトリ構成を記します.

```
third_take
│   ├── bin
│   │   └── lid.176.bin
│   ├── model_temp
│   │   └── bert_vecs.csv
│   │   └── xlm_roberta_vecs.csv
├── input
│    └── 配布されているデータセット
├── src
│    ├── input
│    ├── output
│    ├── Public_Notebook_SSL_Color.ipynb
│    ├── run_feature.ipynb
│    ├── run_folds.ipynb
│    ├── run_rgbm.ipynb
│    └── config.yaml
├── output
└── README.md
```

* lid.176.binは, [Language identification・fastText](https://fasttext.cc/docs/en/language-identification.html)からダウンロード可能です.

## notebook
全てGoogle Colaboratory上で動かすことを想定しています.  
出力ファイルを利用するのでパスを適宜変更する必要があります.  
以下の順番に実行いただければ問題ないと思います.  


### run_folds.ipynb
GroupKFold(n_split=5)

### Public_Notebook_SSL_Color.ipynb
ディスカッションにおける[palette embedding](https://www.guruguru.science/competitions/16/discussions/fddee5ac-f7a1-4ed6-bac6-fbc81668a465/)のnotebook.
作成した画像をXceptionを用いて予測.

### run_feature.ipynb
特徴量作成

### run_rgbm.ipynb
LGBMによる学習



