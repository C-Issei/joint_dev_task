# チーム開発 Rails 課題（基礎）

## 教材のご案内

- [逆転教材のテキスト教材](https://www.yanbaru-code.com/)
  - Ruby on Rails の環境構築
  - Ruby on Rails の基本 〜 resources を使ったCRUD処理の実装
- [逆転教材の動画](https://www.yanbaru-code.com/movies)
  - エンジニアになるために大切な5つの考え方【前半】 〜 動的ページと静的ページ

## 課題の提出方法

- 各課題ごとにGitHubリポジトリを作成し，プッシュして下さい。
  - 課題ディレクトリ `joint_dev_task` 内にRailsアプリを作成しないようにして下さい

## 注意点

- 課題のアプリを１つ作成する度に提出して下さい。

- 「テキスト教材」をベースに課題を進めて下さい。

- データベースは `PostgreSQL` を指定して進めて下さい。（最初の課題を除く）
  - あらかじめ `Homebrew` にインストールし，設定を行う必要があります。

```
# （参考）PostgreSQLをデータベースに指定して Rails のアプリを作成するコマンド
$ rails new アプリ名 -d postgresql
```

- `.gitignore` に次を追加し，Gitの管理下から外すようにして下さい。
  - GitHubに不要なファイルをプッシュしないようにするためです

```
.DS_Store
/vendor/bundle
```

## 課題

### Rails 課題1

「Hello World」を表示するアプリを作成し，提出して下さい。
- [【テキスト教材】Ruby on Rails で Hello World!!](https://www.yanbaru-code.com/texts/209)

### Rails 課題2

両方が完了した時点で提出して下さい。

1. `resources` を使わない「CRUDアプリ」を作成して add, commit して下さい。

- [【テキスト教材】CRUD処理の実装](https://www.yanbaru-code.com/texts/211)

2. `feature/resources` ブランチを作成して切り替え， `resources` を使った「CRUDアプリ」に修正してプルリク を出し，提出して下さい。（マージはしないで下さい！）

- [【テキスト教材】resources を使ったCRUD処理の実装](https://www.yanbaru-code.com/texts/214)

```none:手順
# 【注意】同じアプリを修正するので， rails new を再度実行しないこと

# git log, git status で add, commit できているかどうかを確認

# feature/resources ブランチを作成して切り替える
git switch -c feature/resources

# git branch で feature/resources に切り替わっていることを確認

# resources を使用した形式に変更する

# add, commit, push を実行
git add .
git commit -m "resouces を使用した形式に変更"
git push origin HEAD
```
