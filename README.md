Faker-Japanese
==============

概要
----

日本語ユーザに関する偽の情報をランダムに生成するためのライブラリ

使い方
------

### 名前の生成

 * フルネーム

        20.times do
          name = Faker::Japanese::Name.name
          puts "#{name} (#{name.yomi})"
        end
 
        直江津 儀子 (ナオエツ ノリコ)
        桜本 ひさゑ (サクラモト ヒサヱ)
        棚橋 重隆 (タナハシ シゲタカ)
        明王 白村 (ミョウオウ ハクソン)
        金 義弘 (キン ヨシヒロ)
        岩坪 正太郎 (イワツボ ショウタロウ)
        鎌ヶ谷 哲司 (カマガヤ テツシ)
        種本 徹子 (タネモト テツコ)
        倉谷 増美 (クラタニ マスミ)
        毒島 健夫 (ブスジマ タケオ)
        高樹 俊之丞 (タカキ トシノジョウ)
        国原 英次 (クニハラ エイジ)
        赤泊 優里 (アカドマリ ユリ)
        江袋 武治 (エブクロ タケジ)
        水城 長世 (ミズキ ナガヨ)
        マーソン ふじこ (マーソン フジコ)
        丸谷 安広 (マルタニ ヤスヒロ)
        雅 国次 (ミヤビ クニツグ)
        水科 史 (ミズシナ フミ)
        大重 栄四郎 (オオシゲ エイシロウ)

 * 苗字と名前

        20.times do
          first_name = Faker::Japanese::Name.first_name
          last_name = Faker::Japanese::Name.last_name
          puts "姓：#{last_name}\t名：#{first_name}"
        end

        姓：高垣        名：芳人
        姓：尾関        名：きね子
        姓：夜久野      名：利常
        姓：飯星        名：邦則
        姓：草柳        名：大造
        姓：納米        名：ナツコ
        姓：金高        名：喜久蔵
        姓：キーティング        名：秋江
        姓：島居        名：悦二郎
        姓：戸河内      名：さかえ
        姓：片里        名：朝長
        姓：上依知      名：洌
        姓：湧井        名：宗矩
        姓：隆速        名：美禅
        姓：相島        名：孝次郎
        姓：佐浦        名：捷平
        姓：余川        名：嘉康
        姓：増野        名：ひろふみ
        姓：国頭        名：智賀子
        姓：嶋田        名：光次郎

### 住所の生成

(まだ実装されていません。)

要件
----

 * faker
 * naist-jdic-utf8 (ソースからインストールする場合のみ)


インストール
------------

### gem からインストール

        gem install faker-japanese

### ソースからインストール

        rake generate
        rake install

問題
----

 * 典型的ではない氏名がたまに生成される (「マッカーサー」「茶魔」等)
 * 本家 Faker に比べてデータの量が多すぎる

ライセンス
----------

### naist-jdic-utf8 のライセンス

LISENCE.naist-jdic-utf8 に明記してあります。
何か問題があれば tily05@gmail.com までご連絡ください。

### このライブラリのライセンス

ライセンスのことよくがよく分かっていないのであとで書きます。

