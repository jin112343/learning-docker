# learning-docker: Dockerの練習

## ミニレポート

### Q1-1: 同じ `docker container run` コマンドを2回実行すると、1回目と2回目で違いはありますか？どう違いますか？

１回目は「Ubuntu：latest localの画像が見つかりません」と言われて、2度目Hello Worldがechoされた

### Q1-2: なぜ違いますか？

イメージをダウンロードする必要があったから？

### Q1-3: `docker container ls` と `docker container ls -a` はどう違いますか？

docker container ls -aを実行すると何分か履歴が表記されている

### Q1-4: `docker image ls` と `docker container ls -a` はどう違いますか？（間違ってもいいので、自分の考えを述べてください）

1-3同様に何分か履歴が表記されている

### Q1-5: `ubuntu` イメージでの `cat /etc/issue` の結果をペーストしてください

Ubuntu 18.04.3 LTS \n \l

### Q1-6: `docker image ls` と `docker container ls -a` はどう変化しましたか？

docker container ls -aは/ bin / bash コマンドを実行した履歴が残っていた

### Q2-1: `-d` (デタッチド・モード) でコンテナを起動すると、どのような状態になりましたか？

特に変化なし

### Q2-2: http://localhost/ をブラウザで開くと、何が表示されましたか？

「nginxへようこそ！このページが表示されたら、nginx Webサーバーは正常にインストールされ動作しています。さらに設定が必要です。

オンラインドキュメントとサポートについては、nginx.orgを参照してください。商用サポートはnginx.comで利用できます。

nginxをご利用いただきありがとうございます。」

### Q2-3：コンテナの起動時と終了時で、docker container ls -aはどのように変化しましたか？

TATUSとPORTSに表示されるものが変わっ ている自分の環境では STATUSがup 6 minutes(6分間起動中)からExited (0) 16 seconds ago(16秒前に離脱) PORTSでは0.0.0.0:80->80/tcpが消えている

### Q3-1: `docker build -t sample-image .` 実行時に表示されている `building...` は、Dockerfileのどの行から実行されましたか？

RUN echo "building...

### Q3-2: `docker run sample-image` を実行すると、どうなりましたか？
サンプルイメージが作られた

