# Local Chat Messenger
ローカルシステムで動作するシンプルなチャットメッセンジャーを実装しました。
同じマシン上で動作するサーバ（server.py）とクライアント（client.py）、UNIX ドメインソケットを介してメッセージを送受信するプログラムです。

# 概要
サーバ側では、まずソケットをAF_UNIXという通信形式で作成しました。これは同じコンピュータ上で通信を行うための通信形式です。今回はSOCK_STREAMのタイプで作っています。これはTCP通信をサポートするソケットタイプです。
それから、UNIX ドメインのアドレスにバインドします。
その後、クライアント側からの接続を待つようにします。クライアントから接続があると通信を
始めます。
CLIから実行できて、server.pyを実行したのちにclient.pyを実行することで動きます。

# 作成環境
WSL+ubuntu+Vscode


