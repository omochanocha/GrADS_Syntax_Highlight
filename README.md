# GrADS Syntax Highlight

本拡張機能は`.gs`ファイルに対してsyntax highlight(コード中のキーワードに従って色を付ける機能)を提供するものである。ただしあくまでsyntax highlightのみである、したがってコードの正しさを保証するものではない（つまり、例えばある行がコメントアウトされていてもその行が実行されてしまう可能性もある）のでGrADSで実行する前に必ず各自で確認していただきたい。また、そのようなバグに遭遇した場合や私の知らない重要単語でハイライトさせるべき！という意見があればぜひ樋田に伝えてほしい、できる限り早く対応します。

## インストールと使い方

使用するには以下の手順に従う。

**※GrADSを使うのは主に研究室の計算機で、またVS Codeで`.gs`ファイルを書く人は`Remote-SSH`も使っている人だと思うので以下の手順ではそれを想定している。`Remote-SSH`についてわからない人は他の詳しい人に聞いてほしい。**

1. 以下のコマンドで`storm`の`/work1/toida/`以下にある`grads-syntax-highlight`をあなたのホームディレクトリ以下の`vscode-server/extensions`ディレクトリにコピーする。
   * `cp -r /work1/toida/grads-syntax-highlight /home/[YOUR USER NAME]/.vscode-server/extensions/`

2. `Ctrl+Shift+X`で拡張機能一覧を開き、`grads-syntax-highlight`が表示されていることを確認する。

3. 適当な`.gs`ファイルを開き、右下のCRLF(あるいはLF)と書かれた場所の1つ右の言語モードの選択をクリックし、`GrADS`を選択する。表示されない場合はVSCodeを再起動すると表示されるはずである。そうすると、今開いている`.gs`ファイルのコードがハイライトされる。

4. 以降は`.gs`ファイルを開けば自動でハイライトしてくれるはずであるが、されない場合は言語モードの選択で`GrADS`を逐一選択してほしい。

## Release Notes

### 1.0.0 (2021/12/06)

Initial release of GrADS Syntax Highlight
