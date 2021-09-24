# AutoML-Time-Series

- AutoML-Time-Series を活用した時系列解析のプログラム

## リポジトリ構成
```
.
├── README.md
├── data
│   └── AirPassengers.csv
├── docker
│   ├── darts
│   │   ├── Dockerfile
│   │   └── requirements.txt
│   └── sktime
│       ├── Dockerfile
│       └── requirements.txt
├── docker-compose-darts.yml
├── docker-compose-sktime.yml
├── docs
├── models
├── notebooks
│   ├── Auto_TS_example.ipynb
│   ├── darts
│   │   ├── 01-darts-intro.ipynb
│   │   ├── 02-multi-time-series-and-covariates.ipynb
│   │   ├── 03-data-processing.ipynb
│   │   ├── 04-FFT-examples.ipynb
│   │   ├── 05-RNN-examples.ipynb
│   │   ├── 06-TCN-examples.ipynb
│   │   ├── 07-Transformer-examples.ipynb
│   │   ├── 08-NBEATS-examples.ipynb
│   │   ├── 09-DeepAR-examples.ipynb
│   │   ├── 10-DeepTCN-examples.ipynb
│   │   ├── 11-Kalman-filter-examples.ipynb
│   │   ├── 12-GP-filter-examples.ipynb
│   │   ├── 13-Dynamic-Time-Warping-example.ipynb
│   │   ├── FFT.ipynb
│   │   ├── Multi-Time-Series-Forecasting-Darts.ipynb
│   │   ├── Time-Series-Forecasting-Darts.ipynb
│   │   └── future-covariates-example.ipynb
│   └── sktime
│       └── Time-Series-Forecasting-sktime.ipynb
├── src
│   └── __init__.py
├── tests
│   └── __init__.py
└── work
```

## 環境構築

- Dockderfileがあるホスト側のフォルダへ移動（例：Desktop/AutoML-Time-Series）

```
cd Desktop/AutoML-Time-Series
```

- Dockerによる環境構築（フォルダをマウント：Desktop/AutoML-Time-Series）

```
docker-compose -f docker-compose-{*構築対象}.yml up --build
```

- ブラウザーを立ち上げてlocalhost:8888へアクセス
- ローカルフォルダがマウントされている

## Display notebooks

- [View Jupyter notebooks in nbviewer](https://nbviewer.jupyter.org/github/ykato27/AutoML-Time-Series/tree/main/notebooks/)

## 動作環境
マシンスペック（Mac)
- MacBook Air (Retina, 13-inch, 2018)
- 1.6 GHz デュアルコアIntel Core i5
- 8 GB 2133 MHz LPDDR3
