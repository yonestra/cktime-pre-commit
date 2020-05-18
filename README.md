# cktime-pre-commit
ローカルPCの時刻を変更していたらgit commitを止めてくれるhook

アプリのデバッグなどでローカルPCの時刻を変更(Macの場合「システム環境設定」の「日付と時刻」から)したままcommitすると、logの時刻が変更後のものになってしまう。

commit前に処理を呼べるpre-commitを利用。

※NTPサーバーから時刻を取得するのでcommitに1,2秒時間がかかるようになるのが欠点。


# Requirement
 
* macOS 10.15.2

※MacのOSのメジャーアップデートなどで動かなくなる可能性あり。
 
 
# Usage
 
とりあえずgitで開発中のプロジェクト内の.git/hook以下にpre-commitファイルをコピーすれば使えるはず。
