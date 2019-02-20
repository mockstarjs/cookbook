# mockstar.config.js 配置

| 字段名 |  类型 | 含义描述 |
| --- | --- | --- |
| `rootPath` |  `String` | 项目根目录，默认为 `mockstar.config.js` 的路径，即 `__dirname` |
| `buildPath` |  `String` | 运行路径，默认值为 `path.resolve(__dirname, './build')` |
| `logPath` |  `String` | 日志目录，默认值为 `path.resolve(__dirname, './build/logs')`  |
| `mockServerPath` |  `String` | `mocker` 所处的目录，默认值为 `path.resolve(__dirname, './mock_server')` |
| `port` |  `Number` | 端口，默认值为 `9527` |
| `watch` |  `Boolean` | 是否监听文件变化，推荐本地开发模式下使用，默认值为 `false` |

