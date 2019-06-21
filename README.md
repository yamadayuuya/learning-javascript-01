# learning-javascript-01

テクノロジー（藤原）JavaScriptの練習 (1)

## Q1の回答「コメントを解除したことで、どう変化しましたか？」

こんにちは！という通知のような物が出てきた

## Q2の回答「エラーの原因は何でしょうか？（調べてみましょう）」

参照エラー：ウィンドウが定義されていません

## Chromeデベロッパーツール：Consoleの実行結果

```
const prefList = ["北海道", "青森"];
undefined
for (let i = 1; i <= 5; i++){
    console.log("チンカス");
}
5breadcrumbs.js:58 チンカス
undefined
for (let i = 1; i <= 5; i++){
    console.log(i);
}
breadcrumbs.js:58 1
breadcrumbs.js:58 2
breadcrumbs.js:58 3
breadcrumbs.js:58 4
breadcrumbs.js:58 5
undefined
vendor.eb1e43fd.js:1 WebSocket connection to 'wss://nexus-websocket-a.intercom.io/pubsub/5-nFJJ1KBtSJHDa0fUj4Hgy4JaoCBQYqW1iR43gG7t-HNprE5nY5vrrIyzVext0gXPVrYwxu85udyyY2BrfROLgHqBgfiYMYEKDGfm?X-Nexus-New-Client=true&X-Nexus-Version=0.4.66&user_role=user' failed: WebSocket is closed before the connection is established.
(anonymous) @ vendor.eb1e43fd.js:1
setTimeout (async)
a._startConnectTimeout @ vendor.eb1e43fd.js:1
a._initWebSocket @ vendor.eb1e43fd.js:1
a.reconnectNow @ vendor.eb1e43fd.js:1
(anonymous) @ vendor.eb1e43fd.js:1
setTimeout (async)
a.scheduleReconnect @ vendor.eb1e43fd.js:1
a._onClose @ vendor.eb1e43fd.js:1
vendor.eb1e43fd.js:1 WebSocket connection to 'wss://nexus-websocket-a.intercom.io/pubsub/5-nFJJ1KBtSJHDa0fUj4Hgy4JaoCBQYqW1iR43gG7t-HNprE5nY5vrrIyzVext0gXPVrYwxu85udyyY2BrfROLgHqBgfiYMYEKDGfm?X-Nexus-New-Client=true&X-Nexus-Version=0.4.66&user_role=user' failed: WebSocket is closed before the connection is established.
(anonymous) @ vendor.eb1e43fd.js:1
setTimeout (async)
a._startConnectTimeout @ vendor.eb1e43fd.js:1
a._initWebSocket @ vendor.eb1e43fd.js:1
a.reconnectNow @ vendor.eb1e43fd.js:1
(anonymous) @ vendor.eb1e43fd.js:1
setTimeout (async)
a.scheduleReconnect @ vendor.eb1e43fd.js:1
a._onClose @ vendor.eb1e43fd.js:1
(anonymous) @ vendor.eb1e43fd.js:1
setTimeout (async)
a._startConnectTimeout @ vendor.eb1e43fd.js:1
a._initWebSocket @ vendor.eb1e43fd.js:1
a.reconnectNow @ vendor.eb1e43fd.js:1
(anonymous) @ vendor.eb1e43fd.js:1
setTimeout (async)
a.scheduleReconnect @ vendor.eb1e43fd.js:1
a._onClose @ vendor.eb1e43fd.js:1
for (let i = 1; i <= 5; i++){
    console.log(i+"チンカス");
}
breadcrumbs.js:58 1チンカス
breadcrumbs.js:58 2チンカス
breadcrumbs.js:58 3チンカス
breadcrumbs.js:58 4チンカス
breadcrumbs.js:58 5チンカス
undefined
prefList[0]
"北海道"
const number = 1;
undefined
number =2;
VM408:1 Uncaught TypeError: Assignment to constant variable.
    at <anonymous>:1:8
(anonymous) @ VM408:1
```

## ターミナルの実行結果

```
yamadamasakinoMacBook-Pro:~ boshy$ cd fujiwara
yamadamasakinoMacBook-Pro:fujiwara boshy$ git clone git@github.com:yamadayuuya/learning-javascript-01.git
Cloning into 'learning-javascript-01'...
remote: Enumerating objects: 10, done.
remote: Counting objects: 100% (10/10), done.
remote: Compressing objects: 100% (8/8), done.
remote: Total 10 (delta 0), reused 7 (delta 0), pack-reused 0
Receiving objects: 100% (10/10), done.
You have new mail in /var/mail/boshy
yamadamasakinoMacBook-Pro:learning-javascript-01 boshy$ node node-main.js
/Users/boshy/Documents/fujiwara/learning-javascript-01/node-main.js:1
window.alert("Hello, Node.js!!");
^

ReferenceError: window is not defined
    at Object.<anonymous> (/Users/boshy/Documents/fujiwara/learning-javascript-01/node-main.js:1:1)
    at Module._compile (internal/modules/cjs/loader.js:774:30)
    at Object.Module._extensions..js (internal/modules/cjs/loader.js:785:10)
    at Module.load (internal/modules/cjs/loader.js:641:32)
    at Function.Module._load (internal/modules/cjs/loader.js:556:12)
    at Function.Module.runMain (internal/modules/cjs/loader.js:837:10)
    at internal/main/run_main_module.js:17:11
You have new mail in /var/mail/boshy
yamadamasakinoMacBook-Pro:learning-javascript-01 boshy$ node node-main.js
/Users/boshy/Documents/fujiwara/learning-javascript-01/node-main.js:1
window.alert("Hello, Node.js!!");
^

ReferenceError: window is not defined
    at Object.<anonymous> (/Users/boshy/Documents/fujiwara/learning-javascript-01/node-main.js:1:1)
    at Module._compile (internal/modules/cjs/loader.js:774:30)
    at Object.Module._extensions..js (internal/modules/cjs/loader.js:785:10)
    at Module.load (internal/modules/cjs/loader.js:641:32)
    at Function.Module._load (internal/modules/cjs/loader.js:556:12)
    at Function.Module.runMain (internal/modules/cjs/loader.js:837:10)
    at internal/main/run_main_module.js:17:11
You have new mail in /var/mail/boshy
yamadamasakinoMacBook-Pro:learning-javascript-01 boshy$ node node-main.js
/Users/boshy/Documents/fujiwara/learning-javascript-01/node-main.js:1
window.alert("Hello, Node.js!!");
^

ReferenceError: window is not defined
    at Object.<anonymous> (/Users/boshy/Documents/fujiwara/learning-javascript-01/node-main.js:1:1)
    at Module._compile (internal/modules/cjs/loader.js:774:30)
    at Object.Module._extensions..js (internal/modules/cjs/loader.js:785:10)
    at Module.load (internal/modules/cjs/loader.js:641:32)
    at Function.Module._load (internal/modules/cjs/loader.js:556:12)
    at Function.Module.runMain (internal/modules/cjs/loader.js:837:10)
    at internal/main/run_main_module.js:17:11
You have new mail in /var/mail/boshy
yamadamasakinoMacBook-Pro:learning-javascript-01 boshy$ 
```

