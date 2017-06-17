# MQL4-WebRequest
MQL4でWebRequest関数を楽に扱うためのモジュール


## Requirement
- stdlib.ex4(MT4にデフォルトで付属のLibraryファイル)


## Install
1. Web.mqhをダウンロード
2. データフォルダを開き、/MQL4/Includes/mql4_modules/Web/Web.mqhとして保存


## Usage
Web.mqhをincludeで読み込んで使用する。
GETでアクセスしたい場合はgetメソッドを呼び出す。
``` cpp
Web::get("アクセスしたいサイトのURL", 結果を受け取るstring型の変数);
```

POSTでアクセスしたい場合はpostメソッドを呼び出す。
``` cpp
Web::post("アクセスしたいサイトのURL", 結果を受け取るstring型の変数);
```

パラメータを付けてリクエストしたい場合は、事前にaddPrameterメソッドでパラメータをセットする。
``` cpp
Web::addParameter(key, value);
```

※MQL4-WebではWebRequest関数を使用しているので、事前にMT4のオプションから許可するURLリストにアクセスしたいサイトのURLを登録しておく必要があります。
