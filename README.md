## 説明

pythonの開発用環境

## Usage

`docker-compose build`コマンドでdocker imageを作成します

imageが作成出来たら,`docker-compose up`コマンドでコンテナを立ち上げます

コンテナ名は固定になっています.コンテナ名が`python-rsch`になっていることを確認してください


```
docker-compose build
docker-compose up -d
```

必要なpythonライブラリがあったら,`requirements.txt`に記述してください

#### 例
```
numpy
matplotlib
```

## env
`.env`ファイルにはコンテナのマウント先のディレクトリを記述します

#### 例
```
SRC_PATH=./src
```