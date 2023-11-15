# Zennへの投稿の仕方

しばらく記事を書かないと忘れそうなので整理。

1. ブランチを作成

   ```
   git branch {new branch}
   ```

   ブランチを切る。
2. コマンドを用いて新規記事を作成

   ```
   npx zenn new:article
   ```

   このコマンドで/articles直下に新しく記事が作られる。
   記事の先頭にはFront-matterという記事の設定をするコマンドが作られる。これがないとアップロードに失敗する。

   本を作るときは

   ```
   npx zenn new:book
   ```

   これで/books直下に作られる。
3. Front-matterを埋める
   Front-matterはfront-matter.txtにもコピペしてあるから、articlesフォルダまたはbooksフォルダ下にファイルを新規作成して、Front-matterをコピペすればOK

   ```
   ---
   title: ""
   emoji: "🗒️"
   type: "tech" # tech: 技術記事 / idea: アイデア
   topics: []
   published: false # falseは下書き、trueは公開
   ---

   ```
4. 執筆
   Front-matterの下から描き始める
5. できたらpush
   mainブランチにpushされた時点で記事がアップロードされるっぽい。
   あとはpushするたびに更新される。

# Zenn Markdown

## リンクのカードビュー

```
@[card](url)
```

これでうまくいくはずだけど、VSCodeの設定のせいかうまくいかないから、Zennのサイト上で手直しするしかないかも。
============================================================================================================

@[card] [https://mohki7.notion.site/Mototsugu-Oki-c478f842c4de48f394e2e24b58e206bb?pvs=4](https://mohki7.notion.site/Mototsugu-Oki-c478f842c4de48f394e2e24b58e206bb?pvs=4)

これ、VSCode上だとうまく表示されないから、あとでZenn上で書き直す
