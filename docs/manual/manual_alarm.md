# Alarmの設定方法

![Alt text](../_img/manual/alarm_setting/2024-11-21_12h33_15.png)

AlarmはAlarm lineにRateがクロスしたタイミングでWebhookを利用し任意のメッセージを任意のプラットフォームに送信するツールです。

## 表示方法
VergeRunnerのベルアイコンをクリックするとAlarm Managerが表示されます。

![Alt text](../_img/manual/alarm_setting/2024-11-21_12h35_05.png)

## AlarmSystemの構築
ここではDiscordを使用したAlarm Systemの構築方法を記述します。

### Discordについて
Discordは、オンラインでのコミュニケーションを目的とした無料のプラットフォームです。主に音声通話、ビデオ通話、テキストチャットができ、画像や動画の共有も可能です。

サーバーというコミュニティを作成し、チャンネルで会話や通話を行います。ボットを追加して自動化やエンターテイメント機能も提供でき、役割や権限で管理もできます。ゲームのクランや趣味のグループ、ビジネスチームなど、さまざまな用途で利用されており、デスクトップ、モバイル、ブラウザで利用可能です。

### Discordのアカウントを作成
!!! info
    すでにアカウントを作成済みの方は"サーバーの作成"にお進み下さい

下記のURLからDiscordのアカウント作成画面に移動して下さい

`https://ptb.discord.com/register`

アカウント作成画面が表示されるので、必要な情報を入力後「はい」で次に進みます。

![Alt text](../_img/manual/alarm_setting/img_manual_alarm_001.png)

### サーバーの作成
ここからはサーバーの作成を行います。  
「オリジナル」を選択してください

![Alt text](../_img/manual/alarm_setting/img_manual_alarm_002.png)

!!! info
    サーバー作成画面が表示されていない場合はホーム画面左の「+」ボタンをクリックすると表示されます  

![Alt text](../_img/manual/alarm_setting/img_manual_alarm_003.png)

「自分と友達のため」を選択して下さい。

![Alt text](../_img/manual/alarm_setting/img_manual_alarm_004.png)

任意のサーバー名を入力後、新規作成ボタンを押して下さい。

![Alt text](../_img/manual/alarm_setting/img_manual_alarm_005.png)

「スキップ」を選択して下さい。

![Alt text](../_img/manual/alarm_setting/img_manual_alarm_006.png)

これでサーバーが作成できました。

### チャンネルの作成
ここからはチャンネルの作成を行います。  
一つのサーバーの中でチャンネルは複数作成することができます。  
テキストチャンネルの右にある「+」ボタンをクリックして作成画面に遷移して下さい。

![Alt text](../_img/manual/alarm_setting/img_manual_alarm_007.png)

作成画面が表示されましたら、任意のチャンネル名を入力。プライベートチャンネルにチェックを入れ「次へ」をクリックして下さい。

![Alt text](../_img/manual/alarm_setting/img_manual_alarm_008.png)

スキップをクリックして下さい。

![Alt text](../_img/manual/alarm_setting/img_manual_alarm_009.png)

これでチャンネルが作成できました。


### ウェブフックの作成

チャンネルの作成が完了しましたら、当該チャンネル横の歯車アイコンをクリックし設定画面へ遷移して下さい。

![Alt text](../_img/manual/alarm_setting/img_manual_alarm_010.png)

左側の「連携サービス」を選択し、「ウェブフックを作成」をクリックして下さい

![Alt text](../_img/manual/alarm_setting/img_manual_alarm_011.png)

初期ではCaptain_Hookというアカウントが用意されています。  
このアカウントの名前を任意のものに変更して、「ウェブフックURLをコピー」をクリックして下さい

![Alt text](../_img/manual/alarm_setting/img_manual_alarm_012.png)

!!! warning
    ウェブフックURLは他者に利用されないようにご注意下さい。

### MT4でウェブフックを設定
MT4に移動しツールバーの「ツール > オブション」をクリックして、設定画面を表示して下さい

![Alt text](../_img/manual/alarm_setting/img_manual_alarm_013.png)

エキスパートアドバイザータブをクリック

WebRequesetを許可するURLリストに先ほど作成したウェブフックURLをペーストして「OK」ボタンをクリックして下さい

![Alt text](../_img/manual/alarm_setting/img_manual_alarm_014.png)

VergeRunnerの設定画面を表示します。  
すでにチャートに配置されている場合はチャート右上の「VergeRunner」の文字をクリックすると表示されます。

![Alt text](../_img/manual/alarm_setting/img_manual_alarm_015.png)

「パラメータ入力」タブを選択

webhookの項目に先ほど作成したウェブフックURLをペーストして「OK」ボタンをクリックして下さい。

![Alt text](../_img/manual/alarm_setting/img_manual_alarm_016.png)

### 通知について
Discordはデスクトップアプリやスマートフォン向けのアプリが出ているので、導入されることをおすすめします。  
スマートフォンアプリをインストールしておくことで、PCから離れていても通知を受けることが可能になります。

!!! info
    デスクトップのDiscordアプリが立ち上がっている状態ですとスマホアプリへ通知が来ないので、スマホで通知を受け取りたい場合はデスクトップのDiscordアプリを落とした状態にして下さい。

!!! tips
    スマートウォッチなどのウェアラブルデバイスがあると、スマホを介して通知を受け取ることができるのでとっても便利です！
    
以上でAlarmSystemの構築は完了です。

## Alarmを設定する
Alarmを追加するにはAlarmウィンドウの「追加」ボタンをクリック後、チャートの任意の座標をクリックすると、Alarm Lineが表示されます。  
またAlarm毎にリストにアイテムが作成されます。  

![Alt text](../_img/manual/alarm_setting/2024-11-21_12h38_03.png)

### Alarmの有効化
黄色の状態はまだAlarmが有効化されていないことを意味します。  
Alarmウィンドウからラインに対応するアイテムの「有効化」ボタンをクリックすると緑色に変化します。  
この状態でRateがAlarm Lineと交差するとwebhookを利用して任意のプラットフォームにメッセージが送信されます。

![Alt text](../_img/manual/alarm_setting/2024-11-21_12h38_07.png)

### Alarm Lineの再編集
有効化したラインは移動することができなくなっています。  
ラインを修正したい場合は対応するアイテムの「無効化」ボタンをクリックすると再編集することができます。  
その後「有効化」ボタンをクリックしますと、Alarmが機能します。

![Alt text](../_img/manual/alarm_setting/2024-11-21_12h43_48.png)

### Alarm Lineの削除
不要になったAlarmは個別と全体で削除することができます。  
個別で削除する場合は対応するアイテムの「削除」ボタンをクリックしてください

全てのAlarm Lineを削除する場合はAlarmウィンドウの「全削除」をクリックして下さい
![Alt text](../_img/manual/alarm_setting/2024-11-21_12h44_07.png)

## 注意事項
!!! warning
    AlarmはMT4が起動されていて、VergeRunnerがチャートに配置されている状態に限ります。

    そのためMT4が落ちていたり、VergeRunnerが動作していない場合はAlarmを設定していたとしても通知は発生しません。
    
!!! warning
    Alarmの抜けたと判断する基準はラインを有効化した際のレートとの位置関係になります。
    また、MT4を再起動した場合でも、ラインの設定は残ります。
    その場合、VergeRunnerが起動したタイミングでのラインとレートの位置関係で抜けたと判断する方向が決まります。
