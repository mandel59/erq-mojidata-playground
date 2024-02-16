# セットアップ

Erq と Mojidata で遊ぶための準備をしましょう。

1. Git をセットアップします。

   - [Git のセットアップ](https://docs.github.com/ja/get-started/getting-started-with-git/set-up-git)の手順に従ってセットアップしてください。
   - Git はバージョン管理システムです。ここでは、Erq と Mojidata で遊ぶのに必要なファイルをダウンロードするために使います。
   - Git のいいところは、ただファイルをダウンロードできるだけではなく、最新版に更新するのが簡単だというところです。

2. Node.js をセットアップします。

   - [Node.js](https://nodejs.org/en)から Node.js をダウンロードし、インストールしてください。
   - LTS 版と最新版がありますが、よく分からなければ、LTS 版を選ぶといいと思います。
   - Node.js は、JavaScript で作られたアプリケーションを動かすために使います。`mojidata`コマンドや`erq`コマンドは JavaScript で作られていて、動かすのに Node.js が必要です。

3. jq をセットアップします。

   - [jq](https://jqlang.github.io/jq/) から jq をダウンロードし、インストールしてください。
   - `jq`は、JSON データを扱うためのコマンドです。ここでは、`mojidata`コマンドの出力を見やすくするために使います。

4. ターミナルを起動します。

   > [!TIP]
   >
   > Windows を使っている人は、Git Bash を起動してください。

5. コマンドを入力して、このリポジトリをクローン（ダウンロード）します。

   - コマンド: `git clone https://github.com/mandel59/erq-mojidata-playground.git`
   - [リポジトリのクローン](https://docs.github.com/ja/repositories/creating-and-managing-repositories/cloning-a-repository) の手順に従ってクローンしてください。

6. クローンしたリポジトリに移動します。

   - コマンド: `cd erq-mojidata-playground`

7. NPM を使って、依存ライブラリをインストールします。
   - コマンド: `npm install`

これで遊ぶ準備ができました！
