Google ChromeのNaitive Messageの検証用です。
以下を参考に作成しています。


https://developer.chrome.com/apps/nativeMessaging
https://medium.com/@svanas/chrome-native-messaging-example-5cf8f91cdce6
https://stackoverflow.com/questions/30880709/c-sharp-native-host-with-chrome-native-messaging

・設定方法
1. appフォルダを拡張機能として登録する
2. com.google.chrome.example.echo-win.jsonのallowed_originsに記載されているキーを1で登録したものに変更する
3. host/install_host.batを管理者権限で実行する
4. 任意の画面を開くとbtnExtContentsというボタンができているのでクリックすると、NativeHostSample.exeが実行されてブラウザから送られた文字をコールバックする。
