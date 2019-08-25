# 概要

#### Dockerイメージ（apache + php + MySQL）

    Docker-ComposeでLAMP環境を生成します。
    - Apache 2.4 SSL
    - PHP 7.3 (日本語対応)
    - MySQL 5.7
    - phpMyAdmin

#### 動作環境

    Docker環境で実行します。

# 利用方法

#### Docker-Compose で起動

    - 1.「docker-compose.yml」格納ディレクトリに移動
        $ cd 【格納ディレクトリ】
        
        例）
        $ cd d:/WORK/docker-lamp
    
    - 2.コンテナ起動
        $ docker-compose up -d

    - 3.動作確認
        ブラウザから接続
            ・http://192.168.99.100/
            ・http://192.168.99.100:8080/   ※phpMyAdmin root/root
        
        補足）サーバのIPアドレスはDockerで確認
        $ docker-machine ip

    - 4.コンテナ停止・削除
        $ docker-compose stop
        $ docker-compose rm -f
