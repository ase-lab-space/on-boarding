# 運営の`@ase-lab.space`メール発行までの手順

ここでは運営のメール発行までの手順を説明します．

ASE-Lab.では，運営メールにGmailのエイリアス機能を使っています．簡単に言えば，すでにお持ちのあなたのGmailを`@ase-lab.space`として使うことができるようにする，というものです．もちろん元のGmailが使えなくなるようなことはありません．

ここでは本田大明を例にとって実際にやりながら説明していきます．

> ### 【参考】エイリアスとは
> メールエイリアスとは、**主要なメールアドレスに紐づいた、別名のメールアドレス**です。エイリアスを持つことで、1つの受信トレイで複数のアドレスを管理でき、**プライベートなメールアドレスを隠したり、用途別にメールを仕分けたりするのに役立ちます**。

> ##### メールエイリアスの主な特徴
> * 主要アドレスと共通の受信ボックス: エイリアスに届いたメールは、すべて主要なメールアドレスの受信トレイに届きます。
> * 同じパスワード: エイリアスと主要アドレスは同じパスワードを共有します。
> * 送信元アドレスの選択: メール送信時に、エイリアスを送信元として選択できます。
> * プライバシーの保護: ウェブサイトの登録などにエイリアスを使うことで、主要なメールアドレスを非公開にできます。
> * メールの仕分け: 仕事用、買い物用など用途別にエイリアスを使い分けることで、メールの管理がしやすくなります。

## 転送のために使うGmailメールアドレスを，ソフトウェア管理者に伝える

現在はソフトウェア管理者は本田大明なので，SlackでHiroaki HondaにDMでGmailを教えてください．こちら側で設定を行います．

```plain
例: 運営のGmailを発行するから，Gmailを教えます！よろしく！
hddamin6844@gmail.com
```

伝えられた`@ase-lab.space`メールアドレスを覚えておいてください．（例: `hiroaki.honda@ase-lab.space`）

## 送信された認証メールを認証する

設定の途中で，お伝えしてくれたメール宛に確認メールを送ります．そのメールにあるボタンを押してください．押した後にGoogle Domainのページに飛びますが，すぐにタブを閉じてしまって大丈夫です．

## App passwordを発行する

Gmail上でエイリアス設定をするには，App passwordというものが必要になります．それを発行する手順を説明します．

まず，<https://myaccount.google.com/apppasswords> にいきます．

名前に`ase-lab.space`を入力し，`Create`を押します．

そうすると，16文字のパスワードが表示されるかと思います．これをコピーしてどこかに保存しておいてください．下の手順の中で使います．

これでタブは閉じても構いません．

## Gmailのエイリアス設定をする

実際にGmailの中での設定をします．

まず，<https://mail.google.com> に行き，右上の`Settings`から`See all settings`を押します．`Accounts and Import`タブを押し，下の`Send mail as`欄の中の`Add another email address`を押します．

ここから黄色い画面に進むかと思います．ここからは画面ごとに入力内容を順番に示します．

1. Enter information about your other email address.
    - Name: 相手に表示されたい名前
        - ASE-Lab.運営の皆様はアルファベットで (First Name) (Family name)の順で登録してください
        - 例: Hiroaki Honda
    - Email address: `伝えられたase-lab.spaceのメールアドレス
        - 例: `hiroaki.honda@ase-lab.space`
    - Treat as an alias: チェックを入れる

2. Send mail through your SMTP server
    - SMTP Server: `smtp.gmail.com`
    - Username: 今サインインしているGmailアカウントのメールアドレス
        - 例: `hdddamin6844@gmail.com`
    - Password: 先ほど発行した16桁のApp password
        - 例: `abcdefghijklmnop`
    - Secured connection using TLS: チェックを入れる

## 確認メールを承認する

<https://mail.google.com> に行き，確認メールが来ていることを確認し，承認します．

## 完了

これにて終了です！これにて，`@ase-lab.space`としてメールを送受信することができるようになりました！

- メールを受信した場合，エイリアス登録した元のGmailのメールボックスと一緒に送信されます．

- メールを送信したい場合，<https://mail.google.com> に行き，メールを作成する画面の中で`From`の行に行き，誰として送りたいかを選択することで`@ase-lab.space`として送信することが可能になります．

何かわからないことがあったら，遠慮せずソフトウェア管理者（現在は本田大明）へSlackなどでお聞きください．

参考: <https://support.google.com/domains/answer/9437157>
