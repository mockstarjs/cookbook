# mocker 的 config.json 配置

> 参数中除了 `route` 必填之外，其他的都不是必填的参数，可以根据需要进行配置。

| 字段名 |  类型 | 含义描述 |
| --- | --- | --- |
| `name` |  `String` | 名字，命名规范参考 [package.json#name](https://docs.npmjs.com/files/package.json#name) ，默认为文件夹的文件名 |
| `description` |  `String` | 简要描述 |
| `route` |  `String` | 需要处理的路由，只有匹配到这个路由，才会被处理 |
| `routeExtra` |  `Object` | 额外的路由匹配参数 |
| `host` |  `String` | 还未支持 |
| `disable` |  `Boolean` | 是否为禁用状态，一旦设置为 `true`，则将忽略该 `mocker`，而是去请求现网 |
| `activeModule` |  `String` | 当前激活的 `mockModule` 数据模块的 `name` 值 |
| `defaultModule` |  `String` | 初始化时设置的 `activeModule` |
| `method` |  `String` | `http` 请求方式，包括 `get`(默认) 和 `post`  |
| `plugin` |  `String` | 数据mock的方式，包括 `xhr`(默认) 和 `async`  |
| `priority` |  `Number` | mock server管理端页面中的列表排序权重，值越大则会越靠前展示，默认值为 `0` |
| `tags` | `Array` | mock server管理端页面中的标签，用于分组管理 `mocker`，字符串数组 |







