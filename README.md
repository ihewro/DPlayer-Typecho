## DPlayer-Typecho
[DPlayer](https://github.com/DIYgod/DPlayer) for typecho

### 使用方式


PJAX 回调函数

```javascript
            if ('undefined' == typeof(dPlayerOptions) || 'undefined' == typeof(dPlayers)) {
                return;
            }
            var len = dPlayerOptions.length;
            for(var i=0;i<len;i++){
                dPlayers[i] = new DPlayer({
                    element: document.getElementById('player' + dPlayerOptions[i]['id']),
                    screenshot: false,
                    autoplay: dPlayerOptions[i]['autoplay'],
                    video: dPlayerOptions[i]['video'],
                    theme: dPlayerOptions[i]['theme'],
                    danmaku: dPlayerOptions[i]['danmaku'],
                });
                // dPlayers[i].init();
            }
```
