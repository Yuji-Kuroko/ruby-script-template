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

### bin/console

デバッグ用コンソールを開きます。

### bin/sample_command

サンプル実行ファイルです。
適切なファイル名やクラス名にリネームしてください。

## How to execute

```
bundle install --path vendor/bundle
bin/sample_command sample
```
