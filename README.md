# eggts-pkg

一个使用 pkg 打包 eggjs(ts 版本)的示例

## 初始化项目

### 1.0.0-使用脚手架初始化 eggjs 项目

```shell
npm init egg --type=ts
```

### 1.0.1-安装依赖

```shell
npm i
```

### 1.0.2-测试运行

```shell
npm run dev
```

### 1.0.3创建测试用静态文件并配置 egg-etag

```shell
npm install egg-etag
```

在`plugin.ts`中增加配置启用`egg-etag`

```ts
  etag: {
    package: 'egg-etag',
  },
```

## QuickStart

### Development

```bash
$ npm i
$ npm run dev
$ open http://localhost:7001/
```

Don't tsc compile at development mode, if you had run `tsc` then you need to `npm run clean` before `npm run dev`.

### Deploy

```bash
$ npm run tsc
$ npm start
```

### Npm Scripts

- Use `npm run lint` to check code style
- Use `npm test` to run unit test
- se `npm run clean` to clean compiled js at development mode once

### Requirement

- Node.js 8.x
- Typescript 2.8+
