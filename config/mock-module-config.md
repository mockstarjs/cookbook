# mock module 的 config.json 配置

> 这些参数都不是必填的参数，可以根据需要进行配置。

| 字段名 |  类型 | 含义描述 |
| --- | --- | --- |
| `name` |  `String` | 名字，命名规范参考 [package.json#name](https://docs.npmjs.com/files/package.json#name) ，默认为文件夹的文件名 |
| `description` |  `String` | 简要描述 |
| `priority` |  `Number` | mock server管理端页面中的列表排序权重，值越大则会越靠前展示，默认值为 `0` |
| `delay` |  `Number` | 延时多久返回，如果是 `0`，则不做延时，单位为 `ms` |
| `match` | `Object` | 匹配规则，请求中需要携带的额外数据，必须同时命中这个匹配规则，才算匹配了这个 `mockModule` |
