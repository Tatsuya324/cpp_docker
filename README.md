# cpp_docker

## 注意
本リポジトリは作成者の趣味で作成したものなので動作の保証は致しません。

## 準備
### リポジトリのクローン
``` bash
git clone https://github.com/Tatsuya324/cpp_docker.git
```

### リポジトリのBUILD
``` bash
cd cpp_docker
docker-compose build
```

## 使用
### Dockerコンテナの起動（デーモン）
``` bash
cd cpp_docker
docker-compose up -d
```

### Dockerコンテナにアクセス
``` bash
docker-compose exec cpp_devel bash
```

### C++ファイルのBUILD
コンテナ内に入り、次のコマンドを実行
``` bash
cd build
cmake ..
make
```

### C++実行ファイルの実行
前項でC++ファイルをビルドした後に次のコマンドを実行
``` bash
./helloworld（実行ファイル名）
```