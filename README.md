# pythonの開発環境の構築
***(構築が済んでいるなら飛ばしてください)***<br>
まずは以下のリンクより、python3をインストールしてください。<br>
[python3.12のインストール](https://apps.microsoft.com/detail/9NCVDN91XZQP?ocid=pdpshare&hl=en-us&gl=US)<br>
これがインストール出来たら、スタート メニュー (左下の Windows アイコン)からwindows powershellを起動し、**Python --version**と入力し、Enterを押します。<br>
すると、以下のように表示されます。このように表示されていたらインストール成功です。
![python--version.png](https://github.com/kimshun0213kr/dice_and_caps/blob/main/src/python--version.png)<br>
windows powershellで**Python --version**と実行した結果(筆者の場合、バージョンが3.10.7であることが分かる。)<br>
このようにしてpythonがインストールされていることを確認したら、以下のリンクよりVisual Studio Codeをインストールしてください。<br>
[Visual Studio Codeのインストール](https://code.visualstudio.com/sha/download?build=stable&os=win32-x64-user)<br>
インストール出来たら、以下のリンクより、日本語化パッケージとPython用の拡張機能をダウンロードしてください。<br>
[Japanese Language Pack for Visual Studio Code](https://marketplace.visualstudio.com/items?itemName=MS-CEINTL.vscode-language-pack-ja)<br>
[python用拡張機能](https://marketplace.visualstudio.com/items?itemName=ms-python.python)<br>
ダウンロード出来たら、Visual Studio Codeを起動しましょう。
起動出来たら、Python 3 インタープリターを選択します。コマンド パレットを開き (**Ctrl + Shift + P**)、検索するコマンド「**Python: Select Interpreter**」の入力を開始して、コマンドを選択します。<br>
![PythonSelect Interpreter-1](https://github.com/kimshun0213kr/dice_and_caps/blob/main/src/Python_Select_Interpreter-1.png)<br>
「Python: Select Interpreter」と打ち込み、エンター<br>
![PythonSelect Interpreter-2](https://github.com/kimshun0213kr/dice_and_caps/blob/main/src/Python_Select_Interpreter-2.png)<br>
表示されたpythonを選択<br>

## pip コマンドの使用方法
### パッケージをインストールするとき
パッケージのインストールの際は、以下のコマンドを使用する。
```bash
pip install パッケージ名
```
例えば[pandas](https://pandas.pydata.org/docs/user_guide/index.html)をインストールする際は以下のようにpower shell上で実行する。
```bash
pip install pandas
```

### パッケージのアンインストール
パッケージのアンインストールをする際は以下のコマンドを使用する。
```bash
pip uninstall パッケージ名
```
途中で以下のように聞かれるので、その際はyと入力し、Enterを押すことでアンインストール作業が継続される。
```bash
Proceed (Y/n)? y
```
また、途中でのこの確認が面倒である場合には、先述のアンインストールコマンドの末尾に" -y"とつければよい。
```bash
pip uninstall パッケージ名 -y
```
