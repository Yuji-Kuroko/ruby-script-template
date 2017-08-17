# Ruby Script Template

Rubyで簡単なプログラムを書く時に便利そうなテンプレです。  
activesupportを入れているので、 `.blank?` や `.underscore` 等を使えます。

## How to use

### app/

いわゆるmodelやserviceに近いものは `app/services` 以下に入れます。  
任意でフォルダを作っても、その下のファイルは自動で読み込みされます。

### config/setting.yml

yaml形式で設定を書けます。  

```
foo:
  bar: hoge
```

と書けば、 `Settings.foo.bar` で取得可能です。

### ruby-script-template

実行ファイルです。ここの下部に追記します。  
基本的にはコピーやリネームして使用する想定です。

## How to execute

```
bundle install --path vendor/bundle
./ruby-script-template
```
