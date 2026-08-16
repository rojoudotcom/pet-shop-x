# みんなのペットショップ

犬・猫などのペットを紹介する、静的な HTML のデモサイトです。
GitHub チーム運用（DevOps）研修の演習で使います。

## セットアップ

1. このリポジトリを clone します
2. `index.html` をブラウザで開きます（サーバーは不要です）

## 使い方

- `index.html` がペットの一覧ページです
- `pets/` の下に、ペット 1 種ごとの紹介ページを置きます
- ページを追加したら、`index.html` の一覧にリンクを足します

## 開発ルール

1. まず Issue を立てます（`.github/ISSUE_TEMPLATE` のテンプレートを使います）
2. 作業用のブランチを作ります

   ```bash
   git switch -c feature/issue-<番号>
   ```

3. 変更を記録して送ります

   ```bash
   git add <変更したファイル>
   git commit -m "<変更の内容>"
   git push -u origin feature/issue-<番号>
   ```

4. Pull Request を出し、本文に `Closes #<番号>` と書きます（Issue が自動で閉じます）
5. レビューと CI が通ったら main にマージします

### `.github/workflows` の `.draft` について

`ci.yml.draft` と `deploy.yml.draft` は、研修の演習で皆さん自身に有効化していただくファイルです。
`.draft` が付いているあいだ、GitHub はこれらをワークフローとして読みません。
演習③・⑥でファイル名から `.draft` を消すと、その瞬間に動き始めます。

## 困ったときは

研修中は講師に挙手で聞いてください。研修後は Issue を立ててください。

---

この README は「概要 → セットアップ → 使い方 → 開発ルール」の型で書いています。
参考: [GitHub Docs「About READMEs」](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/about-readmes)・[Standard Readme](https://github.com/RichardLitt/standard-readme)・[Make a README](https://www.makeareadme.com/)
