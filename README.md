エディタ環境にインストールする gem を bundler で管理しようぜプロジェクト

エディタの拡張機能で使用する gem を Gemfile で管理するやつ。

* rubocop
  * https://docs.rubocop.org/rubocop/compatibility.html
* solargraph

gem が依存する gem のさらに依存する gem が高い ruby バージョンを要求するケースがあるので，明示的に gem バージョンを指定しないといけない依存 gem が存在する。そういったものを手動で解決する。

## Usage

install

```sh
gem install bundler:X.Y.Z [--no-document | --no-doc --no-ri]
bundle install
```

update

```sh
bundle update --bundler # to update bundler
bundle update # to update editor environment
# bundle clean --force # to remove unwanted gems
```
