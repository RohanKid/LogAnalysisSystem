# Log Analysis System

## 目的
Wikipediaのアクセスログの情報を使い、サイトのユーザーの活動に関する質問に答えるシステムを作成
このシステムはコマンドラインから実行されるプログラムで、データベースに接続し、SQLクエリを使ってアクセスログを分析し、いくつかの質問に対する答えを出力する。

## システム説明
データは2021年12月1日のログを使用
最もビュー数の多い記事を、指定した記事数分だけビュー数が多い順にソートし、ドメインコードとページタイトル、ビュー数を提示する
（例）コマンドライン上で2記事と指定した場合、下記を表示する
”en”, “Main_Page”, 120
”en”, ”Wikipedia:Umnyango_wamgwamanda”, 112

指定したドメインコードに対して、人気順にソートし、ドメインコード名と合計ビュー数を提示する
（例）コマンドライン上で「en de」と指定した場合、下記を表示する
”en”, 10700
”de”, 5300
