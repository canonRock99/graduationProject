## サービス概要
言葉遊び「なぞかけ」を楽しめるアプリ。お題はランダムで表示され（変更可）、なぞかけを投稿すると採点してもらえます（ChatGPTが採点）。また、ユーザー登録をすることでマイページに作品を保存したり、出来のいい作品をランキングに投稿したりできます。


## このサービスへの思い・作りたい理由
漫談家・ねづっちさんのYouTubeチャンネルを見ていて、なぞかけを自分でも作ってみることが多くなったものの、それを他人に見てもらう機会がありませんでした。そこで、自分の作ったなぞかけを他の人に見せたり、他の人が作ったなぞかけを見ることができるアプリを作りたいと考えました。


## ユーザー層について
ねづっちさんのYouTubeチャンネルの登録者のうち、94％が男性というデータがあるようです（本人がライブでそう話している）。また、ねづっちさんに話しかけてくる人は大半が「おじさん」世代ということなので、30歳以上の男性がメインユーザーと考えています。


## サービスの利用イメージ
- なぞかけの「お題」をこちらで出すので、それをもとに作ったなぞかけを採点してもらえる→ここまではユーザー登録不要
- ユーザー登録をすると、作品を保存できる
- ユーザー登録をすると、作品を他のユーザーに見てもらえる
- ユーザー登録をすると、良い作品には「うまい！」がもらえる／他の人の作品に「うまい！」ができる


## ユーザーの獲得について
- SEO対策を施す。キーワードは「なぞかけ」「なぞかけ アプリ」など。タイトルには「なぞかけ」という言葉が入っている
- QiitaやZennに、開発に関する記事を投稿する（宣伝がメインでなければOKらしいので）


## サービスの差別化ポイント・推しポイント
なぞかけをテーマとしたアプリはすでにありますが、作り込んだものは見当たりません。また、与えられたお題に対して答えを作り、それを採点してもらうようなものもありませんので、その点で差別化されています。

また、アプリはSPA風に構成しており、DOM操作のみでコンテツが表示されるため、ページ遷移がありません。その分、表示のストレスが少なくなっています（予想）。

## 機能候補
### MVPリリース時：
- ログイン不要で、なぞかけを採点してもらえる
- ログイン機能→作品の保存、ランキングへの登録

### 本リリース以降：
- なぞかけの「ヒント」機能（ChatGPTが連想ワードを表示）
- 「なぞかけトレーニング」（～とかけて～ととく。まで与え、こころを解答してもらう）


## 機能の実装方針予定
- Googleログイン
- ChatGPT（openAI API）による採点
- 「うまい！」機能（いわゆる「いいね！」と同じ）


## その他（講師の方への連絡用・後で消します）
- アプリはすでにある程度、できあがっています（ただしバグも多い）。
使用した言語・技術はJavaScript、Firebase（Authentication、Firestore、Hosting）、Bootstrap5で、Railsはまったく使っていないのですが、これで卒業要件を満たすでしょうか（ダメなら卒業しないことも視野に入れて対応を検討します）。
- 現在はバニラJsでコードを書いていますが、Reactへの移行や、React Nativeによるネイティブアプリ化も検討中です。
- 「高度な機能」に該当するものが含まれているかどうかわかりませんが、Google Colabログインなど、上記の機能くらいではダメでしょうか？

以上、よろしくお願いします。

![スクリーンショット 2024-09-05 162237](https://github.com/user-attachments/assets/6a5c24f6-9f83-446f-860e-a0fa093530a3)
![スクリーンショット 2024-09-05 162511](https://github.com/user-attachments/assets/3de63288-13e3-4200-985b-f4e62027a388)
![スクリーンショット 2024-09-05 162601](https://github.com/user-attachments/assets/e17362b9-6d05-4704-abe7-76fdd500adb7)

