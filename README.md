■サービス概要
推し活に特化した日記コラージュアプリで写真を加工したり可愛いフォントの文字、スタンプ、蛍光ペンで推し活の思い出を残せます。
共有しない限り公開されることがないので人目を気にせず自分だけのデコ日記が作れます。
ID交換をしたら友達追加ができ、交換日記とプロフィール帳で交流ができます。

■ このサービスへの思い・作りたい理由
元々日記コラージュへの憧れはあったが、字が汚くデザインセンスもないので折角オタ活をしても記録に残すことが出来ていませんでした。
また、推し活に関しては人によって熱量も程度も違うため棲み分けが難しく、人目を気にしてSNSにアップするのを躊躇していました。
そんな自分の経験から、自由にデコれる自分だけの推し活日記アプリがあれば素敵な思い出を残すことが出来ると考え開発に至りました。

■ ユーザー層について
メインターゲットは、推し活を楽しむ10代から30代の女性
推し活は様々ですが、可愛く写真に残したりグッズを集めたりするのは若い女性が圧倒的に多い傾向があるため需要があると考えました。

■サービスの利用イメージ
推し活の思い出を気軽で簡単に日記として残せるます。ただの記録としてではなく、見た目に特化しているので後で見返しても幸せな気持ちが蘇ります。
日記を残したい日にだけ残せば良く、自分が許可したユーザー以外に監視されることがないため自分のペースでまったり楽しく推し活ができます。
完成したコラージュ日記を画像として保存もできるので外部のSNSで共有も可能です。

■ ユーザーの獲得について
XなどのSNSを使って、自分がアプリを使って作成した推し活日記を色んなパターンで掲載し、ユーザーにアプリを使った際に可能なことを可視化して伝えます。

■ サービスの差別化ポイント・推しポイント
日記のコラージュアプリは存在しますが、推し活に特化することで自分の思い出の整理ができ、交換日記機能やプロフィール帳機能で、不特定多数ではなく特定の人物と安心して交流を楽しめます。交流といってもメッセージをリアルタイムで行ったりはできないため、いつ交換日記が返ってくるかわからない幼少期に感じたようなドキドキ感が楽しめ、返事をしないと、といったプレッシャーもなくなります。閉鎖的に自分の好きなように自己表現を行うこともでき、可愛くコラージュできたものを画像にして他のSNSに共有したり、友人間だけで閲覧しあったり、使う範囲を自在に選べます。

■ 機能候補
・MVPリリース時
ユーザー登録機能
ID検索機能
フォロー機能
文字投稿機能
公開選択機能
写真登録、投稿機能
ページネーション機能

・本リリース時
パスワードロック機能(スマホなどでアプリとして使用する際)
写真加工機能
交換日記機能
文字フォントの変更、追加やスタンプ機能
いいね機能(集計機能)
通知機能(LINE)
画像保存機能
SNSシェア機能
問い合わせ
利用規約

■ 機能の実装方針予定
Ruby on Railsで開発。Herokuで本番環境へデプロイする。
gem deviseでアカウント登録、ログイン、ログアウト機能。
gem ransackでID検索機能。
Relationsipモデルを作成し、Userモデルと関連付けてフォロー機能。
gem carrierwaveとmini_magickで写真投稿。
gem kaminariとdeviseで公開選択機能。
gem kaminariでページネーション機能。
Google Calendar APIでカレンダー情報を取得し、日付を入力しなくても自動で設定される。
Cloudinary APIで画像加工機能。
LINE Messaging APIで通知機能。