# 「Meshitero」
![meshitero](app/assets/images/logo.png)
### サービス概要
グルメ画像専用の投稿サイトです。普段何気なく撮ったグルメの画像を共有することで、お店の魅力をPRすることができます。

### 登場人物
- 自分のおすすめのレストランを広く知ってもらいたい方(グルメ好きユーザー)
- レストラン経営者の方(レストランユーザー)

### ユーザーが抱える課題
(グルメ好きユーザー)</br>
- お店を探すときに、口コミや他社の評価など情報が多すぎる
- ネガティブな情報に惑わされてしまい、新しいお店に行く機会を損失している
</br>

(レストランユーザー)

- 食べログやぐるなびでネガティブな口コミが掲載されてしまっているとお店のファンが作りにくい
- クーポンがきっかけで来店するお客はリピーターに繋がりにくい
  
### 解決方法と望む未来
(グルメ好きユーザー)

* 1枚のグルメ画像を元にレストランを探す　→新しいレストラン探しの機会創出
* 自分が大好きなレストランを他のユーザーにおすすめできる →レストランを間接的に応援することができる
</br>

(レストランユーザー)

* 自慢の料理画像1枚でお店をPRできる　→グルメ好きなユーザーに向けて積極的に情報発信することができる 
* 料理画像をきっかけに来店するユーザーが増える →純粋なお店のファンを増やすことができる

##### :fork_and_knife:　お店とグルメ好きをつなぐプラットフォームサービスを目指しています。

### サービスを作った背景
前々職で、飲食店へ送客を促すためのクーポンを提供してもらう営業を行なっておりました。クーポンやお得感をきっかけに来店された方はリピーターに繋がりにくく、それではお店のファンが作りにくいと感じていました。レストランの料理が目当てで来店した方は、その味が気に入ればリピーターになってもらう確率は上がると思いました。</br>
また私自身も飲食店を探す際に、少しでもネガティブな情報があると行きにくくなってしまうことがよくあります。評判は悪くても、実際に行ってみたら自分の好きな味でそのお店のファンになった!という経験は誰しもがあると思います。たった1枚の画像から、「美味しそう」という感性だけを頼りにレストラン探しをする機会を作りたいと思い、本アプリケーションを作成しました。


### :globe_with_meridians: URL
https://meshitero31632.herokuapp.com/

### :key: Accounts
- ベーシック認証
ID: admin</br>
Pass: 2222</br>

- テスト用アカウント/下記のURLからログインしてください</br>
- https://meshitero31632.herokuapp.com/users/sign_in
```
  email: meshitero_test@test
  password:  meshitero123
```
  


### ローカル環境のセットアップ方法
```
git clone https://github.com/yuka-sakamaki/meshitero31632.git
```
```
bundle install
```
```
#起動コマンド
rails s
```

### :page_facing_up: 主な機能

  |機能|理由|詳細|
  |:---|:---|:---|
  |新規投稿機能|ユーザーが画像とテキストを投稿することができるようにするため|ログイン状態のユーザーは画像とテキストを新たに投稿することができる|
  |新規投稿画像プレビュー機能|新規投稿する際に画像のプレビュー表示をして投稿した画像の確認ができるようにするため|ログイン状態のユーザーは画像を投稿する際に自分が選択した画像が正しいかどうかをプレビュー表示で確認することができる|
  |投稿一覧表示機能|ユーザーが投稿された画像とテキストを一覧で表示できるようにするため|ログイン状態に関わらず、投稿された画像とテキストが一覧で閲覧できる|
  |投稿内容詳細閲覧機能|ユーザーが投稿されている内容の詳細を閲覧できるようにするため。自分が投稿した内容は編集と削除のアクションをできるようにするため。|ログイン状態のユーザーは全ての投稿の詳細ページを閲覧することができる|
  |投稿編集機能|ユーザーが投稿した内容を更新できるようにするため|ログイン状態のユーザーは自分が投稿した内容のみ編集することができる|
  |投稿削除機能|ユーザーが投稿した内容を削除できるようにするため|ログイン状態のユーザーは自分が投稿した内容のみ削除することができる|
  |同じタグが紐づいている投稿の一覧表示機能|同じタグがついている投稿の一覧を表示するため|同じタグがついている投稿の一覧を表示することで、ユーザーの好きなタグがついている投稿を一覧で表示させることができる|
  |ユーザー登録機能|トップページ閲覧以外のアクションを行うためにはユーザー情報登録を必須にするため|ユーザーのニックネーム、メールアドレス、パスワード、レストラン名（任意）、レストランの住所（任意）、レストランの電話番号（任意）を登録できるようにする|
  |ユーザーログイン機能|ログインしているユーザーのみ投稿・編集・削除を有効にするため|登録済みのユーザーはメールアドレスとパスワードを入力すればログインできるようにする|
  |マイページ表示機能|ユーザーが自分が投稿した内容を一覧で閲覧できるようにするため|ログイン状態のユーザーは自分が投稿した内容が確認できるマイページを閲覧することができる|
  |ユーザー情報編集機能|ユーザーが自分が登録したニックネーム、メールアドレス、パスワード、レストラン名（任意）、レストランの住所（任意）、レストランの電話番号（任意）の内容を変更できるようにするため|マイページを閲覧しているユーザーは自分が登録した内容を変更することができる|
  |コメント投稿機能|ユーザーが自分の投稿や他のユーザーの投稿に対してコメントをつけられるようにするため|投稿詳細ページで投稿の下部にコメント入力フォームを設置し、誰がコメントしたかが分かるようにする|


### :package: Database
<img width="823" alt="スクリーンショット 2022-10-10 12 44 10" src="https://user-images.githubusercontent.com/69895997/194796596-757047e9-4520-4e18-a75a-ff993af6f2cf.png">



### :books: Version
- Ruby/Ruby on Rails/JavaScript/MySQL/Github/AWS/Visual Studio Code
* ruby 2.6.5
* Rails 6.0.3.4
* gem 3.0.3
* git version 2.24.3
* mysql  Ver 14.14 Distrib 5.6.50
* heroku/7.47.4 darwin-x64 node-v12.16.2
* AWS S3
