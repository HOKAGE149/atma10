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

## notebook
全てGoogle Colaboratory上で動かすことを想定しています.

以下の順番に
