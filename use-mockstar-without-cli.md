# 非 CLI 方式

有些场景下不适合使用 CLI 命令来启动 mock server，MockStar 提供[mockstar-local-server](https://www.npmjs.com/package/mockstar-local-server)来支持。

最简单的例子详见 https://github.com/mockstarjs/mockstar/blob/master/packages/mockstar-local-server/demo/01/index.js

> 如果不需要停止服务，删除 `setTimeout` 中的代码即可。

```javascript
const path = require('path');
const mockstarLocalServer = require('mockstar-local-server');

// 服务启动参数
const configOpts = {
    rootPath: __dirname,
    mockServerPath: path.resolve(__dirname, '../../../mockstar/test/data/fixtures/mock_server/mockers'),
    watch: true
};

// 启动本地服务
const runServer = mockstarLocalServer.startServer(configOpts, (isSuccess, data) => {
    console.log('startServer callback', isSuccess, data);
});

// 3s 之后停止服务
setTimeout(() => {
    runServer.stop(() => {
        console.log('stop server success!');
    });
}, 3000);
```

