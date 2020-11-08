# linebot-template


### Step 2

Tap the deploy button.

[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy?template=https://github.com/naomichi0904/linesimple)

## 概要

JavaでLINEBOTを作成する際のテンプレート

line-bot-sdk-javaのsample-spring-boot-kitchensinkを元に作成

　https://github.com/line/line-bot-sdk-java/tree/master/sample-spring-boot-kitchensink
 
・メインアプリケーション以外のプロジェクトを削除

・不要と思われるファイルをできるだけ削除

・build.gradleを修正

　ー親プロジェクトと子プロジェクトのbuild.gradleをマージ
 
　ーcheckstyleやspotbugsの適用除外

・.gitignoreを修正

・channel_token, channel_secretを環境変数として外出しする形式に変更

・ローカルデバッグ用のapplication_local.ymlを追加

・SampleController.javaに残している機能はhandleTextContent(シンプルなテキストメッセージ)のロジックだけ


## テンプレート使用時の注意点

・プロジェクト名に合わせて、settings.gradleの記載を変更

・SampleXXX.javaというファイル名はプロジェクトに合わせて適宜変更

・channel_tokenとchannel_secretは、環境変数として外出しする前提

　外出ししない場合はapplication.ymlに直接記載
　
