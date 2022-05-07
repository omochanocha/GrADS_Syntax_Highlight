# GrADS Syntax Highlight

本拡張機能は`.gs`ファイルに対してSyntax Highlight(コード中のキーワードに従って色を付ける機能)を提供するものである。ただしあくまでSyntax Highlightのみであるので、**コードの正しさは保証できない**(つまり、例えばある行がコメントアウトされていてもその行が実行されてしまう可能性もある)のでGrADSで実行する前に必ず各自で確認していただきたい。また、そのようなバグに遭遇した場合やこの単語はハイライトさせるべき！という意見があればPull requestsやIssuesを立てていただきたい。

<!-- ## インストールと使い方

--- -->

<!-- 使用するには以下の手順に従う。

**※VS Codeで`.gs`ファイルを書く人は`Remote-SSH`も使っている人だと思うので以下の手順ではそれを想定し、stormの環境で書いている。他の計算機でも使いたい場合は`scp`や`Winscp`等を使って本拡張機能を転送すれば動くはずである。`Remote-SSH`についての説明はここでは割愛するので、わからない人は他の詳しい人に聞いてほしい。**

1. 以下のコマンドで`storm`の`/work1/toida/`以下にある`grads-syntax-highlight`をあなたのホームディレクトリ以下の`vscode-server/extensions`ディレクトリにコピーする。
   * `cp -r /work1/toida/grads-syntax-highlight /home/[YOUR USER NAME]/.vscode-server/extensions/`

2. `Ctrl`(Macの人は`Command`)`+Shift+X`で拡張機能一覧を開き、`grads-syntax-highlight`がstormの欄にインストールされていることを確認する(おそらく下の方にあるはずである)。

3. VS Codeを再起動した後、最初は適当な`.gs`ファイルを開き、右下のCRLF(あるいはLF)と書かれた場所の1つ右の言語モードの選択(下の画像ではMarkdownと書かれている場所、デフォルトでは`プレーンテキスト`となっているはず)をクリックし、その後出てくるウィンドウで`'.gs'に対するファイルの関連付けの構成...`をクリックし、`GrADS`を選択する。すると今開いている`.gs`ファイルのコードがハイライトされる。<br>
   ![参考画像](https://user-images.githubusercontent.com/76525239/144768604-86f39a7a-2f8f-4262-94b4-72cb29d572ed.png)

4. 以降は`.gs`ファイルを開けば自動でハイライトしてくれるはずであるが、されない場合は上記手順3を再度行ってほしい。 -->

## Release Notes

---

### 1.0.0 (2021/12/06)

Initial release of GrADS Syntax Highlight

### 1.1.0 (2021/12/06)

ダブルクォーテーションによるバグとVS Codeのコメントアウトショートカットキー(`Ctrl` or `Command +/`)でコメントアウトができる機能の追加

### 1.2.0 (2021/12/11)

ハイライトされる単語の追加と"#"によるコメントアウトのバグの修正

### 1.2.1 (2021/12/27)

軽微なバグの修正

### 1.2.2 (2022/01/22)

指数表記のバグの修正

## 参考URL

---

* [github.devでマイナー言語のシンタックスハイライト](https://www.slideshare.net/kyusque/vscode-conference-japan-2021-kyusque)
* [vscodeで自作のシンタックスハイライト・スニペット拡張機能を作る](https://qiita.com/OrukRed/items/03f0e38e0f8553ee35d2#%E6%8B%A1%E5%BC%B5%E6%A9%9F%E8%83%BD%E3%82%92%E5%8F%96%E3%82%8A%E8%BE%BC%E3%82%80)
* [Visual Studio CodeやAtomのシンタックスハイライト拡張機能を作る](https://qiita.com/maxfie1d/items/51af2984b7a628c41a94)
* [TextMateでの正規表現ルールの日本語訳](https://macromates.com/manual/ja/regular_expressions)
* [nameの命名規則](https://macromates.com/manual/en/language_grammars)
