# 🎨️ ACG

## AcFun <Site url="www.acfun.cn"/>

### 番剧 <Site url="www.acfun.cn" size="sm" />

<Route namespace="acfun" :data='{"path":"/bangumi/:id","categories":["anime"],"example":"/acfun/bangumi/5022158","parameters":{"id":"番剧 id"},"features":{"requireConfig":false,"requirePuppeteer":false,"antiCrawler":false,"supportBT":false,"supportPodcast":false,"supportScihub":false},"name":"番剧","maintainers":["xyqfer"],"description":":::tip\n番剧 id 不包含开头的 aa。\n例如：`https://www.acfun.cn/bangumi/aa5022158` 的番剧 id 是 5022158，不包括开头的 aa。\n:::","location":"bangumi.ts"}' :test='{"code":0}' />

:::tip
番剧 id 不包含开头的 aa。
例如：`https://www.acfun.cn/bangumi/aa5022158` 的番剧 id 是 5022158，不包括开头的 aa。
:::

### 文章 <Site url="www.acfun.cn" size="sm" />

<Route namespace="acfun" :data='{"path":"/article/:categoryId/:sortType?/:timeRange?","categories":["anime"],"example":"/acfun/article/110","parameters":{"categoryId":"分区 ID，见下表","sortType":"排序，见下表，默认为 `createTime`","timeRange":"时间范围，见下表，仅在排序是 `hotScore` 有效，默认为 `all`"},"features":{"requireConfig":false,"requirePuppeteer":false,"antiCrawler":false,"supportBT":false,"supportPodcast":false,"supportScihub":false},"name":"文章","maintainers":["TonyRL"],"description":"| 二次元画师 | 综合 | 生活情感 | 游戏 | 动漫文化 | 漫画文学 |\n  | ---------- | ---- | -------- | ---- | -------- | -------- |\n  | 184        | 110  | 73       | 164  | 74       | 75       |\n\n  | 最新发表   | 最新动态        | 最热文章 |\n  | ---------- | --------------- | -------- |\n  | createTime | lastCommentTime | hotScore |\n\n  | 时间不限 | 24 小时 | 三天     | 一周    | 一个月   |\n  | -------- | ------- | -------- | ------- | -------- |\n  | all      | oneDay  | threeDay | oneWeek | oneMonth |","location":"article.ts"}' :test='{"code":0}' />

| 二次元画师 | 综合 | 生活情感 | 游戏 | 动漫文化 | 漫画文学 |
  | ---------- | ---- | -------- | ---- | -------- | -------- |
  | 184        | 110  | 73       | 164  | 74       | 75       |

  | 最新发表   | 最新动态        | 最热文章 |
  | ---------- | --------------- | -------- |
  | createTime | lastCommentTime | hotScore |

  | 时间不限 | 24 小时 | 三天     | 一周    | 一个月   |
  | -------- | ------- | -------- | ------- | -------- |
  | all      | oneDay  | threeDay | oneWeek | oneMonth |

### 用户投稿 <Site url="www.acfun.cn" size="sm" />

<Route namespace="acfun" :data='{"path":"/user/video/:uid","radar":[{"source":["www.acfun.cn/u/:id"],"target":"/user/video/:id"}],"name":"用户投稿","parameters":{"uid":"用户 UID"},"categories":["anime"],"maintainers":["wdssmq"],"location":"video.ts"}' :test='undefined' />

## ACG17 <Site url="acg17.com"/>

### 全部文章 <Site url="acg17.com/post" size="sm" />

<Route namespace="acg17" :data='{"path":"/post/all","categories":["anime"],"example":"/acg17/post/all","parameters":{},"features":{"requireConfig":false,"requirePuppeteer":false,"antiCrawler":false,"supportBT":false,"supportPodcast":false,"supportScihub":false},"radar":[{"source":["acg17.com/post"]}],"name":"全部文章","maintainers":["SunBK201"],"url":"acg17.com/post","location":"post.ts"}' :test='{"code":0}' />

## AGE 动漫 <Site url="agemys.cc"/>

### 番剧详情 <Site url="agemys.cc" size="sm" />

<Route namespace="agefans" :data='{"path":"/detail/:id","categories":["anime"],"example":"/agefans/detail/20200035","parameters":{"id":"番剧 id，对应详情 URL 中找到"},"features":{"requireConfig":false,"requirePuppeteer":false,"antiCrawler":false,"supportBT":false,"supportPodcast":false,"supportScihub":false},"radar":[{"source":["agemys.org/detail/:id"]}],"name":"番剧详情","maintainers":["s2marine"],"location":"detail.ts"}' :test='{"code":0}' />

### 最近更新 <Site url="agemys.org/update" size="sm" />

<Route namespace="agefans" :data='{"path":"/update","categories":["anime"],"example":"/agefans/update","parameters":{},"features":{"requireConfig":false,"requirePuppeteer":false,"antiCrawler":false,"supportBT":false,"supportPodcast":false,"supportScihub":false},"radar":[{"source":["agemys.org/update","agemys.org/"]}],"name":"最近更新","maintainers":["nczitzk"],"url":"agemys.org/update","location":"update.ts"}' :test='{"code":1,"message":"AssertionError: expected 503 to be 200 // Object.is equality\n    at /home/runner/work/RSSHub/RSSHub/lib/routes.test.ts:79:41\n    at runTest (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/@vitest+runner@2.0.4/node_modules/@vitest/runner/dist/index.js:955:11)\n    at async Promise.all (index 16)\n    at runSuite (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/@vitest+runner@2.0.4/node_modules/@vitest/runner/dist/index.js:1097:13)\n    at runSuite (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/@vitest+runner@2.0.4/node_modules/@vitest/runner/dist/index.js:1111:15)\n    at runFiles (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/@vitest+runner@2.0.4/node_modules/@vitest/runner/dist/index.js:1168:5)\n    at startTests (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/@vitest+runner@2.0.4/node_modules/@vitest/runner/dist/index.js:1177:3)\n    at file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/vitest@2.0.4_@types+node@20.14.12_jsdom@24.1.1_bufferutil@4.0.8_utf-8-validate@5.0.10_/node_modules/vitest/dist/chunks/runtime-runBaseTests.Dq_sJZq9.js:132:11\n    at withEnv (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/vitest@2.0.4_@types+node@20.14.12_jsdom@24.1.1_bufferutil@4.0.8_utf-8-validate@5.0.10_/node_modules/vitest/dist/chunks/runtime-runBaseTests.Dq_sJZq9.js:94:5)\n    at run (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/vitest@2.0.4_@types+node@20.14.12_jsdom@24.1.1_bufferutil@4.0.8_utf-8-validate@5.0.10_/node_modules/vitest/dist/chunks/runtime-runBaseTests.Dq_sJZq9.js:117:3)\n    at runBaseTests (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/vitest@2.0.4_@types+node@20.14.12_jsdom@24.1.1_bufferutil@4.0.8_utf-8-validate@5.0.10_/node_modules/vitest/dist/vendor/base.Csk7BT3h.js:31:3)\n    at ForksBaseWorker.executeTests (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/vitest@2.0.4_@types+node@20.14.12_jsdom@24.1.1_bufferutil@4.0.8_utf-8-validate@5.0.10_/node_modules/vitest/dist/workers/forks.js:25:7)\n    at execute (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/vitest@2.0.4_@types+node@20.14.12_jsdom@24.1.1_bufferutil@4.0.8_utf-8-validate@5.0.10_/node_modules/vitest/dist/worker.js:116:5)\n    at onMessage (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/tinypool@1.0.0/node_modules/tinypool/dist/entry/process.js:54:20)"}' />

## CnGal <Site url="www.cngal.org"/>

### 每周速报 <Site url="www.cngal.org/" size="sm" />

<Route namespace="cngal" :data='{"path":"/weekly","categories":["anime"],"example":"/cngal/weekly","parameters":{},"features":{"requireConfig":false,"requirePuppeteer":false,"antiCrawler":false,"supportBT":false,"supportPodcast":false,"supportScihub":false},"radar":[{"source":["www.cngal.org/","www.cngal.org/weeklynews"]}],"name":"每周速报","maintainers":["chengyuhui"],"url":"www.cngal.org/","location":"weekly.ts"}' :test='{"code":0}' />

### 制作者 / 游戏新闻 <Site url="www.cngal.org" size="sm" />

<Route namespace="cngal" :data='{"path":"/entry/:id","categories":["anime"],"example":"/cngal/entry/2693","parameters":{"id":"词条ID，游戏或制作者页面URL的最后一串数字"},"features":{"requireConfig":false,"requirePuppeteer":false,"antiCrawler":false,"supportBT":false,"supportPodcast":false,"supportScihub":false},"radar":[{"source":["www.cngal.org/entries/index/:id"]}],"name":"制作者 / 游戏新闻","maintainers":["chengyuhui"],"location":"entry.ts"}' :test='{"code":1,"message":"AssertionError: expected [ …(5) ] to not include &#39;https://weibo.com/7615758653/Ominv18wd&#39;\n    at Proxy.<anonymous> (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/@vitest+expect@2.0.4/node_modules/@vitest/expect/dist/index.js:1135:17)\n    at Proxy.<anonymous> (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/@vitest+expect@2.0.4/node_modules/@vitest/expect/dist/index.js:912:17)\n    at Proxy.methodWrapper (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/chai@5.1.1/node_modules/chai/chai.js:1591:25)\n    at checkRSS (/home/runner/work/RSSHub/RSSHub/lib/routes.test.ts:65:27)\n    at processTicksAndRejections (node:internal/process/task_queues:95:5)\n    at /home/runner/work/RSSHub/RSSHub/lib/routes.test.ts:80:17\n    at runTest (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/@vitest+runner@2.0.4/node_modules/@vitest/runner/dist/index.js:955:11)\n    at async Promise.all (index 297)\n    at runSuite (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/@vitest+runner@2.0.4/node_modules/@vitest/runner/dist/index.js:1097:13)\n    at runSuite (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/@vitest+runner@2.0.4/node_modules/@vitest/runner/dist/index.js:1111:15)\n    at runFiles (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/@vitest+runner@2.0.4/node_modules/@vitest/runner/dist/index.js:1168:5)\n    at startTests (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/@vitest+runner@2.0.4/node_modules/@vitest/runner/dist/index.js:1177:3)\n    at file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/vitest@2.0.4_@types+node@20.14.12_jsdom@24.1.1_bufferutil@4.0.8_utf-8-validate@5.0.10_/node_modules/vitest/dist/chunks/runtime-runBaseTests.Dq_sJZq9.js:132:11\n    at withEnv (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/vitest@2.0.4_@types+node@20.14.12_jsdom@24.1.1_bufferutil@4.0.8_utf-8-validate@5.0.10_/node_modules/vitest/dist/chunks/runtime-runBaseTests.Dq_sJZq9.js:94:5)\n    at run (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/vitest@2.0.4_@types+node@20.14.12_jsdom@24.1.1_bufferutil@4.0.8_utf-8-validate@5.0.10_/node_modules/vitest/dist/chunks/runtime-runBaseTests.Dq_sJZq9.js:117:3)\n    at runBaseTests (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/vitest@2.0.4_@types+node@20.14.12_jsdom@24.1.1_bufferutil@4.0.8_utf-8-validate@5.0.10_/node_modules/vitest/dist/vendor/base.Csk7BT3h.js:31:3)"}' />

## COLAMANGA <Site url="www.colamanga.com"/>

### Manga <Site url="www.colamanga.com" size="sm" />

<Route namespace="colamanga" :data='{"path":"/:id","parameters":{"id":"漫画id"},"name":"Manga","maintainers":["machsix"],"example":"/colamanga/manga-qq978758","categories":["anime"],"radar":[{"source":["www.colamanga.com/:id/"],"target":"/:id"}],"features":{"requireConfig":false,"requirePuppeteer":true,"antiCrawler":true,"supportBT":false,"supportPodcast":false,"supportScihub":false},"location":"manga.ts"}' :test='{"code":1,"message":"AssertionError: expected 503 to be 200 // Object.is equality\n    at /home/runner/work/RSSHub/RSSHub/lib/routes.test.ts:79:41\n    at runTest (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/@vitest+runner@2.0.4/node_modules/@vitest/runner/dist/index.js:955:11)\n    at async Promise.all (index 307)\n    at runSuite (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/@vitest+runner@2.0.4/node_modules/@vitest/runner/dist/index.js:1097:13)\n    at runSuite (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/@vitest+runner@2.0.4/node_modules/@vitest/runner/dist/index.js:1111:15)\n    at runFiles (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/@vitest+runner@2.0.4/node_modules/@vitest/runner/dist/index.js:1168:5)\n    at startTests (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/@vitest+runner@2.0.4/node_modules/@vitest/runner/dist/index.js:1177:3)\n    at file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/vitest@2.0.4_@types+node@20.14.12_jsdom@24.1.1_bufferutil@4.0.8_utf-8-validate@5.0.10_/node_modules/vitest/dist/chunks/runtime-runBaseTests.Dq_sJZq9.js:132:11\n    at withEnv (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/vitest@2.0.4_@types+node@20.14.12_jsdom@24.1.1_bufferutil@4.0.8_utf-8-validate@5.0.10_/node_modules/vitest/dist/chunks/runtime-runBaseTests.Dq_sJZq9.js:94:5)\n    at run (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/vitest@2.0.4_@types+node@20.14.12_jsdom@24.1.1_bufferutil@4.0.8_utf-8-validate@5.0.10_/node_modules/vitest/dist/chunks/runtime-runBaseTests.Dq_sJZq9.js:117:3)\n    at runBaseTests (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/vitest@2.0.4_@types+node@20.14.12_jsdom@24.1.1_bufferutil@4.0.8_utf-8-validate@5.0.10_/node_modules/vitest/dist/vendor/base.Csk7BT3h.js:31:3)\n    at ForksBaseWorker.executeTests (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/vitest@2.0.4_@types+node@20.14.12_jsdom@24.1.1_bufferutil@4.0.8_utf-8-validate@5.0.10_/node_modules/vitest/dist/workers/forks.js:25:7)\n    at execute (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/vitest@2.0.4_@types+node@20.14.12_jsdom@24.1.1_bufferutil@4.0.8_utf-8-validate@5.0.10_/node_modules/vitest/dist/worker.js:116:5)\n    at onMessage (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/tinypool@1.0.0/node_modules/tinypool/dist/entry/process.js:54:20)"}' />

## Comicat <Site url="comicat.org"/>

### 搜索关键词 <Site url="comicat.org" size="sm" />

<Route namespace="comicat" :data='{"path":"/search/:keyword","categories":["anime"],"example":"/comicat/search/喵萌奶茶屋+跃动青春+720P+简日","parameters":{"keyword":"关键词，请用`+`号连接"},"features":{"requireConfig":false,"requirePuppeteer":false,"antiCrawler":false,"supportBT":true,"supportPodcast":false,"supportScihub":false},"name":"搜索关键词","maintainers":["Cyang39"],"location":"search.ts"}' :test='{"code":0}' />

## Comics Kingdom <Site url="comicskingdom.com"/>

### Archive <Site url="comicskingdom.com" size="sm" />

<Route namespace="comicskingdom" :data='{"path":"/:name","categories":["anime"],"example":"/comicskingdom/pardon-my-planet","parameters":{"name":"URL path of the strip on comicskingdom.com"},"features":{"requireConfig":false,"requirePuppeteer":false,"antiCrawler":false,"supportBT":false,"supportPodcast":false,"supportScihub":false},"radar":[{"source":["comicskingdom.com/:name/*","comicskingdom.com/:name"]}],"name":"Archive","maintainers":["stjohnjohnson"],"location":"index.ts"}' :test='{"code":1,"message":"AssertionError: expected 503 to be 200 // Object.is equality\n    at /home/runner/work/RSSHub/RSSHub/lib/routes.test.ts:79:41\n    at processTicksAndRejections (node:internal/process/task_queues:95:5)\n    at runTest (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/@vitest+runner@2.0.4/node_modules/@vitest/runner/dist/index.js:955:11)\n    at async Promise.all (index 309)\n    at runSuite (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/@vitest+runner@2.0.4/node_modules/@vitest/runner/dist/index.js:1097:13)\n    at runSuite (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/@vitest+runner@2.0.4/node_modules/@vitest/runner/dist/index.js:1111:15)\n    at runFiles (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/@vitest+runner@2.0.4/node_modules/@vitest/runner/dist/index.js:1168:5)\n    at startTests (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/@vitest+runner@2.0.4/node_modules/@vitest/runner/dist/index.js:1177:3)\n    at file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/vitest@2.0.4_@types+node@20.14.12_jsdom@24.1.1_bufferutil@4.0.8_utf-8-validate@5.0.10_/node_modules/vitest/dist/chunks/runtime-runBaseTests.Dq_sJZq9.js:132:11\n    at withEnv (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/vitest@2.0.4_@types+node@20.14.12_jsdom@24.1.1_bufferutil@4.0.8_utf-8-validate@5.0.10_/node_modules/vitest/dist/chunks/runtime-runBaseTests.Dq_sJZq9.js:94:5)\n    at run (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/vitest@2.0.4_@types+node@20.14.12_jsdom@24.1.1_bufferutil@4.0.8_utf-8-validate@5.0.10_/node_modules/vitest/dist/chunks/runtime-runBaseTests.Dq_sJZq9.js:117:3)\n    at runBaseTests (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/vitest@2.0.4_@types+node@20.14.12_jsdom@24.1.1_bufferutil@4.0.8_utf-8-validate@5.0.10_/node_modules/vitest/dist/vendor/base.Csk7BT3h.js:31:3)\n    at ForksBaseWorker.executeTests (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/vitest@2.0.4_@types+node@20.14.12_jsdom@24.1.1_bufferutil@4.0.8_utf-8-validate@5.0.10_/node_modules/vitest/dist/workers/forks.js:25:7)\n    at execute (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/vitest@2.0.4_@types+node@20.14.12_jsdom@24.1.1_bufferutil@4.0.8_utf-8-validate@5.0.10_/node_modules/vitest/dist/worker.js:116:5)\n    at onMessage (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/tinypool@1.0.0/node_modules/tinypool/dist/entry/process.js:54:20)"}' />

## CCC 創作集 <Site url="creative-comic.tw"/>

### 漫畫 <Site url="creative-comic.tw" size="sm" />

<Route namespace="creative-comic" :data='{"path":"/book/:id/:coverOnly?/:quality?","categories":["anime"],"example":"/creative-comic/book/117","parameters":{"id":"漫畫 ID，可在 URL 中找到","coverOnly":"僅獲取封面，非 `true` 時將獲取**全部**頁面，預設 `true`","quality":"閱讀品質，標準畫質 `1`，高畫質 `2`，預設 `1`"},"features":{"requireConfig":false,"requirePuppeteer":false,"antiCrawler":false,"supportBT":false,"supportPodcast":false,"supportScihub":false},"radar":[{"source":["creative-comic.tw/book/:id/*"],"target":"/:id"}],"name":"漫畫","maintainers":["TonyRL"],"location":"book.ts"}' :test='undefined' />

## DLsite <Site url="dlsite.com"/>

### Current Release <Site url="dlsite.com" size="sm" />

<Route namespace="dlsite" :data='{"path":"/new/:type","categories":["anime"],"example":"/dlsite/new/home","parameters":{"type":"Type, see table below"},"features":{"requireConfig":false,"requirePuppeteer":false,"antiCrawler":false,"supportBT":false,"supportPodcast":false,"supportScihub":false},"name":"Current Release","maintainers":["cssxsh"],"description":"| Doujin | Comics | PC Games | Doujin (R18) | Adult Comics | H Games | Otome | BL |\n  | ------ | ------ | -------- | ------------ | ------------ | ------- | ----- | -- |\n  | home   | comic  | soft     | maniax       | books        | pro     | girls | bl |","location":"new.ts"}' :test='{"code":1,"message":"AssertionError: expected 503 to be 200 // Object.is equality\n    at /home/runner/work/RSSHub/RSSHub/lib/routes.test.ts:79:41\n    at processTicksAndRejections (node:internal/process/task_queues:95:5)\n    at runTest (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/@vitest+runner@2.0.4/node_modules/@vitest/runner/dist/index.js:955:11)\n    at async Promise.all (index 394)\n    at runSuite (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/@vitest+runner@2.0.4/node_modules/@vitest/runner/dist/index.js:1097:13)\n    at runSuite (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/@vitest+runner@2.0.4/node_modules/@vitest/runner/dist/index.js:1111:15)\n    at runFiles (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/@vitest+runner@2.0.4/node_modules/@vitest/runner/dist/index.js:1168:5)\n    at startTests (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/@vitest+runner@2.0.4/node_modules/@vitest/runner/dist/index.js:1177:3)\n    at file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/vitest@2.0.4_@types+node@20.14.12_jsdom@24.1.1_bufferutil@4.0.8_utf-8-validate@5.0.10_/node_modules/vitest/dist/chunks/runtime-runBaseTests.Dq_sJZq9.js:132:11\n    at withEnv (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/vitest@2.0.4_@types+node@20.14.12_jsdom@24.1.1_bufferutil@4.0.8_utf-8-validate@5.0.10_/node_modules/vitest/dist/chunks/runtime-runBaseTests.Dq_sJZq9.js:94:5)\n    at run (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/vitest@2.0.4_@types+node@20.14.12_jsdom@24.1.1_bufferutil@4.0.8_utf-8-validate@5.0.10_/node_modules/vitest/dist/chunks/runtime-runBaseTests.Dq_sJZq9.js:117:3)\n    at runBaseTests (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/vitest@2.0.4_@types+node@20.14.12_jsdom@24.1.1_bufferutil@4.0.8_utf-8-validate@5.0.10_/node_modules/vitest/dist/vendor/base.Csk7BT3h.js:31:3)\n    at ForksBaseWorker.executeTests (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/vitest@2.0.4_@types+node@20.14.12_jsdom@24.1.1_bufferutil@4.0.8_utf-8-validate@5.0.10_/node_modules/vitest/dist/workers/forks.js:25:7)\n    at execute (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/vitest@2.0.4_@types+node@20.14.12_jsdom@24.1.1_bufferutil@4.0.8_utf-8-validate@5.0.10_/node_modules/vitest/dist/worker.js:116:5)\n    at onMessage (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/tinypool@1.0.0/node_modules/tinypool/dist/entry/process.js:54:20)"}' />

| Doujin | Comics | PC Games | Doujin (R18) | Adult Comics | H Games | Otome | BL |
  | ------ | ------ | -------- | ------------ | ------------ | ------- | ----- | -- |
  | home   | comic  | soft     | maniax       | books        | pro     | girls | bl |

### Ci-en Creators' Article <Site url="dlsite.com" size="sm" />

<Route namespace="dlsite" :data='{"path":"/ci-en/:id/article","categories":["anime"],"example":"/dlsite/ci-en/7400/article","parameters":{"id":"Creator id, can be found in URL"},"features":{"requireConfig":false,"requirePuppeteer":false,"antiCrawler":false,"supportBT":false,"supportPodcast":false,"supportScihub":false},"radar":[{"source":["ci-en.dlsite.com/creator/:id/article/843558","ci-en.dlsite.com/"]}],"name":"Ci-en Creators&#39; Article","maintainers":["nczitzk"],"location":"ci-en/article.ts"}' :test='{"code":1,"message":"AssertionError: expected 503 to be 200 // Object.is equality\n    at /home/runner/work/RSSHub/RSSHub/lib/routes.test.ts:79:41\n    at processTicksAndRejections (node:internal/process/task_queues:95:5)\n    at runTest (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/@vitest+runner@2.0.4/node_modules/@vitest/runner/dist/index.js:955:11)\n    at async Promise.all (index 395)\n    at runSuite (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/@vitest+runner@2.0.4/node_modules/@vitest/runner/dist/index.js:1097:13)\n    at runSuite (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/@vitest+runner@2.0.4/node_modules/@vitest/runner/dist/index.js:1111:15)\n    at runFiles (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/@vitest+runner@2.0.4/node_modules/@vitest/runner/dist/index.js:1168:5)\n    at startTests (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/@vitest+runner@2.0.4/node_modules/@vitest/runner/dist/index.js:1177:3)\n    at file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/vitest@2.0.4_@types+node@20.14.12_jsdom@24.1.1_bufferutil@4.0.8_utf-8-validate@5.0.10_/node_modules/vitest/dist/chunks/runtime-runBaseTests.Dq_sJZq9.js:132:11\n    at withEnv (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/vitest@2.0.4_@types+node@20.14.12_jsdom@24.1.1_bufferutil@4.0.8_utf-8-validate@5.0.10_/node_modules/vitest/dist/chunks/runtime-runBaseTests.Dq_sJZq9.js:94:5)\n    at run (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/vitest@2.0.4_@types+node@20.14.12_jsdom@24.1.1_bufferutil@4.0.8_utf-8-validate@5.0.10_/node_modules/vitest/dist/chunks/runtime-runBaseTests.Dq_sJZq9.js:117:3)\n    at runBaseTests (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/vitest@2.0.4_@types+node@20.14.12_jsdom@24.1.1_bufferutil@4.0.8_utf-8-validate@5.0.10_/node_modules/vitest/dist/vendor/base.Csk7BT3h.js:31:3)\n    at ForksBaseWorker.executeTests (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/vitest@2.0.4_@types+node@20.14.12_jsdom@24.1.1_bufferutil@4.0.8_utf-8-validate@5.0.10_/node_modules/vitest/dist/workers/forks.js:25:7)\n    at execute (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/vitest@2.0.4_@types+node@20.14.12_jsdom@24.1.1_bufferutil@4.0.8_utf-8-validate@5.0.10_/node_modules/vitest/dist/worker.js:116:5)\n    at onMessage (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/tinypool@1.0.0/node_modules/tinypool/dist/entry/process.js:54:20)"}' />

### Discounted Works <Site url="dlsite.com" size="sm" />

<Route namespace="dlsite" :data='{"path":"/campaign/:type/:free?","categories":["anime"],"example":"/dlsite/campaign/home","parameters":{"type":"Type, see table above","free":"Free only, empty means false, other value means true"},"features":{"requireConfig":false,"requirePuppeteer":false,"antiCrawler":false,"supportBT":false,"supportPodcast":false,"supportScihub":false},"name":"Discounted Works","maintainers":["cssxsh"],"location":"campaign.ts"}' :test='{"code":1,"message":"AssertionError: expected 503 to be 200 // Object.is equality\n    at /home/runner/work/RSSHub/RSSHub/lib/routes.test.ts:79:41\n    at runTest (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/@vitest+runner@2.0.4/node_modules/@vitest/runner/dist/index.js:955:11)\n    at async Promise.all (index 393)\n    at runSuite (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/@vitest+runner@2.0.4/node_modules/@vitest/runner/dist/index.js:1097:13)\n    at runSuite (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/@vitest+runner@2.0.4/node_modules/@vitest/runner/dist/index.js:1111:15)\n    at runFiles (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/@vitest+runner@2.0.4/node_modules/@vitest/runner/dist/index.js:1168:5)\n    at startTests (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/@vitest+runner@2.0.4/node_modules/@vitest/runner/dist/index.js:1177:3)\n    at file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/vitest@2.0.4_@types+node@20.14.12_jsdom@24.1.1_bufferutil@4.0.8_utf-8-validate@5.0.10_/node_modules/vitest/dist/chunks/runtime-runBaseTests.Dq_sJZq9.js:132:11\n    at withEnv (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/vitest@2.0.4_@types+node@20.14.12_jsdom@24.1.1_bufferutil@4.0.8_utf-8-validate@5.0.10_/node_modules/vitest/dist/chunks/runtime-runBaseTests.Dq_sJZq9.js:94:5)\n    at run (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/vitest@2.0.4_@types+node@20.14.12_jsdom@24.1.1_bufferutil@4.0.8_utf-8-validate@5.0.10_/node_modules/vitest/dist/chunks/runtime-runBaseTests.Dq_sJZq9.js:117:3)\n    at runBaseTests (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/vitest@2.0.4_@types+node@20.14.12_jsdom@24.1.1_bufferutil@4.0.8_utf-8-validate@5.0.10_/node_modules/vitest/dist/vendor/base.Csk7BT3h.js:31:3)\n    at ForksBaseWorker.executeTests (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/vitest@2.0.4_@types+node@20.14.12_jsdom@24.1.1_bufferutil@4.0.8_utf-8-validate@5.0.10_/node_modules/vitest/dist/workers/forks.js:25:7)\n    at execute (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/vitest@2.0.4_@types+node@20.14.12_jsdom@24.1.1_bufferutil@4.0.8_utf-8-validate@5.0.10_/node_modules/vitest/dist/worker.js:116:5)\n    at onMessage (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/tinypool@1.0.0/node_modules/tinypool/dist/entry/process.js:54:20)"}' />

### Unknown <Site url="dlsite.com" size="sm" />

<Route namespace="dlsite" :data='{"path":"*","name":"Unknown","maintainers":[],"location":"index.ts"}' :test='undefined' />

## Doraemon Channel <Site url="www.dora-world.com"/>

### Article <Site url="www.dora-world.com" size="sm" />

<Route namespace="dora-world" :data='{"path":"/article/:topic/:topicId?","categories":["anime"],"example":"/dora-world/article/contents","parameters":{"topic":"Topic name, can be found in URL. For example: the topic name of [https://www.dora-world.com/movie](https://www.dora-world.com/movie) is `movie`","topicId":"Topic id, can be found in URL. For example: the topic id of [https://www.dora-world.com/contents?t=197](https://www.dora-world.com/contents?t=197) is `197`"},"features":{"requireConfig":false,"requirePuppeteer":false,"antiCrawler":false,"supportBT":false,"supportPodcast":false,"supportScihub":false},"radar":[{"source":["www.dora-world.com/:topic"]}],"name":"Article","maintainers":["AChangAZha"],"location":"article.ts"}' :test='undefined' />

## Eventernote <Site url="www.eventernote.com"/>

### 声优活动及演唱会 <Site url="www.eventernote.com" size="sm" />

<Route namespace="eventernote" :data='{"path":"/actors/:name/:id","categories":["anime"],"example":"/eventernote/actors/三森すずこ/2634","parameters":{"name":"声优姓名","id":"声优 ID"},"features":{"requireConfig":false,"requirePuppeteer":false,"antiCrawler":false,"supportBT":false,"supportPodcast":false,"supportScihub":false},"radar":[{"source":["www.eventernote.com/actors/:name/:id/events"]}],"name":"声优活动及演唱会","maintainers":["KTachibanaM"],"location":"actors.ts"}' :test='{"code":0}' />

## Gogoanimehd <Site url="developer.anitaku.to"/>

### Recent Releases <Site url="developer.anitaku.to/" size="sm" />

<Route namespace="gogoanimehd" :data='{"path":"/recent-releases","categories":["anime"],"example":"/gogoanimehd/recent-releases","parameters":{},"features":{"requireConfig":false,"requirePuppeteer":false,"antiCrawler":false,"supportBT":false,"supportPodcast":false,"supportScihub":false},"radar":[{"source":["developer.anitaku.to/"]}],"name":"Recent Releases","maintainers":["user4302"],"url":"developer.anitaku.to/","location":"recent-releases.ts"}' :test='{"code":0}' />

## Hpoi 手办维基 <Site url="www.hpoi.net"/>

### 角色周边 <Site url="www.hpoi.net" size="sm" />

<Route namespace="hpoi" :data='{"path":"/items/character/:id/:order?","categories":["anime"],"example":"/hpoi/items/character/1035374","parameters":{"id":"角色 ID","order":"排序, 见下表，默认为 add"},"features":{"requireConfig":false,"requirePuppeteer":false,"antiCrawler":false,"supportBT":false,"supportPodcast":false,"supportScihub":false},"name":"角色周边","maintainers":["DIYgod"],"description":"| 发售    | 入库 | 总热度 | 一周热度 | 一天热度 | 评价   |\n  | ------- | ---- | ------ | -------- | -------- | ------ |\n  | release | add  | hits   | hits7Day | hitsDay  | rating |","location":"character.ts"}' :test='{"code":0}' />

| 发售    | 入库 | 总热度 | 一周热度 | 一天热度 | 评价   |
  | ------- | ---- | ------ | -------- | -------- | ------ |
  | release | add  | hits   | hits7Day | hitsDay  | rating |

### 情报 <Site url="www.hpoi.net" size="sm" />

<Route namespace="hpoi" :data='{"path":"/info/:type?","categories":["anime"],"example":"/hpoi/info/all","parameters":{"type":"分类, 见下表, 默认为`all`"},"features":{"requireConfig":false,"requirePuppeteer":false,"antiCrawler":false,"supportBT":false,"supportPodcast":false,"supportScihub":false},"name":"情报","maintainers":["sanmmm DIYgod"],"description":"分类\n\n  | 全部 | 手办  | 模型  |\n  | ---- | ----- | ----- |\n  | all  | hobby | model |","location":"info.ts"}' :test='{"code":1,"message":"AssertionError: expected [ &#39;https://www.hpoi.net/hobby/99835&#39; ] to not include &#39;https://www.hpoi.net/hobby/99835&#39;\n    at Proxy.<anonymous> (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/@vitest+expect@2.0.4/node_modules/@vitest/expect/dist/index.js:1135:17)\n    at Proxy.<anonymous> (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/@vitest+expect@2.0.4/node_modules/@vitest/expect/dist/index.js:912:17)\n    at Proxy.methodWrapper (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/chai@5.1.1/node_modules/chai/chai.js:1591:25)\n    at checkRSS (/home/runner/work/RSSHub/RSSHub/lib/routes.test.ts:65:27)\n    at processTicksAndRejections (node:internal/process/task_queues:95:5)\n    at /home/runner/work/RSSHub/RSSHub/lib/routes.test.ts:80:17\n    at runTest (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/@vitest+runner@2.0.4/node_modules/@vitest/runner/dist/index.js:955:11)\n    at async Promise.all (index 757)\n    at runSuite (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/@vitest+runner@2.0.4/node_modules/@vitest/runner/dist/index.js:1097:13)\n    at runSuite (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/@vitest+runner@2.0.4/node_modules/@vitest/runner/dist/index.js:1111:15)\n    at runFiles (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/@vitest+runner@2.0.4/node_modules/@vitest/runner/dist/index.js:1168:5)\n    at startTests (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/@vitest+runner@2.0.4/node_modules/@vitest/runner/dist/index.js:1177:3)\n    at file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/vitest@2.0.4_@types+node@20.14.12_jsdom@24.1.1_bufferutil@4.0.8_utf-8-validate@5.0.10_/node_modules/vitest/dist/chunks/runtime-runBaseTests.Dq_sJZq9.js:132:11\n    at withEnv (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/vitest@2.0.4_@types+node@20.14.12_jsdom@24.1.1_bufferutil@4.0.8_utf-8-validate@5.0.10_/node_modules/vitest/dist/chunks/runtime-runBaseTests.Dq_sJZq9.js:94:5)\n    at run (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/vitest@2.0.4_@types+node@20.14.12_jsdom@24.1.1_bufferutil@4.0.8_utf-8-validate@5.0.10_/node_modules/vitest/dist/chunks/runtime-runBaseTests.Dq_sJZq9.js:117:3)\n    at runBaseTests (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/vitest@2.0.4_@types+node@20.14.12_jsdom@24.1.1_bufferutil@4.0.8_utf-8-validate@5.0.10_/node_modules/vitest/dist/vendor/base.Csk7BT3h.js:31:3)"}' />

分类

  | 全部 | 手办  | 模型  |
  | ---- | ----- | ----- |
  | all  | hobby | model |

### 热门推荐 <Site url="www.hpoi.net/bannerItem/list" size="sm" />

<Route namespace="hpoi" :data='{"path":"/bannerItem","categories":["anime"],"example":"/hpoi/bannerItem","parameters":{},"features":{"requireConfig":false,"requirePuppeteer":false,"antiCrawler":false,"supportBT":false,"supportPodcast":false,"supportScihub":false},"radar":[{"source":["www.hpoi.net/bannerItem/list"]}],"name":"热门推荐","maintainers":["DIYgod"],"url":"www.hpoi.net/bannerItem/list","location":"banner-item.ts"}' :test='{"code":0}' />

### 所有周边 <Site url="www.hpoi.net/hobby/all" size="sm" />

<Route namespace="hpoi" :data='{"path":"/items/all/:order?","categories":["anime"],"example":"/hpoi/items/all","parameters":{"order":"排序, 见下表，默认为 add"},"features":{"requireConfig":false,"requirePuppeteer":false,"antiCrawler":false,"supportBT":false,"supportPodcast":false,"supportScihub":false},"radar":[{"source":["www.hpoi.net/hobby/all"],"target":"/items/all"}],"name":"所有周边","maintainers":["DIYgod"],"url":"www.hpoi.net/hobby/all","description":"| 发售    | 入库 | 总热度 | 一周热度 | 一天热度 | 评价   |\n  | ------- | ---- | ------ | -------- | -------- | ------ |\n  | release | add  | hits   | hits7Day | hitsDay  | rating |","location":"all.ts"}' :test='{"code":0}' />

| 发售    | 入库 | 总热度 | 一周热度 | 一天热度 | 评价   |
  | ------- | ---- | ------ | -------- | -------- | ------ |
  | release | add  | hits   | hits7Day | hitsDay  | rating |

### 用户动态 <Site url="www.hpoi.net" size="sm" />

<Route namespace="hpoi" :data='{"path":"/user/:user_id/:caty","categories":["anime"],"example":"/hpoi/user/116297/buy","parameters":{"user_id":"用户ID","caty":"类别, 见下表"},"features":{"requireConfig":false,"requirePuppeteer":false,"antiCrawler":false,"supportBT":false,"supportPodcast":false,"supportScihub":false},"name":"用户动态","maintainers":["DIYgod","luyuhuang"],"description":"| 想买 | 预定     | 已入 | 关注 | 有过   |\n  | ---- | -------- | ---- | ---- | ------ |\n  | want | preorder | buy  | care | resell |","location":"user.ts"}' :test='{"code":0}' />

| 想买 | 预定     | 已入 | 关注 | 有过   |
  | ---- | -------- | ---- | ---- | ------ |
  | want | preorder | buy  | care | resell |

### 作品周边 <Site url="www.hpoi.net" size="sm" />

<Route namespace="hpoi" :data='{"path":"/items/work/:id/:order?","categories":["anime"],"example":"/hpoi/items/work/4117491","parameters":{"id":"作品 ID","order":"排序, 见下表，默认为 add"},"features":{"requireConfig":false,"requirePuppeteer":false,"antiCrawler":false,"supportBT":false,"supportPodcast":false,"supportScihub":false},"name":"作品周边","maintainers":["DIYgod"],"description":"| 发售    | 入库 | 总热度 | 一周热度 | 一天热度 | 评价   |\n  | ------- | ---- | ------ | -------- | -------- | ------ |\n  | release | add  | hits   | hits7Day | hitsDay  | rating |","location":"work.ts"}' :test='{"code":0}' />

| 发售    | 入库 | 总热度 | 一周热度 | 一天热度 | 评价   |
  | ------- | ---- | ------ | -------- | -------- | ------ |
  | release | add  | hits   | hits7Day | hitsDay  | rating |

## IDOLY PRIDE 偶像荣耀 <Site url="idolypride.jp"/>

### News <Site url="idolypride.jp/news" size="sm" />

<Route namespace="idolypride" :data='{"path":"/news","categories":["anime"],"example":"/idolypride/news","parameters":{},"features":{"requireConfig":false,"requirePuppeteer":false,"antiCrawler":false,"supportBT":false,"supportPodcast":false,"supportScihub":false},"radar":[{"source":["idolypride.jp/news"]}],"name":"News","maintainers":["Mingxia1"],"url":"idolypride.jp/news","location":"news.ts"}' :test='{"code":0}' />

## iwara <Site url="ecchi.iwara.tv"/>

### Unknown <Site url="ecchi.iwara.tv" size="sm" />

<Route namespace="iwara" :data='{"path":"/users/:username?/:type?","name":"Unknown","maintainers":["Fatpandac"],"location":"index.ts"}' :test='undefined' />

### User Subscriptions <Site url="ecchi.iwara.tv/" size="sm" />

<Route namespace="iwara" :data='{"path":"/subscriptions","categories":["anime"],"example":"/iwara/subscriptions","parameters":{},"features":{"requireConfig":[{"name":"IWARA_USERNAME","description":""},{"name":"IWARA_PASSWORD","description":""}],"requirePuppeteer":false,"antiCrawler":false,"supportBT":false,"supportPodcast":false,"supportScihub":false},"radar":[{"source":["ecchi.iwara.tv/"]}],"name":"User Subscriptions","maintainers":["FeCCC"],"url":"ecchi.iwara.tv/","description":":::warning\n  This route requires username and password, therefore it&#39;s only available when self-hosting, refer to the [Deploy Guide](https://docs.rsshub.app/deploy/config#route-specific-configurations) for route-specific configurations.\n  :::","location":"subscriptions.ts"}' :test='undefined' />

:::warning
  This route requires username and password, therefore it's only available when self-hosting, refer to the [Deploy Guide](https://docs.rsshub.app/deploy/config#route-specific-configurations) for route-specific configurations.
  :::

## Kemono <Site url="kemono.su"/>

### Posts <Site url="kemono.su" size="sm" />

<Route namespace="kemono" :data='{"path":"/:source?/:id?","categories":["anime"],"example":"/kemono","parameters":{"source":"Source, see below, Posts by default","id":"User id, can be found in URL"},"features":{"requireConfig":false,"requirePuppeteer":false,"antiCrawler":false,"supportBT":false,"supportPodcast":false,"supportScihub":false},"radar":[{"source":["kemono.su/:source/user/:id","kemono.su/"]}],"name":"Posts","maintainers":["nczitzk"],"description":"Sources\n\n  | Posts | Patreon | Pixiv Fanbox | Gumroad | SubscribeStar | DLsite | Discord | Fantia |\n  | ----- | ------- | ------------ | ------- | ------------- | ------ | ------- | ------ |\n  | posts | patreon | fanbox       | gumroad | subscribestar | dlsite | discord | fantia |\n\n  :::tip\n  When `posts` is selected as the value of the parameter **source**, the parameter **id** does not take effect.\n  There is an optinal parameter **limit** which controls the number of posts to fetch, default value is 25.\n  :::","location":"index.ts"}' :test='{"code":0}' />

Sources

  | Posts | Patreon | Pixiv Fanbox | Gumroad | SubscribeStar | DLsite | Discord | Fantia |
  | ----- | ------- | ------------ | ------- | ------------- | ------ | ------- | ------ |
  | posts | patreon | fanbox       | gumroad | subscribestar | dlsite | discord | fantia |

  :::tip
  When `posts` is selected as the value of the parameter **source**, the parameter **id** does not take effect.
  There is an optinal parameter **limit** which controls the number of posts to fetch, default value is 25.
  :::

## lovelive-anime <Site url="www.lovelive-anime.jp"/>

### Love Live! Official Website Latest NEWS <Site url="www.lovelive-anime.jp/" size="sm" />

<Route namespace="lovelive-anime" :data='{"path":"/news/:option?","categories":["anime"],"example":"/lovelive-anime/news","parameters":{"option":"Crawl full text when `option` is `detail`."},"features":{"requireConfig":false,"requirePuppeteer":false,"antiCrawler":false,"supportBT":false,"supportPodcast":false,"supportScihub":false},"radar":[{"source":["www.lovelive-anime.jp/","www.lovelive-anime.jp/news"],"target":"/news"}],"name":"Love Live! Official Website Latest NEWS","maintainers":["axojhf"],"url":"www.lovelive-anime.jp/","location":"news.ts"}' :test='undefined' />

### Love Live Official Website Categories Topics <Site url="www.lovelive-anime.jp" size="sm" />

<Route namespace="lovelive-anime" :data='{"path":"/topics/:abbr/:category?/:option?","categories":["anime"],"example":"/lovelive-anime/topics/otonokizaka","parameters":{"abbr":"The path to the Love Live series of sub-projects on the official website is detailed in the table below","category":"The official website lists the Topics category, `category` is `detail` when crawling the full text, other categories see the following table for details","option":"Crawl full text when `option` is `detail`."},"features":{"requireConfig":false,"requirePuppeteer":false,"antiCrawler":false,"supportBT":false,"supportPodcast":false,"supportScihub":false},"name":"Love Live Official Website Categories Topics","maintainers":["axojhf"],"description":"| Sub-project Name (not full name) | Lovelive!   | Lovelive! Sunshine!! | Lovelive! Nijigasaki High School Idol Club | Lovelive! Superstar!! | 幻日のヨハネ | ラブライブ！スクールアイドルミュージカル |\n  | -------------------------------- | ----------- | -------------------- | ------------------------------------------ | --------------------- | ------------ | ---------------------------------------- |\n  | `abbr`parameter                  | otonokizaka | uranohoshi           | nijigasaki                                 | yuigaoka              | yohane       | musical                                  |\n\n  | Category Name       | 全てのニュース        | 音楽商品 | アニメ映像商品 | キャスト映像商品 | 劇場    | アニメ放送 / 配信 | キャスト配信 / ラジオ | ライブ / イベント | ブック | グッズ | ゲーム | メディア | ご当地情報 | その他 | キャンペーン |\n  | ------------------- | --------------------- | -------- | -------------- | ---------------- | ------- | ----------------- | --------------------- | ----------------- | ------ | ------ | ------ | -------- | ---------- | ------ | ------------ |\n  | `category`parameter | <u>*No parameter*</u> | music    | anime_movie   | cast_movie      | theater | onair             | radio                 | event             | books  | goods  | game   | media    | local      | other  | campaign     |","location":"topics.ts"}' :test='undefined' />

| Sub-project Name (not full name) | Lovelive!   | Lovelive! Sunshine!! | Lovelive! Nijigasaki High School Idol Club | Lovelive! Superstar!! | 幻日のヨハネ | ラブライブ！スクールアイドルミュージカル |
  | -------------------------------- | ----------- | -------------------- | ------------------------------------------ | --------------------- | ------------ | ---------------------------------------- |
  | `abbr`parameter                  | otonokizaka | uranohoshi           | nijigasaki                                 | yuigaoka              | yohane       | musical                                  |

  | Category Name       | 全てのニュース        | 音楽商品 | アニメ映像商品 | キャスト映像商品 | 劇場    | アニメ放送 / 配信 | キャスト配信 / ラジオ | ライブ / イベント | ブック | グッズ | ゲーム | メディア | ご当地情報 | その他 | キャンペーン |
  | ------------------- | --------------------- | -------- | -------------- | ---------------- | ------- | ----------------- | --------------------- | ----------------- | ------ | ------ | ------ | -------- | ---------- | ------ | ------------ |
  | `category`parameter | <u>*No parameter*</u> | music    | anime_movie   | cast_movie      | theater | onair             | radio                 | event             | books  | goods  | game   | media    | local      | other  | campaign     |

### Unknown <Site url="www.lovelive-anime.jp" size="sm" />

<Route namespace="lovelive-anime" :data='{"path":"/schedules/:serie?/:category?","name":"Unknown","maintainers":[],"location":"schedules.ts"}' :test='undefined' />

## Mox.moe <Site url="mox.moe"/>

### 首頁 <Site url="mox.moe" size="sm" />

<Route namespace="mox" :data='{"path":"/:category?","categories":["anime"],"example":"/mox","parameters":{"category":"分类，可在对应分类页 URL 中找到"},"features":{"requireConfig":[{"name":"MOX_COOKIE","optional":true,"description":"注册用户登录后的 Cookie, 可以从浏览器开发者工具Network面板中的mox页面请求获取，Cookie内容形如VOLSKEY=xxxxxx; VLIBSID=xxxxxx; VOLSESS=xxxxxx"}],"antiCrawler":true},"radar":[{"source":["mox.moe/l/:category","mox.moe/"]}],"name":"首頁","maintainers":["nczitzk"],"description":":::tip\n  在首页将分类参数选择确定后跳转到的分类页面 URL 中，`/l/` 后的字段即为分类参数。\n\n  如 [科幻 + 日語 + 日本 + 長篇 + 完結 + 最近更新](https://mox.moe/l/CAT%2A科幻,日本,完結,lastupdate,jpn,l,BL) 的 URL 为 [https://mox.moe/l/CAT%2A 科幻，日本，完結，lastupdate,jpn,l,BL](https://mox.moe/l/CAT%2A科幻,日本,完結,lastupdate,jpn,l,BL)，此时 `/l/` 后的字段为 `CAT%2A科幻,日本,完結,lastupdate,jpn,l,BL`。最终获得路由为 [`/mox/CAT%2A科幻,日本,完結,lastupdate,jpn,l,BL`](https://rsshub.app/mox/CAT%2A科幻,日本,完結,lastupdate,jpn,l,BL)\n  :::\n\n  :::warning\n  由于 mox.moe 对非登录用户屏蔽了部分漫画详情内容的获取，且极易触发反爬机制，导致访问ip被重定向至google.com，因此在未配置`MOX_COOKIE`参数的情况下路由只会返回漫画标题和封面，不会对详情内容进行抓取。\n  :::","location":"index.ts"}' :test='{"code":0}' />

:::tip
  在首页将分类参数选择确定后跳转到的分类页面 URL 中，`/l/` 后的字段即为分类参数。

  如 [科幻 + 日語 + 日本 + 長篇 + 完結 + 最近更新](https://mox.moe/l/CAT%2A科幻,日本,完結,lastupdate,jpn,l,BL) 的 URL 为 [https://mox.moe/l/CAT%2A 科幻，日本，完結，lastupdate,jpn,l,BL](https://mox.moe/l/CAT%2A科幻,日本,完結,lastupdate,jpn,l,BL)，此时 `/l/` 后的字段为 `CAT%2A科幻,日本,完結,lastupdate,jpn,l,BL`。最终获得路由为 [`/mox/CAT%2A科幻,日本,完結,lastupdate,jpn,l,BL`](https://rsshub.app/mox/CAT%2A科幻,日本,完結,lastupdate,jpn,l,BL)
  :::

  :::warning
  由于 mox.moe 对非登录用户屏蔽了部分漫画详情内容的获取，且极易触发反爬机制，导致访问ip被重定向至google.com，因此在未配置`MOX_COOKIE`参数的情况下路由只会返回漫画标题和封面，不会对详情内容进行抓取。
  :::

## nhentai <Site url="nhentai.net"/>

### Advanced Search <Site url="nhentai.net" size="sm" />

<Route namespace="nhentai" :data='{"path":"/search/:keyword/:mode?","example":"/nhentai/search/language%3Ajapanese+-scat+-yaoi+-guro+-\"mosaic+censorship\"","parameters":{"keyword":"Keywords for search. You can copy the content after `q=` after searching on the original website, or you can enter it directly. See the [official website](https://nhentai.net/info/) for details","mode":"mode, `simple` to only show cover, `detail` to show all pages, `torrent` to include Magnet URI, need login, refer to [Route-specific Configurations](https://docs.rsshub.app/deploy/config#route-specific-configurations), default to `simple`"},"features":{"antiCrawler":true,"supportBT":true},"radar":[{"source":["nhentai.net/:key/:keyword"],"target":"/:key/:keyword"}],"name":"Advanced Search","maintainers":["MegrezZhu","hoilc"],"location":"search.ts"}' :test='{"code":0}' />

### Filter <Site url="nhentai.net" size="sm" />

<Route namespace="nhentai" :data='{"path":"/index/:key/:keyword/:mode?","example":"/nhentai/index/language/chinese","parameters":{"key":"Filter term, can be: `parody`, `character`, `tag`, `artist`, `group`, `language` or `category`","keyword":"Filter value","mode":"mode, `simple` to only show cover, `detail` to show all pages, `torrent` to include Magnet URI, need login, refer to [Route-specific Configurations](https://docs.rsshub.app/deploy/config#route-specific-configurations), default to `simple`"},"features":{"antiCrawler":true,"supportBT":true},"radar":[{"source":["nhentai.net/:key/:keyword"],"target":"/index/:key/:keyword"}],"name":"Filter","maintainers":["MegrezZhu","hoilc"],"location":"index.ts"}' :test='{"code":0}' />

## NT动漫 <Site url="www.ntdm9.com"/>

### 番剧详情 <Site url="www.ntdm9.com" size="sm" />

<Route namespace="ntdm" :data='{"path":"/video/:id","categories":["anime"],"example":"/ntdm/video/4309","parameters":{"id":"番剧 id，对应详情 URL 中找到"},"features":{"requireConfig":false,"requirePuppeteer":false,"antiCrawler":false,"supportBT":false,"supportPodcast":false,"supportScihub":false},"radar":[{"source":["ntdm9.com/video/:id"]}],"name":"番剧详情","maintainers":["Yamico"],"location":"video.ts"}' :test='{"code":0}' />

## QooApp <Site url="apps.qoo-app.com"/>

### Game Store - Cards <Site url="apps.qoo-app.com" size="sm" />

<Route namespace="qoo-app" :data='{"path":"/apps/:lang?/card/:id","categories":["anime"],"example":"/qoo-app/apps/en/card/7675","parameters":{"lang":"Language, see the table above, empty means `中文`","id":"Game ID, can be found in URL"},"features":{"requireConfig":false,"requirePuppeteer":false,"antiCrawler":false,"supportBT":false,"supportPodcast":false,"supportScihub":false},"name":"Game Store - Cards","maintainers":["TonyRL"],"location":"apps/card.ts"}' :test='undefined' />

### Game Store - Review <Site url="apps.qoo-app.com" size="sm" />

<Route namespace="qoo-app" :data='{"path":"/apps/:lang?/comment/:id","categories":["anime"],"example":"/qoo-app/apps/en/comment/7675","parameters":{"lang":"Language, see the table below, empty means `中文`","id":"Game ID, can be found in URL"},"features":{"requireConfig":false,"requirePuppeteer":false,"antiCrawler":false,"supportBT":false,"supportPodcast":false,"supportScihub":false},"name":"Game Store - Review","maintainers":["TonyRL"],"description":"| 中文 | English | 한국어 | Español | 日本語 | ไทย | Tiếng Việt |\n  | ---- | ------- | ------ | ------- | ------ | --- | ---------- |\n  |      | en      | ko     | es      | ja     | th  | vi         |","location":"apps/comment.ts"}' :test='undefined' />

| 中文 | English | 한국어 | Español | 日本語 | ไทย | Tiếng Việt |
  | ---- | ------- | ------ | ------- | ------ | --- | ---------- |
  |      | en      | ko     | es      | ja     | th  | vi         |

### Game Store - Notes <Site url="apps.qoo-app.com" size="sm" />

<Route namespace="qoo-app" :data='{"path":"/apps/:lang?/note/:id","categories":["anime"],"example":"/qoo-app/apps/en/note/7675","parameters":{"lang":"Language, see the table above, empty means `中文`","id":"Game ID, can be found in URL"},"features":{"requireConfig":false,"requirePuppeteer":false,"antiCrawler":false,"supportBT":false,"supportPodcast":false,"supportScihub":false},"name":"Game Store - Notes","maintainers":["TonyRL"],"location":"apps/note.ts"}' :test='undefined' />

### Game Store - Article <Site url="apps.qoo-app.com" size="sm" />

<Route namespace="qoo-app" :data='{"path":"/apps/:lang?/post/:id","categories":["anime"],"example":"/qoo-app/apps/en/post/7675","parameters":{"lang":"Language, see the table above, empty means `中文`","id":"Game ID, can be found in URL"},"features":{"requireConfig":false,"requirePuppeteer":false,"antiCrawler":false,"supportBT":false,"supportPodcast":false,"supportScihub":false},"name":"Game Store - Article","maintainers":["TonyRL"],"location":"apps/post.ts"}' :test='undefined' />

### News <Site url="apps.qoo-app.com" size="sm" />

<Route namespace="qoo-app" :data='{"path":"/news/:lang?","categories":["anime"],"example":"/qoo-app/news/en","parameters":{"lang":"Language, see the table below, empty means `中文`"},"features":{"requireConfig":false,"requirePuppeteer":false,"antiCrawler":false,"supportBT":false,"supportPodcast":false,"supportScihub":false},"name":"News","maintainers":["TonyRL"],"description":"| 中文 | English |\n  | ---- | ------- |\n  |      | en      |","location":"news.ts"}' :test='undefined' />

| 中文 | English |
  | ---- | ------- |
  |      | en      |

### Note Comments <Site url="apps.qoo-app.com" size="sm" />

<Route namespace="qoo-app" :data='{"path":"/notes/:lang?/note/:id","categories":["anime"],"example":"/qoo-app/notes/en/note/2329113","parameters":{"lang":"Language, see the table above, empty means `中文`","id":"Note ID, can be found in URL"},"features":{"requireConfig":false,"requirePuppeteer":false,"antiCrawler":false,"supportBT":false,"supportPodcast":false,"supportScihub":false},"name":"Note Comments","maintainers":["TonyRL"],"location":"notes/note.ts"}' :test='undefined' />

### Unknown <Site url="apps.qoo-app.com" size="sm" />

<Route namespace="qoo-app" :data='{"path":"/notes/:lang?/topic/:topic","name":"Unknown","maintainers":["TonyRL"],"location":"notes/topic.ts"}' :test='undefined' />

### User Notes <Site url="apps.qoo-app.com" size="sm" />

<Route namespace="qoo-app" :data='{"path":"/notes/:lang?/user/:uid","categories":["anime"],"example":"/qoo-app/notes/en/user/35399143","parameters":{"lang":"Language, see the table above, empty means `中文`","uid":"User ID, can be found in URL"},"features":{"requireConfig":false,"requirePuppeteer":false,"antiCrawler":false,"supportBT":false,"supportPodcast":false,"supportScihub":false},"name":"User Notes","maintainers":["TonyRL"],"location":"notes/user.ts"}' :test='undefined' />

### User Game Comments <Site url="apps.qoo-app.com" size="sm" />

<Route namespace="qoo-app" :data='{"path":"/user/:lang?/appComment/:uid","categories":["anime"],"example":"/qoo-app/user/en/appComment/35399143","parameters":{"lang":"Language, see the table above, empty means `中文`","uid":"User ID, can be found in URL"},"features":{"requireConfig":false,"requirePuppeteer":false,"antiCrawler":false,"supportBT":false,"supportPodcast":false,"supportScihub":false},"name":"User Game Comments","maintainers":["TonyRL"],"location":"user/app-comment.ts"}' :test='undefined' />

## Rawkuma <Site url="rawkuma.com"/>

### Manga <Site url="rawkuma.com" size="sm" />

<Route namespace="rawkuma" :data='{"path":"/manga/:id","categories":["anime"],"example":"/rawkuma/manga/tensei-shitara-dai-nana-ouji-dattanode-kimamani-majutsu-o-kiwamemasu","parameters":{"id":"Manga ID, can be found in URL"},"features":{"requireConfig":false,"requirePuppeteer":false,"antiCrawler":false,"supportBT":false,"supportPodcast":false,"supportScihub":false},"radar":[{"source":["rawkuma.com/manga/:id","rawkuma.com/"]}],"name":"Manga","maintainers":["nczitzk"],"location":"manga.ts"}' :test='{"code":0}' />

## THBWiki <Site url="thwiki.cc"/>

### Calendar <Site url="thwiki.cc/" size="sm" />

<Route namespace="thwiki" :data='{"path":"/calendar/:before?/:after?","categories":["anime"],"example":"/thwiki/calendar","parameters":{"before":"From how many days ago (default 30)","after":"To how many days after (default 30)"},"features":{"requireConfig":false,"requirePuppeteer":false,"antiCrawler":false,"supportBT":false,"supportPodcast":false,"supportScihub":false},"radar":[{"source":["thwiki.cc/","thwiki.cc/日程表"],"target":"/calendar"}],"name":"Calendar","maintainers":["aether17"],"url":"thwiki.cc/","location":"index.ts"}' :test='{"code":1,"message":"AssertionError: expected 503 to be 200 // Object.is equality\n    at /home/runner/work/RSSHub/RSSHub/lib/routes.test.ts:79:41\n    at processTicksAndRejections (node:internal/process/task_queues:95:5)\n    at runTest (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/@vitest+runner@2.0.4/node_modules/@vitest/runner/dist/index.js:955:11)\n    at async Promise.all (index 1562)\n    at runSuite (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/@vitest+runner@2.0.4/node_modules/@vitest/runner/dist/index.js:1097:13)\n    at runSuite (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/@vitest+runner@2.0.4/node_modules/@vitest/runner/dist/index.js:1111:15)\n    at runFiles (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/@vitest+runner@2.0.4/node_modules/@vitest/runner/dist/index.js:1168:5)\n    at startTests (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/@vitest+runner@2.0.4/node_modules/@vitest/runner/dist/index.js:1177:3)\n    at file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/vitest@2.0.4_@types+node@20.14.12_jsdom@24.1.1_bufferutil@4.0.8_utf-8-validate@5.0.10_/node_modules/vitest/dist/chunks/runtime-runBaseTests.Dq_sJZq9.js:132:11\n    at withEnv (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/vitest@2.0.4_@types+node@20.14.12_jsdom@24.1.1_bufferutil@4.0.8_utf-8-validate@5.0.10_/node_modules/vitest/dist/chunks/runtime-runBaseTests.Dq_sJZq9.js:94:5)\n    at run (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/vitest@2.0.4_@types+node@20.14.12_jsdom@24.1.1_bufferutil@4.0.8_utf-8-validate@5.0.10_/node_modules/vitest/dist/chunks/runtime-runBaseTests.Dq_sJZq9.js:117:3)\n    at runBaseTests (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/vitest@2.0.4_@types+node@20.14.12_jsdom@24.1.1_bufferutil@4.0.8_utf-8-validate@5.0.10_/node_modules/vitest/dist/vendor/base.Csk7BT3h.js:31:3)\n    at ForksBaseWorker.executeTests (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/vitest@2.0.4_@types+node@20.14.12_jsdom@24.1.1_bufferutil@4.0.8_utf-8-validate@5.0.10_/node_modules/vitest/dist/workers/forks.js:25:7)\n    at execute (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/vitest@2.0.4_@types+node@20.14.12_jsdom@24.1.1_bufferutil@4.0.8_utf-8-validate@5.0.10_/node_modules/vitest/dist/worker.js:116:5)\n    at onMessage (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/tinypool@1.0.0/node_modules/tinypool/dist/entry/process.js:54:20)"}' />

## VCB-Studio <Site url="vcb-s.com"/>

### Unknown <Site url="vcb-s.com/" size="sm" />

<Route namespace="vcb-s" :data='{"path":"/","radar":[{"source":["vcb-s.com/"],"target":""}],"name":"Unknown","maintainers":["cxfksword"],"url":"vcb-s.com/","location":"index.ts"}' :test='undefined' />

### 分类文章 <Site url="vcb-s.com/" size="sm" />

<Route namespace="vcb-s" :data='{"path":"/category/:cate","categories":["anime"],"example":"/vcb-s/category/works","parameters":{"cate":"分类"},"features":{"requireConfig":false,"requirePuppeteer":false,"antiCrawler":false,"supportBT":false,"supportPodcast":false,"supportScihub":false},"radar":[{"source":["vcb-s.com/archives/category/:cate"]}],"name":"分类文章","maintainers":["cxfksword"],"url":"vcb-s.com/","description":"| 作品项目 | 科普系列 | 计划与日志 |\n  | -------- | -------- | ---------- |\n  | works    | kb       | planlog    |","location":"category.ts"}' :test='undefined' />

| 作品项目 | 科普系列 | 计划与日志 |
  | -------- | -------- | ---------- |
  | works    | kb       | planlog    |

## X 漫画 <Site url="xmanhua.com"/>

### 最新动态 <Site url="xmanhua.com" size="sm" />

<Route namespace="xmanhua" :data='{"path":"/:uid","categories":["anime"],"example":"/xmanhua/73xm","parameters":{"uid":"漫画 id,在浏览器中可见，例如鬼灭之刃对应的 id 为 `73xm`"},"features":{"requireConfig":false,"requirePuppeteer":false,"antiCrawler":false,"supportBT":false,"supportPodcast":false,"supportScihub":false},"radar":[{"source":["xmanhua.com/:uid"]}],"name":"最新动态","maintainers":["Ye11"],"location":"index.ts"}' :test='{"code":0}' />

## yande <Site url="yande.re"/>

yande post

### posts <Site url="yande.re" size="sm" />

<Route namespace="yande" :data='{"path":"/post/popular_recent/:period?","categories":["anime"],"example":"/yande/post/popular_recent/1d","parameters":{"period":"展示时间"},"radar":[{"source":["yande.re/post/"]}],"name":"posts","maintainers":["fashioncj"],"description":"| 最近 24 小时    | 最近一周     | 最近一月    | 最近一年     | \n  | ------- | -------- | ------- | -------- | \n  | 1d | 1w | 1m ｜1y｜","location":"post.ts"}' :test='{"code":0}' />

| 最近 24 小时    | 最近一周     | 最近一月    | 最近一年     | 
  | ------- | -------- | ------- | -------- | 
  | 1d | 1w | 1m ｜1y｜

## 俺の 3D エロ動画 (oreno3d) <Site url="oreno3d.com"/>

:::tip
You can use some RSS parsing libraries (like `feedpraser` in `Python`) to receive the video update messages and download them automatically
:::

### Author Search <Site url="oreno3d.com" size="sm" />

<Route namespace="oreno3d" :data='{"path":["/authors/:authorid/:sort/:pagelimit?","/characters/:characterid/:sort/:pagelimit?","/origins/:originid/:sort/:pagelimit?","/search/:keyword/:sort/:pagelimit?","/tags/:tagid/:sort/:pagelimit?"],"categories":["anime"],"example":"/oreno3d/authors/3189/latest/1","parameters":{"authorid":"Author id, can be found in URL","sort":"Sort method, see the table above","pagelimit":"The maximum number of pages to be crawled, the default is 1"},"features":{"requireConfig":false,"requirePuppeteer":false,"antiCrawler":false,"supportBT":false,"supportPodcast":false,"supportScihub":false},"name":"Author Search","maintainers":["xueli_sherryli"],"description":"| favorites | hot | latest | popularity |\n  | --------- | --- | ------ | ---------- |\n  | favorites | hot | latest | popularity |","location":"main.ts"}' :test='{"code":0}' />

| favorites | hot | latest | popularity |
  | --------- | --- | ------ | ---------- |
  | favorites | hot | latest | popularity |

### Author Search <Site url="oreno3d.com" size="sm" />

<Route namespace="oreno3d" :data='{"path":["/authors/:authorid/:sort/:pagelimit?","/characters/:characterid/:sort/:pagelimit?","/origins/:originid/:sort/:pagelimit?","/search/:keyword/:sort/:pagelimit?","/tags/:tagid/:sort/:pagelimit?"],"categories":["anime"],"example":"/oreno3d/authors/3189/latest/1","parameters":{"authorid":"Author id, can be found in URL","sort":"Sort method, see the table above","pagelimit":"The maximum number of pages to be crawled, the default is 1"},"features":{"requireConfig":false,"requirePuppeteer":false,"antiCrawler":false,"supportBT":false,"supportPodcast":false,"supportScihub":false},"name":"Author Search","maintainers":["xueli_sherryli"],"description":"| favorites | hot | latest | popularity |\n  | --------- | --- | ------ | ---------- |\n  | favorites | hot | latest | popularity |","location":"main.ts"}' :test='{"code":1,"message":"AssertionError: expected 503 to be 200 // Object.is equality\n    at /home/runner/work/RSSHub/RSSHub/lib/routes.test.ts:79:41\n    at runTest (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/@vitest+runner@2.0.4/node_modules/@vitest/runner/dist/index.js:955:11)\n    at async Promise.all (index 1179)\n    at runSuite (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/@vitest+runner@2.0.4/node_modules/@vitest/runner/dist/index.js:1097:13)\n    at runSuite (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/@vitest+runner@2.0.4/node_modules/@vitest/runner/dist/index.js:1111:15)\n    at runFiles (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/@vitest+runner@2.0.4/node_modules/@vitest/runner/dist/index.js:1168:5)\n    at startTests (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/@vitest+runner@2.0.4/node_modules/@vitest/runner/dist/index.js:1177:3)\n    at file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/vitest@2.0.4_@types+node@20.14.12_jsdom@24.1.1_bufferutil@4.0.8_utf-8-validate@5.0.10_/node_modules/vitest/dist/chunks/runtime-runBaseTests.Dq_sJZq9.js:132:11\n    at withEnv (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/vitest@2.0.4_@types+node@20.14.12_jsdom@24.1.1_bufferutil@4.0.8_utf-8-validate@5.0.10_/node_modules/vitest/dist/chunks/runtime-runBaseTests.Dq_sJZq9.js:94:5)\n    at run (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/vitest@2.0.4_@types+node@20.14.12_jsdom@24.1.1_bufferutil@4.0.8_utf-8-validate@5.0.10_/node_modules/vitest/dist/chunks/runtime-runBaseTests.Dq_sJZq9.js:117:3)\n    at runBaseTests (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/vitest@2.0.4_@types+node@20.14.12_jsdom@24.1.1_bufferutil@4.0.8_utf-8-validate@5.0.10_/node_modules/vitest/dist/vendor/base.Csk7BT3h.js:31:3)\n    at ForksBaseWorker.executeTests (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/vitest@2.0.4_@types+node@20.14.12_jsdom@24.1.1_bufferutil@4.0.8_utf-8-validate@5.0.10_/node_modules/vitest/dist/workers/forks.js:25:7)\n    at execute (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/vitest@2.0.4_@types+node@20.14.12_jsdom@24.1.1_bufferutil@4.0.8_utf-8-validate@5.0.10_/node_modules/vitest/dist/worker.js:116:5)\n    at onMessage (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/tinypool@1.0.0/node_modules/tinypool/dist/entry/process.js:54:20)"}' />

| favorites | hot | latest | popularity |
  | --------- | --- | ------ | ---------- |
  | favorites | hot | latest | popularity |

### Author Search <Site url="oreno3d.com" size="sm" />

<Route namespace="oreno3d" :data='{"path":["/authors/:authorid/:sort/:pagelimit?","/characters/:characterid/:sort/:pagelimit?","/origins/:originid/:sort/:pagelimit?","/search/:keyword/:sort/:pagelimit?","/tags/:tagid/:sort/:pagelimit?"],"categories":["anime"],"example":"/oreno3d/authors/3189/latest/1","parameters":{"authorid":"Author id, can be found in URL","sort":"Sort method, see the table above","pagelimit":"The maximum number of pages to be crawled, the default is 1"},"features":{"requireConfig":false,"requirePuppeteer":false,"antiCrawler":false,"supportBT":false,"supportPodcast":false,"supportScihub":false},"name":"Author Search","maintainers":["xueli_sherryli"],"description":"| favorites | hot | latest | popularity |\n  | --------- | --- | ------ | ---------- |\n  | favorites | hot | latest | popularity |","location":"main.ts"}' :test='{"code":1,"message":"AssertionError: expected 503 to be 200 // Object.is equality\n    at /home/runner/work/RSSHub/RSSHub/lib/routes.test.ts:79:41\n    at runTest (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/@vitest+runner@2.0.4/node_modules/@vitest/runner/dist/index.js:955:11)\n    at async Promise.all (index 1180)\n    at runSuite (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/@vitest+runner@2.0.4/node_modules/@vitest/runner/dist/index.js:1097:13)\n    at runSuite (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/@vitest+runner@2.0.4/node_modules/@vitest/runner/dist/index.js:1111:15)\n    at runFiles (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/@vitest+runner@2.0.4/node_modules/@vitest/runner/dist/index.js:1168:5)\n    at startTests (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/@vitest+runner@2.0.4/node_modules/@vitest/runner/dist/index.js:1177:3)\n    at file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/vitest@2.0.4_@types+node@20.14.12_jsdom@24.1.1_bufferutil@4.0.8_utf-8-validate@5.0.10_/node_modules/vitest/dist/chunks/runtime-runBaseTests.Dq_sJZq9.js:132:11\n    at withEnv (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/vitest@2.0.4_@types+node@20.14.12_jsdom@24.1.1_bufferutil@4.0.8_utf-8-validate@5.0.10_/node_modules/vitest/dist/chunks/runtime-runBaseTests.Dq_sJZq9.js:94:5)\n    at run (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/vitest@2.0.4_@types+node@20.14.12_jsdom@24.1.1_bufferutil@4.0.8_utf-8-validate@5.0.10_/node_modules/vitest/dist/chunks/runtime-runBaseTests.Dq_sJZq9.js:117:3)\n    at runBaseTests (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/vitest@2.0.4_@types+node@20.14.12_jsdom@24.1.1_bufferutil@4.0.8_utf-8-validate@5.0.10_/node_modules/vitest/dist/vendor/base.Csk7BT3h.js:31:3)\n    at ForksBaseWorker.executeTests (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/vitest@2.0.4_@types+node@20.14.12_jsdom@24.1.1_bufferutil@4.0.8_utf-8-validate@5.0.10_/node_modules/vitest/dist/workers/forks.js:25:7)\n    at execute (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/vitest@2.0.4_@types+node@20.14.12_jsdom@24.1.1_bufferutil@4.0.8_utf-8-validate@5.0.10_/node_modules/vitest/dist/worker.js:116:5)\n    at onMessage (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/tinypool@1.0.0/node_modules/tinypool/dist/entry/process.js:54:20)"}' />

| favorites | hot | latest | popularity |
  | --------- | --- | ------ | ---------- |
  | favorites | hot | latest | popularity |

### Author Search <Site url="oreno3d.com" size="sm" />

<Route namespace="oreno3d" :data='{"path":["/authors/:authorid/:sort/:pagelimit?","/characters/:characterid/:sort/:pagelimit?","/origins/:originid/:sort/:pagelimit?","/search/:keyword/:sort/:pagelimit?","/tags/:tagid/:sort/:pagelimit?"],"categories":["anime"],"example":"/oreno3d/authors/3189/latest/1","parameters":{"authorid":"Author id, can be found in URL","sort":"Sort method, see the table above","pagelimit":"The maximum number of pages to be crawled, the default is 1"},"features":{"requireConfig":false,"requirePuppeteer":false,"antiCrawler":false,"supportBT":false,"supportPodcast":false,"supportScihub":false},"name":"Author Search","maintainers":["xueli_sherryli"],"description":"| favorites | hot | latest | popularity |\n  | --------- | --- | ------ | ---------- |\n  | favorites | hot | latest | popularity |","location":"main.ts"}' :test='{"code":1,"message":"AssertionError: expected 503 to be 200 // Object.is equality\n    at /home/runner/work/RSSHub/RSSHub/lib/routes.test.ts:79:41\n    at runTest (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/@vitest+runner@2.0.4/node_modules/@vitest/runner/dist/index.js:955:11)\n    at async Promise.all (index 1181)\n    at runSuite (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/@vitest+runner@2.0.4/node_modules/@vitest/runner/dist/index.js:1097:13)\n    at runSuite (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/@vitest+runner@2.0.4/node_modules/@vitest/runner/dist/index.js:1111:15)\n    at runFiles (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/@vitest+runner@2.0.4/node_modules/@vitest/runner/dist/index.js:1168:5)\n    at startTests (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/@vitest+runner@2.0.4/node_modules/@vitest/runner/dist/index.js:1177:3)\n    at file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/vitest@2.0.4_@types+node@20.14.12_jsdom@24.1.1_bufferutil@4.0.8_utf-8-validate@5.0.10_/node_modules/vitest/dist/chunks/runtime-runBaseTests.Dq_sJZq9.js:132:11\n    at withEnv (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/vitest@2.0.4_@types+node@20.14.12_jsdom@24.1.1_bufferutil@4.0.8_utf-8-validate@5.0.10_/node_modules/vitest/dist/chunks/runtime-runBaseTests.Dq_sJZq9.js:94:5)\n    at run (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/vitest@2.0.4_@types+node@20.14.12_jsdom@24.1.1_bufferutil@4.0.8_utf-8-validate@5.0.10_/node_modules/vitest/dist/chunks/runtime-runBaseTests.Dq_sJZq9.js:117:3)\n    at runBaseTests (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/vitest@2.0.4_@types+node@20.14.12_jsdom@24.1.1_bufferutil@4.0.8_utf-8-validate@5.0.10_/node_modules/vitest/dist/vendor/base.Csk7BT3h.js:31:3)\n    at ForksBaseWorker.executeTests (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/vitest@2.0.4_@types+node@20.14.12_jsdom@24.1.1_bufferutil@4.0.8_utf-8-validate@5.0.10_/node_modules/vitest/dist/workers/forks.js:25:7)\n    at execute (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/vitest@2.0.4_@types+node@20.14.12_jsdom@24.1.1_bufferutil@4.0.8_utf-8-validate@5.0.10_/node_modules/vitest/dist/worker.js:116:5)\n    at onMessage (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/tinypool@1.0.0/node_modules/tinypool/dist/entry/process.js:54:20)"}' />

| favorites | hot | latest | popularity |
  | --------- | --- | ------ | ---------- |
  | favorites | hot | latest | popularity |

### Author Search <Site url="oreno3d.com" size="sm" />

<Route namespace="oreno3d" :data='{"path":["/authors/:authorid/:sort/:pagelimit?","/characters/:characterid/:sort/:pagelimit?","/origins/:originid/:sort/:pagelimit?","/search/:keyword/:sort/:pagelimit?","/tags/:tagid/:sort/:pagelimit?"],"categories":["anime"],"example":"/oreno3d/authors/3189/latest/1","parameters":{"authorid":"Author id, can be found in URL","sort":"Sort method, see the table above","pagelimit":"The maximum number of pages to be crawled, the default is 1"},"features":{"requireConfig":false,"requirePuppeteer":false,"antiCrawler":false,"supportBT":false,"supportPodcast":false,"supportScihub":false},"name":"Author Search","maintainers":["xueli_sherryli"],"description":"| favorites | hot | latest | popularity |\n  | --------- | --- | ------ | ---------- |\n  | favorites | hot | latest | popularity |","location":"main.ts"}' :test='{"code":1,"message":"AssertionError: expected 503 to be 200 // Object.is equality\n    at /home/runner/work/RSSHub/RSSHub/lib/routes.test.ts:79:41\n    at runTest (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/@vitest+runner@2.0.4/node_modules/@vitest/runner/dist/index.js:955:11)\n    at async Promise.all (index 1182)\n    at runSuite (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/@vitest+runner@2.0.4/node_modules/@vitest/runner/dist/index.js:1097:13)\n    at runSuite (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/@vitest+runner@2.0.4/node_modules/@vitest/runner/dist/index.js:1111:15)\n    at runFiles (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/@vitest+runner@2.0.4/node_modules/@vitest/runner/dist/index.js:1168:5)\n    at startTests (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/@vitest+runner@2.0.4/node_modules/@vitest/runner/dist/index.js:1177:3)\n    at file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/vitest@2.0.4_@types+node@20.14.12_jsdom@24.1.1_bufferutil@4.0.8_utf-8-validate@5.0.10_/node_modules/vitest/dist/chunks/runtime-runBaseTests.Dq_sJZq9.js:132:11\n    at withEnv (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/vitest@2.0.4_@types+node@20.14.12_jsdom@24.1.1_bufferutil@4.0.8_utf-8-validate@5.0.10_/node_modules/vitest/dist/chunks/runtime-runBaseTests.Dq_sJZq9.js:94:5)\n    at run (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/vitest@2.0.4_@types+node@20.14.12_jsdom@24.1.1_bufferutil@4.0.8_utf-8-validate@5.0.10_/node_modules/vitest/dist/chunks/runtime-runBaseTests.Dq_sJZq9.js:117:3)\n    at runBaseTests (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/vitest@2.0.4_@types+node@20.14.12_jsdom@24.1.1_bufferutil@4.0.8_utf-8-validate@5.0.10_/node_modules/vitest/dist/vendor/base.Csk7BT3h.js:31:3)\n    at ForksBaseWorker.executeTests (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/vitest@2.0.4_@types+node@20.14.12_jsdom@24.1.1_bufferutil@4.0.8_utf-8-validate@5.0.10_/node_modules/vitest/dist/workers/forks.js:25:7)\n    at execute (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/vitest@2.0.4_@types+node@20.14.12_jsdom@24.1.1_bufferutil@4.0.8_utf-8-validate@5.0.10_/node_modules/vitest/dist/worker.js:116:5)\n    at onMessage (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/tinypool@1.0.0/node_modules/tinypool/dist/entry/process.js:54:20)"}' />

| favorites | hot | latest | popularity |
  | --------- | --- | ------ | ---------- |
  | favorites | hot | latest | popularity |

## 巴哈姆特電玩資訊站 <Site url="acg.gamer.com.tw"/>

### GNN 新聞 <Site url="acg.gamer.com.tw" size="sm" />

<Route namespace="gamer" :data='{"path":"/gnn/:category?","categories":["anime"],"example":"/gamer/gnn/1","parameters":{"category":"版块"},"features":{"requireConfig":false,"requirePuppeteer":false,"antiCrawler":true,"supportBT":false,"supportPodcast":false,"supportScihub":false},"name":"GNN 新聞","maintainers":["Arracc","ladeng07"],"description":"| 首頁 | PC | TV 掌機 | 手機遊戲 | 動漫畫 | 主題報導 | 活動展覽 | 電競 |\n  | ---- | -- | ------- | -------- | ------ | -------- | -------- | ---- |\n  | 缺省 | 1  | 3       | 4        | 5      | 9        | 11       | 13   |\n\n  | Switch | PS5 | PS4 | XboxOne | XboxSX | PC 單機 | PC 線上 | iOS | Android | Web | 漫畫  | 動畫  |\n  | ------ | --- | --- | ------- | ------ | ------- | ------- | --- | ------- | --- | ----- | ----- |\n  | ns     | ps5 | ps4 | xbone   | xbsx   | pc      | olg     | ios | android | web | comic | anime |","location":"gnn-index.ts"}' :test='{"code":0}' />

| 首頁 | PC | TV 掌機 | 手機遊戲 | 動漫畫 | 主題報導 | 活動展覽 | 電競 |
  | ---- | -- | ------- | -------- | ------ | -------- | -------- | ---- |
  | 缺省 | 1  | 3       | 4        | 5      | 9        | 11       | 13   |

  | Switch | PS5 | PS4 | XboxOne | XboxSX | PC 單機 | PC 線上 | iOS | Android | Web | 漫畫  | 動畫  |
  | ------ | --- | --- | ------- | ------ | ------- | ------- | --- | ------- | --- | ----- | ----- |
  | ns     | ps5 | ps4 | xbone   | xbsx   | pc      | olg     | ios | android | web | comic | anime |

### 動畫瘋 - 動畫 <Site url="acg.gamer.com.tw" size="sm" />

<Route namespace="gamer" :data='{"path":"/ani/anime/:sn","categories":["anime"],"example":"/gamer/ani/anime/36868","parameters":{"sn":"動畫 sn，在 URL 可以找到"},"features":{"requireConfig":false,"requirePuppeteer":false,"antiCrawler":false,"supportBT":false,"supportPodcast":false,"supportScihub":false},"name":"動畫瘋 - 動畫","maintainers":[],"location":"ani/anime.ts"}' :test='{"code":0}' />

### 動畫瘋 - 最後更新 <Site url="ani.gamer.com.tw/" size="sm" />

<Route namespace="gamer" :data='{"path":"/ani/new_anime","categories":["anime"],"example":"/gamer/ani/new_anime","parameters":{},"features":{"requireConfig":false,"requirePuppeteer":false,"antiCrawler":false,"supportBT":false,"supportPodcast":false,"supportScihub":false},"radar":[{"source":["ani.gamer.com.tw/"],"target":"/new_anime"}],"name":"動畫瘋 - 最後更新","maintainers":[],"url":"ani.gamer.com.tw/","location":"ani/new-anime.ts"}' :test='{"code":0}' />

### 熱門推薦 <Site url="acg.gamer.com.tw" size="sm" />

<Route namespace="gamer" :data='{"path":"/hot/:bsn","categories":["anime"],"example":"/gamer/hot/47157","parameters":{"bsn":"板块 id，在 URL 可以找到"},"features":{"requireConfig":false,"requirePuppeteer":false,"antiCrawler":false,"supportBT":false,"supportPodcast":false,"supportScihub":false},"name":"熱門推薦","maintainers":["nczitzk","TonyRL"],"location":"hot.ts"}' :test='{"code":1,"message":"AssertionError: expected 503 to be 200 // Object.is equality\n    at /home/runner/work/RSSHub/RSSHub/lib/routes.test.ts:79:41\n    at processTicksAndRejections (node:internal/process/task_queues:95:5)\n    at runTest (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/@vitest+runner@2.0.4/node_modules/@vitest/runner/dist/index.js:955:11)\n    at async Promise.all (index 553)\n    at runSuite (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/@vitest+runner@2.0.4/node_modules/@vitest/runner/dist/index.js:1097:13)\n    at runSuite (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/@vitest+runner@2.0.4/node_modules/@vitest/runner/dist/index.js:1111:15)\n    at runFiles (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/@vitest+runner@2.0.4/node_modules/@vitest/runner/dist/index.js:1168:5)\n    at startTests (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/@vitest+runner@2.0.4/node_modules/@vitest/runner/dist/index.js:1177:3)\n    at file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/vitest@2.0.4_@types+node@20.14.12_jsdom@24.1.1_bufferutil@4.0.8_utf-8-validate@5.0.10_/node_modules/vitest/dist/chunks/runtime-runBaseTests.Dq_sJZq9.js:132:11\n    at withEnv (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/vitest@2.0.4_@types+node@20.14.12_jsdom@24.1.1_bufferutil@4.0.8_utf-8-validate@5.0.10_/node_modules/vitest/dist/chunks/runtime-runBaseTests.Dq_sJZq9.js:94:5)\n    at run (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/vitest@2.0.4_@types+node@20.14.12_jsdom@24.1.1_bufferutil@4.0.8_utf-8-validate@5.0.10_/node_modules/vitest/dist/chunks/runtime-runBaseTests.Dq_sJZq9.js:117:3)\n    at runBaseTests (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/vitest@2.0.4_@types+node@20.14.12_jsdom@24.1.1_bufferutil@4.0.8_utf-8-validate@5.0.10_/node_modules/vitest/dist/vendor/base.Csk7BT3h.js:31:3)\n    at ForksBaseWorker.executeTests (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/vitest@2.0.4_@types+node@20.14.12_jsdom@24.1.1_bufferutil@4.0.8_utf-8-validate@5.0.10_/node_modules/vitest/dist/workers/forks.js:25:7)\n    at execute (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/vitest@2.0.4_@types+node@20.14.12_jsdom@24.1.1_bufferutil@4.0.8_utf-8-validate@5.0.10_/node_modules/vitest/dist/worker.js:116:5)\n    at onMessage (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/tinypool@1.0.0/node_modules/tinypool/dist/entry/process.js:54:20)"}' />

## 包子漫画 <Site url="www.baozimh.com"/>

### 订阅漫画 <Site url="www.baozimh.com" size="sm" />

<Route namespace="baozimh" :data='{"path":"/comic/:name","categories":["anime"],"example":"/baozimh/comic/guowangpaiming-shiricaofu","parameters":{"name":"漫画名称，在漫画链接可以得到(`comic/` 后的那段)"},"features":{"requireConfig":false,"requirePuppeteer":false,"antiCrawler":false,"supportBT":false,"supportPodcast":false,"supportScihub":false},"radar":[{"source":["www.baozimh.com/comic/:name"]}],"name":"订阅漫画","maintainers":["Fatpandac"],"location":"index.ts"}' :test='{"code":0}' />

## 动漫之家 <Site url="news.dmzj.com"/>

### 新闻站 <Site url="news.dmzj.com/" size="sm" />

<Route namespace="dmzj" :data='{"path":"/news/:category?","categories":["anime"],"example":"/dmzj/news/donghuaqingbao","parameters":{"category":"类别"},"features":{"requireConfig":false,"requirePuppeteer":false,"antiCrawler":false,"supportBT":false,"supportPodcast":false,"supportScihub":false},"radar":[{"source":["news.dmzj.com/"],"target":"/news"}],"name":"新闻站","maintainers":["vzz64"],"url":"news.dmzj.com/","description":"| 漫画情报      | 轻小说情报          | 动漫周边       | 声优情报        | 音乐资讯    | 游戏资讯   | 美图欣赏      | 漫展情报       | 大杂烩  |\n  | ------------- | ------------------- | -------------- | --------------- | ----------- | ---------- | ------------- | -------------- | ------- |\n  | manhuaqingbao | qingxiaoshuoqingbao | manhuazhoubian | shengyouqingbao | yinyuezixun | youxizixun | meituxinshang | manzhanqingbao | dazahui |","location":"news.ts"}' :test='{"code":0}' />

| 漫画情报      | 轻小说情报          | 动漫周边       | 声优情报        | 音乐资讯    | 游戏资讯   | 美图欣赏      | 漫展情报       | 大杂烩  |
  | ------------- | ------------------- | -------------- | --------------- | ----------- | ---------- | ------------- | -------------- | ------- |
  | manhuaqingbao | qingxiaoshuoqingbao | manhuazhoubian | shengyouqingbao | yinyuezixun | youxizixun | meituxinshang | manzhanqingbao | dazahui |

## 動漫狂 <Site url="cartoonmad.com"/>

### 漫画更新 <Site url="cartoonmad.com" size="sm" />

<Route namespace="cartoonmad" :data='{"path":"/comic/:id","categories":["anime"],"example":"/cartoonmad/comic/5827","parameters":{"id":"漫画ID"},"features":{"requireConfig":false,"requirePuppeteer":false,"antiCrawler":false,"supportBT":false,"supportPodcast":false,"supportScihub":false},"radar":[{"source":["cartoonmad.com/comic/:id"]}],"name":"漫画更新","maintainers":["KellyHwong"],"location":"comic.ts"}' :test='{"code":0}' />

## 番组放送 <Site url="bgmlist.com"/>

### 开播提醒 <Site url="bgmlist.com" size="sm" />

<Route namespace="bgmlist" :data='{"path":"/onair/:lang?","categories":["anime"],"example":"/bgmlist/onair/zh-Hans","parameters":{"lang":"语言"},"features":{"requireConfig":false,"requirePuppeteer":false,"antiCrawler":false,"supportBT":false,"supportPodcast":false,"supportScihub":false},"name":"开播提醒","maintainers":["x2cf"],"location":"onair.ts"}' :test='{"code":1,"message":"AssertionError: expected 324807144266 to be less than 311040000000\n    at checkDate (/home/runner/work/RSSHub/RSSHub/lib/routes.test.ts:36:46)\n    at checkRSS (/home/runner/work/RSSHub/RSSHub/lib/routes.test.ts:61:13)\n    at processTicksAndRejections (node:internal/process/task_queues:95:5)\n    at /home/runner/work/RSSHub/RSSHub/lib/routes.test.ts:80:17\n    at runTest (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/@vitest+runner@2.0.4/node_modules/@vitest/runner/dist/index.js:955:11)\n    at async Promise.all (index 105)\n    at runSuite (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/@vitest+runner@2.0.4/node_modules/@vitest/runner/dist/index.js:1097:13)\n    at runSuite (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/@vitest+runner@2.0.4/node_modules/@vitest/runner/dist/index.js:1111:15)\n    at runFiles (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/@vitest+runner@2.0.4/node_modules/@vitest/runner/dist/index.js:1168:5)\n    at startTests (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/@vitest+runner@2.0.4/node_modules/@vitest/runner/dist/index.js:1177:3)\n    at file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/vitest@2.0.4_@types+node@20.14.12_jsdom@24.1.1_bufferutil@4.0.8_utf-8-validate@5.0.10_/node_modules/vitest/dist/chunks/runtime-runBaseTests.Dq_sJZq9.js:132:11\n    at withEnv (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/vitest@2.0.4_@types+node@20.14.12_jsdom@24.1.1_bufferutil@4.0.8_utf-8-validate@5.0.10_/node_modules/vitest/dist/chunks/runtime-runBaseTests.Dq_sJZq9.js:94:5)\n    at run (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/vitest@2.0.4_@types+node@20.14.12_jsdom@24.1.1_bufferutil@4.0.8_utf-8-validate@5.0.10_/node_modules/vitest/dist/chunks/runtime-runBaseTests.Dq_sJZq9.js:117:3)\n    at runBaseTests (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/vitest@2.0.4_@types+node@20.14.12_jsdom@24.1.1_bufferutil@4.0.8_utf-8-validate@5.0.10_/node_modules/vitest/dist/vendor/base.Csk7BT3h.js:31:3)\n    at ForksBaseWorker.executeTests (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/vitest@2.0.4_@types+node@20.14.12_jsdom@24.1.1_bufferutil@4.0.8_utf-8-validate@5.0.10_/node_modules/vitest/dist/workers/forks.js:25:7)\n    at execute (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/vitest@2.0.4_@types+node@20.14.12_jsdom@24.1.1_bufferutil@4.0.8_utf-8-validate@5.0.10_/node_modules/vitest/dist/worker.js:116:5)"}' />

## 风之动漫 <Site url="manhua.fffdm.com"/>

### 在线漫画 <Site url="manhua.fffdm.com" size="sm" />

<Route namespace="fffdm" :data='{"path":"/manhua/:id/:cdn?","categories":["anime"],"example":"/fffdm/manhua/93","parameters":{"id":"漫画ID。默认获取全部，建议使用通用参数limit获取指定数量","cdn":"cdn加速器。默认5，当前可选1-5"},"features":{"requireConfig":false,"requirePuppeteer":false,"antiCrawler":false,"supportBT":false,"supportPodcast":false,"supportScihub":false},"radar":[{"source":["www.fffdm.com/manhua/:id","www.fffdm.com/:id"],"target":"/manhua/:id"}],"name":"在线漫画","maintainers":["zytomorrow"],"location":"manhua/manhua.ts"}' :test='{"code":1,"message":"AssertionError: expected [ …(20) ] to not include &#39;https://manhua.fffdm.com/93/020/&#39;\n    at Proxy.<anonymous> (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/@vitest+expect@2.0.4/node_modules/@vitest/expect/dist/index.js:1135:17)\n    at Proxy.<anonymous> (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/@vitest+expect@2.0.4/node_modules/@vitest/expect/dist/index.js:912:17)\n    at Proxy.methodWrapper (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/chai@5.1.1/node_modules/chai/chai.js:1591:25)\n    at checkRSS (/home/runner/work/RSSHub/RSSHub/lib/routes.test.ts:65:27)\n    at processTicksAndRejections (node:internal/process/task_queues:95:5)\n    at /home/runner/work/RSSHub/RSSHub/lib/routes.test.ts:80:17\n    at runTest (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/@vitest+runner@2.0.4/node_modules/@vitest/runner/dist/index.js:955:11)\n    at async Promise.all (index 510)\n    at runSuite (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/@vitest+runner@2.0.4/node_modules/@vitest/runner/dist/index.js:1097:13)\n    at runSuite (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/@vitest+runner@2.0.4/node_modules/@vitest/runner/dist/index.js:1111:15)\n    at runFiles (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/@vitest+runner@2.0.4/node_modules/@vitest/runner/dist/index.js:1168:5)\n    at startTests (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/@vitest+runner@2.0.4/node_modules/@vitest/runner/dist/index.js:1177:3)\n    at file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/vitest@2.0.4_@types+node@20.14.12_jsdom@24.1.1_bufferutil@4.0.8_utf-8-validate@5.0.10_/node_modules/vitest/dist/chunks/runtime-runBaseTests.Dq_sJZq9.js:132:11\n    at withEnv (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/vitest@2.0.4_@types+node@20.14.12_jsdom@24.1.1_bufferutil@4.0.8_utf-8-validate@5.0.10_/node_modules/vitest/dist/chunks/runtime-runBaseTests.Dq_sJZq9.js:94:5)\n    at run (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/vitest@2.0.4_@types+node@20.14.12_jsdom@24.1.1_bufferutil@4.0.8_utf-8-validate@5.0.10_/node_modules/vitest/dist/chunks/runtime-runBaseTests.Dq_sJZq9.js:117:3)\n    at runBaseTests (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/vitest@2.0.4_@types+node@20.14.12_jsdom@24.1.1_bufferutil@4.0.8_utf-8-validate@5.0.10_/node_modules/vitest/dist/vendor/base.Csk7BT3h.js:31:3)"}' />

## 幻之羁绊动漫网 <Site url="005.tv"/>

### 资讯 <Site url="005.tv" size="sm" />

<Route namespace="005" :data='{"path":"/:category?","name":"资讯","url":"005.tv","maintainers":["nczitzk"],"example":"/005/zx","parameters":{"category":"分类，可在对应分类页 URL 中找到，默认为二次元资讯"},"description":"\n  | 二次元资讯 | 慢慢说 | 道听途说 | 展会资讯 |\n  | ---------- | ------ | -------- | -------- |\n  | zx         | zwh    | dtts     | zh       |\n    ","categories":["anime"],"features":{"requireConfig":false,"requirePuppeteer":false,"antiCrawler":false,"supportRadar":true,"supportBT":false,"supportPodcast":false,"supportScihub":false},"radar":[{"source":["005.tv/:category"]},{"title":"二次元资讯","source":["005.tv/zx/"],"target":"/005/zx"},{"title":"慢慢说","source":["005.tv/zwh/"],"target":"/005/zwh"},{"title":"道听途说","source":["005.tv/dtts/"],"target":"/005/dtts"},{"title":"展会资讯","source":["005.tv/zh/"],"target":"/005/zh"}],"location":"index.ts"}' :test='undefined' />


  | 二次元资讯 | 慢慢说 | 道听途说 | 展会资讯 |
  | ---------- | ------ | -------- | -------- |
  | zx         | zwh    | dtts     | zh       |
    

## 禁漫天堂 <Site url="18comic.org"/>

:::tip
禁漫天堂有多个备用域名，本路由默认使用域名 `https://jmcomic.me`，若该域名无法访问，可以通过在路由最后加上 `?domain=<域名>` 指定路由访问的域名。如指定备用域名为 `https://jmcomic1.me`，则在所有禁漫天堂路由最后加上 `?domain=jmcomic1.me` 即可，此时路由为 [`/18comic?domain=jmcomic1.me`](https://rsshub.app/18comic?domain=jmcomic1.me)
:::

### 成人 A 漫 <Site url="jmcomic.group/" size="sm" />

<Route namespace="18comic" :data='{"path":"/:category?/:time?/:order?/:keyword?","categories":["anime"],"example":"/18comic","parameters":{"category":"分类，见下表，默认为 `all` 即全部","time":"时间范围，见下表，默认为 `a` 即全部","order":"排列顺序，见下表，默认为 `mr` 即最新","keyword":"关键字，见下表，默认为空"},"features":{"requireConfig":false,"requirePuppeteer":false,"antiCrawler":true,"supportBT":false,"supportPodcast":false,"supportScihub":false},"radar":[{"source":["jmcomic.group/"]}],"name":"成人 A 漫","maintainers":["nczitzk"],"url":"jmcomic.group/","description":"分类\n\n  | 全部 | 其他漫畫 | 同人   | 韓漫   | 美漫   | 短篇  | 单本   |\n  | ---- | -------- | ------ | ------ | ------ | ----- | ------ |\n  | all  | another  | doujin | hanman | meiman | short | single |\n\n  时间范围\n\n  | 全部 | 今天 | 这周 | 本月 |\n  | ---- | ---- | ---- | ---- |\n  | a    | t    | w    | m    |\n\n  排列顺序\n\n  | 最新 | 最多点阅的 | 最多图片 | 最高评分 | 最多评论 | 最多爱心 |\n  | ---- | ---------- | -------- | -------- | -------- | -------- |\n  | mr   | mv         | mp       | tr       | md       | tf       |\n\n  关键字（供参考）\n\n  | YAOI | 女性向 | NTR | 非 H | 3D | 獵奇 |\n  | ---- | ------ | --- | ---- | -- | ---- |","location":"index.ts"}' :test='undefined' />

分类

  | 全部 | 其他漫畫 | 同人   | 韓漫   | 美漫   | 短篇  | 单本   |
  | ---- | -------- | ------ | ------ | ------ | ----- | ------ |
  | all  | another  | doujin | hanman | meiman | short | single |

  时间范围

  | 全部 | 今天 | 这周 | 本月 |
  | ---- | ---- | ---- | ---- |
  | a    | t    | w    | m    |

  排列顺序

  | 最新 | 最多点阅的 | 最多图片 | 最高评分 | 最多评论 | 最多爱心 |
  | ---- | ---------- | -------- | -------- | -------- | -------- |
  | mr   | mv         | mp       | tr       | md       | tf       |

  关键字（供参考）

  | YAOI | 女性向 | NTR | 非 H | 3D | 獵奇 |
  | ---- | ------ | --- | ---- | -- | ---- |

### 搜索 <Site url="jmcomic.group/" size="sm" />

<Route namespace="18comic" :data='{"path":"/search/:option?/:category?/:keyword?/:time?/:order?","categories":["anime"],"example":"/18comic/search/photos/all/NTR","parameters":{"option":"选项，可选 `video` 和 `photos`，默认为 `photos`","category":"分类，同上表，默认为 `all` 即全部","keyword":"关键字，同上表，默认为空","time":"时间范围，同上表，默认为 `a` 即全部","order":"排列顺序，同上表，默认为 `mr` 即最新"},"features":{"requireConfig":false,"requirePuppeteer":false,"antiCrawler":true,"supportBT":false,"supportPodcast":false,"supportScihub":false},"radar":[{"source":["jmcomic.group/"],"target":"/:category?/:time?/:order?/:keyword?"}],"name":"搜索","maintainers":[],"url":"jmcomic.group/","description":":::tip\n  关键字必须超过两个字，这是来自网站的限制。\n  :::","location":"search.ts"}' :test='undefined' />

:::tip
  关键字必须超过两个字，这是来自网站的限制。
  :::

### 文庫 <Site url="jmcomic.group/" size="sm" />

<Route namespace="18comic" :data='{"path":"/blogs/:category?","categories":["anime"],"example":"/18comic/blogs","parameters":{"category":"分类，见下表，默认为空即全部"},"features":{"requireConfig":false,"requirePuppeteer":false,"antiCrawler":true,"supportBT":false,"supportPodcast":false,"supportScihub":false},"radar":[{"source":["jmcomic.group/"]}],"name":"文庫","maintainers":["nczitzk"],"url":"jmcomic.group/","description":"分类\n\n  | 全部 | 紳夜食堂 | 遊戲文庫 | JG GAMES | 模型山下 |\n  | ---- | -------- | -------- | -------- | -------- |\n  |      | dinner   | raiders  | jg       | figure   |","location":"blogs.ts"}' :test='undefined' />

分类

  | 全部 | 紳夜食堂 | 遊戲文庫 | JG GAMES | 模型山下 |
  | ---- | -------- | -------- | -------- | -------- |
  |      | dinner   | raiders  | jg       | figure   |

### 专辑 <Site url="jmcomic.group/" size="sm" />

<Route namespace="18comic" :data='{"path":"/album/:id","categories":["anime"],"example":"/18comic/album/292282","parameters":{"id":"专辑 id，可在专辑页 URL 中找到"},"features":{"requireConfig":false,"requirePuppeteer":false,"antiCrawler":true,"supportBT":false,"supportPodcast":false,"supportScihub":false},"radar":[{"source":["jmcomic.group/"]}],"name":"专辑","maintainers":["nczitzk"],"url":"jmcomic.group/","description":":::tip\n  专辑 id 不包括 URL 中标题的部分。\n  :::","location":"album.ts"}' :test='undefined' />

:::tip
  专辑 id 不包括 URL 中标题的部分。
  :::

## 看漫画 <Site url="www.manhuagui.com"/>

### 漫画更新 <Site url="www.manhuagui.com" size="sm" />

<Route namespace="manhuagui" :data='{"path":["/comic/:id/:chapterCnt?","/:domain?/comic/:id/:chapterCnt?"],"categories":["anime"],"example":"/manhuagui/comic/22942/5","parameters":{"id":"漫画ID","chapterCnt":"返回章节的数量，默认为0，返回所有章节"},"features":{"requireConfig":false,"requirePuppeteer":false,"antiCrawler":true,"supportBT":false,"supportPodcast":false,"supportScihub":false},"radar":[{"source":["www.mhgui.com/comic/:id/"],"target":"/comic/:id"}],"name":"漫画更新","maintainers":["MegrezZhu"],"location":"comic.ts"}' :test='{"code":0}' />

### 漫画更新 <Site url="www.manhuagui.com" size="sm" />

<Route namespace="manhuagui" :data='{"path":["/comic/:id/:chapterCnt?","/:domain?/comic/:id/:chapterCnt?"],"categories":["anime"],"example":"/manhuagui/comic/22942/5","parameters":{"id":"漫画ID","chapterCnt":"返回章节的数量，默认为0，返回所有章节"},"features":{"requireConfig":false,"requirePuppeteer":false,"antiCrawler":true,"supportBT":false,"supportPodcast":false,"supportScihub":false},"radar":[{"source":["www.mhgui.com/comic/:id/"],"target":"/comic/:id"}],"name":"漫画更新","maintainers":["MegrezZhu"],"location":"comic.ts"}' :test='{"code":0}' />

### 漫画个人订阅 <Site url="www.mhgui.com/user/book/shelf" size="sm" />

<Route namespace="manhuagui" :data='{"path":"/subscribe","categories":["anime"],"example":"/manhuagui/subscribe","parameters":{},"features":{"requireConfig":[{"name":"MHGUI_COOKIE","description":""}],"requirePuppeteer":false,"antiCrawler":false,"supportBT":false,"supportPodcast":false,"supportScihub":false},"radar":[{"source":["www.mhgui.com/user/book/shelf"]}],"name":"漫画个人订阅","maintainers":["shininome"],"url":"www.mhgui.com/user/book/shelf","description":":::tip\n  个人订阅需要自建\n  环境变量需要添加 MHGUI_COOKIE\n  :::","location":"subscribe.ts"}' :test='undefined' />

:::tip
  个人订阅需要自建
  环境变量需要添加 MHGUI_COOKIE
  :::

## 拷贝漫画 <Site url="copymanga.com"/>

### 漫画更新 <Site url="copymanga.com" size="sm" />

<Route namespace="copymanga" :data='{"path":"/comic/:id/:chapterCnt?","categories":["anime"],"example":"/copymanga/comic/dianjuren/5","parameters":{"id":"漫画ID","chapterCnt":"返回章节的数量，默认为 `10`"},"features":{"requireConfig":false,"requirePuppeteer":false,"antiCrawler":false,"supportBT":false,"supportPodcast":false,"supportScihub":false},"name":"漫画更新","maintainers":["btdwv","marvolo666","yan12125"],"location":"comic.ts"}' :test='{"code":0}' />

## 来漫画 <Site url="www.laimanhua8.com"/>

### 漫画列表 <Site url="www.laimanhua8.com" size="sm" />

<Route namespace="laimanhua" :data='{"path":"/:id","categories":["anime"],"example":"/laimanhua/tiandikangzhanjiVERSUS","parameters":{"id":"漫画 ID，可在 URL 中找到"},"features":{"requireConfig":false,"requirePuppeteer":false,"antiCrawler":false,"supportBT":false,"supportPodcast":false,"supportScihub":false},"radar":[{"source":["www.laimanhua8.com/kanmanhua/:id"]}],"name":"漫画列表","maintainers":["TonyRL"],"location":"index.ts"}' :test='{"code":1,"message":"AssertionError: expected [ …(7) ] to not include &#39;https://www.laimanhua8.com/kanmanhua/…&#39;\n    at Proxy.<anonymous> (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/@vitest+expect@2.0.4/node_modules/@vitest/expect/dist/index.js:1135:17)\n    at Proxy.<anonymous> (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/@vitest+expect@2.0.4/node_modules/@vitest/expect/dist/index.js:912:17)\n    at Proxy.methodWrapper (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/chai@5.1.1/node_modules/chai/chai.js:1591:25)\n    at checkRSS (/home/runner/work/RSSHub/RSSHub/lib/routes.test.ts:65:27)\n    at processTicksAndRejections (node:internal/process/task_queues:95:5)\n    at /home/runner/work/RSSHub/RSSHub/lib/routes.test.ts:80:17\n    at runTest (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/@vitest+runner@2.0.4/node_modules/@vitest/runner/dist/index.js:955:11)\n    at async Promise.all (index 921)\n    at runSuite (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/@vitest+runner@2.0.4/node_modules/@vitest/runner/dist/index.js:1097:13)\n    at runSuite (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/@vitest+runner@2.0.4/node_modules/@vitest/runner/dist/index.js:1111:15)\n    at runFiles (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/@vitest+runner@2.0.4/node_modules/@vitest/runner/dist/index.js:1168:5)\n    at startTests (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/@vitest+runner@2.0.4/node_modules/@vitest/runner/dist/index.js:1177:3)\n    at file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/vitest@2.0.4_@types+node@20.14.12_jsdom@24.1.1_bufferutil@4.0.8_utf-8-validate@5.0.10_/node_modules/vitest/dist/chunks/runtime-runBaseTests.Dq_sJZq9.js:132:11\n    at withEnv (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/vitest@2.0.4_@types+node@20.14.12_jsdom@24.1.1_bufferutil@4.0.8_utf-8-validate@5.0.10_/node_modules/vitest/dist/chunks/runtime-runBaseTests.Dq_sJZq9.js:94:5)\n    at run (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/vitest@2.0.4_@types+node@20.14.12_jsdom@24.1.1_bufferutil@4.0.8_utf-8-validate@5.0.10_/node_modules/vitest/dist/chunks/runtime-runBaseTests.Dq_sJZq9.js:117:3)\n    at runBaseTests (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/vitest@2.0.4_@types+node@20.14.12_jsdom@24.1.1_bufferutil@4.0.8_utf-8-validate@5.0.10_/node_modules/vitest/dist/vendor/base.Csk7BT3h.js:31:3)"}' />

## 漫小肆韓漫 <Site url="freexcomic.com"/>

### 漫画更新 <Site url="www.jjmhw.cc" size="sm" />

<Route namespace="freexcomic" :data='{"path":"/book/:id","example":"/freexcomic/book/90","parameters":{"id":"漫画id，漫画主页的地址栏中"},"radar":[{"source":["www.jjmhw.cc/book/:id"]}],"name":"漫画更新","maintainers":["junfengP"],"url":"www.jjmhw.cc","location":"book.ts"}' :test='{"code":0}' />

## 腾讯网 <Site url="qq.com"/>

### 排行榜 <Site url="qq.com" size="sm" />

<Route namespace="qq" :data='{"path":"/ac/rank/:type?/:time?","categories":["anime"],"example":"/qq/ac/rank","parameters":{"type":"分类，见下表，默认为月票榜","time":"时间，`cur` 为当周、`prev` 为上周"},"features":{"requireConfig":false,"requirePuppeteer":false,"antiCrawler":false,"supportBT":false,"supportPodcast":false,"supportScihub":false},"radar":[{"source":["ac.qq.com/Rank/comicRank/type/:type","ac.qq.com/"]}],"name":"排行榜","maintainers":["nczitzk"],"description":"| 月票榜 | 飙升榜 | 新作榜 | 畅销榜 | TOP100 | 男生榜 | 女生榜 |\n  | ------ | ------ | ------ | ------ | ------ | ------ | ------ |\n  | mt     | rise   | new    | pay    | top    | male   | female |\n\n  :::tip\n  `time` 参数仅在 `type` 参数选为 **月票榜** 的时候生效。\n  :::","location":"ac/rank.ts"}' :test='{"code":0}' />

| 月票榜 | 飙升榜 | 新作榜 | 畅销榜 | TOP100 | 男生榜 | 女生榜 |
  | ------ | ------ | ------ | ------ | ------ | ------ | ------ |
  | mt     | rise   | new    | pay    | top    | male   | female |

  :::tip
  `time` 参数仅在 `type` 参数选为 **月票榜** 的时候生效。
  :::

## 天使动漫论坛 <Site url="www.tsdm39.com"/>

### BD <Site url="www.tsdm39.com" size="sm" />

<Route namespace="tsdm39" :data='{"path":"/bd/:type?","name":"BD","categories":["anime"],"maintainers":["equt"],"example":"/tsdm39/bd","parameters":{"type":"BD type, checkout the table below for details"},"features":{"requireConfig":[{"name":"TSDM39_COOKIES","optional":false,"description":"天使动漫论坛登陆后的 cookie 值，可在浏览器控制台通过 `document.cookie` 获取。"}],"requirePuppeteer":false,"antiCrawler":false,"supportBT":false,"supportPodcast":false,"supportScihub":false},"description":"| 720P | 1080P | BDMV | 4K | AV1 |\n| :--: | :--: | :--: | :--: | :--: |\n| 403 | 404 | 405 | 4130 | 5815 |","location":"bd.ts"}' :test='undefined' />

| 720P | 1080P | BDMV | 4K | AV1 |
| :--: | :--: | :--: | :--: | :--: |
| 403 | 404 | 405 | 4130 | 5815 |

## 月幕 Galgame <Site url="ymgal.games"/>

### 本月新作 <Site url="ymgal.games/" size="sm" />

<Route namespace="ymgal" :data='{"path":"/game/release","categories":["anime"],"example":"/ymgal/game/release","parameters":{},"features":{"requireConfig":false,"requirePuppeteer":false,"antiCrawler":false,"supportBT":false,"supportPodcast":false,"supportScihub":false},"radar":[{"source":["ymgal.games/"]}],"name":"本月新作","maintainers":["SunBK201"],"url":"ymgal.games/","location":"game.ts"}' :test='{"code":0}' />

### 文章 <Site url="ymgal.games" size="sm" />

<Route namespace="ymgal" :data='{"path":"/article/:type?","categories":["anime"],"example":"/ymgal/article","parameters":{"type":"文章类型"},"features":{"requireConfig":false,"requirePuppeteer":false,"antiCrawler":false,"supportBT":false,"supportPodcast":false,"supportScihub":false},"name":"文章","maintainers":["SunBK201"],"description":"| 全部文章 | 资讯 | 专栏   |\n  | -------- | ---- | ------ |\n  | all      | news | column |","location":"article.ts"}' :test='{"code":0}' />

| 全部文章 | 资讯 | 专栏   |
  | -------- | ---- | ------ |
  | all      | news | column |

## アニメ新番組 <Site url="bangumi.moe"/>

### Unknown <Site url="bangumi.moe/" size="sm" />

<Route namespace="bangumi" :data='{"path":"/moe/*","radar":[{"source":["bangumi.moe/"],"target":"/moe"}],"name":"Unknown","maintainers":[],"url":"bangumi.moe/","location":"moe/index.ts"}' :test='undefined' />

### 成员关注榜 <Site url="bangumi.moe" size="sm" />

<Route namespace="bangumi" :data='{"path":"/:type/followrank","categories":["anime"],"example":"/bangumi/anime/followrank","parameters":{"type":"类型：anime - 动画, book - 图书, music - 音乐, game - 游戏, real - 三次元"},"features":{"requireConfig":false,"requirePuppeteer":false,"antiCrawler":false,"supportBT":false,"supportPodcast":false,"supportScihub":false},"radar":[{"source":["bgm.tv/:type"],"target":"/:type/followrank"}],"name":"成员关注榜","maintainers":["honue","zhoukuncheng"],"location":"tv/other/followrank.ts"}' :test='{"code":0}' />

### 當季新番 <Site url="bangumi.online/" size="sm" />

<Route namespace="bangumi" :data='{"path":"/online","categories":["anime"],"example":"/bangumi/online","parameters":{},"features":{"requireConfig":false,"requirePuppeteer":false,"antiCrawler":true,"supportBT":false,"supportPodcast":false,"supportScihub":false},"radar":[{"source":["bangumi.online/"]}],"name":"當季新番","maintainers":["devinmugen"],"url":"bangumi.online/","location":"online/online.ts"}' :test='{"code":1,"message":"AssertionError: expected 503 to be 200 // Object.is equality\n    at /home/runner/work/RSSHub/RSSHub/lib/routes.test.ts:79:41\n    at processTicksAndRejections (node:internal/process/task_queues:95:5)\n    at runTest (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/@vitest+runner@2.0.4/node_modules/@vitest/runner/dist/index.js:955:11)\n    at async Promise.all (index 86)\n    at runSuite (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/@vitest+runner@2.0.4/node_modules/@vitest/runner/dist/index.js:1097:13)\n    at runSuite (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/@vitest+runner@2.0.4/node_modules/@vitest/runner/dist/index.js:1111:15)\n    at runFiles (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/@vitest+runner@2.0.4/node_modules/@vitest/runner/dist/index.js:1168:5)\n    at startTests (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/@vitest+runner@2.0.4/node_modules/@vitest/runner/dist/index.js:1177:3)\n    at file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/vitest@2.0.4_@types+node@20.14.12_jsdom@24.1.1_bufferutil@4.0.8_utf-8-validate@5.0.10_/node_modules/vitest/dist/chunks/runtime-runBaseTests.Dq_sJZq9.js:132:11\n    at withEnv (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/vitest@2.0.4_@types+node@20.14.12_jsdom@24.1.1_bufferutil@4.0.8_utf-8-validate@5.0.10_/node_modules/vitest/dist/chunks/runtime-runBaseTests.Dq_sJZq9.js:94:5)\n    at run (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/vitest@2.0.4_@types+node@20.14.12_jsdom@24.1.1_bufferutil@4.0.8_utf-8-validate@5.0.10_/node_modules/vitest/dist/chunks/runtime-runBaseTests.Dq_sJZq9.js:117:3)\n    at runBaseTests (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/vitest@2.0.4_@types+node@20.14.12_jsdom@24.1.1_bufferutil@4.0.8_utf-8-validate@5.0.10_/node_modules/vitest/dist/vendor/base.Csk7BT3h.js:31:3)\n    at ForksBaseWorker.executeTests (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/vitest@2.0.4_@types+node@20.14.12_jsdom@24.1.1_bufferutil@4.0.8_utf-8-validate@5.0.10_/node_modules/vitest/dist/workers/forks.js:25:7)\n    at execute (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/vitest@2.0.4_@types+node@20.14.12_jsdom@24.1.1_bufferutil@4.0.8_utf-8-validate@5.0.10_/node_modules/vitest/dist/worker.js:116:5)\n    at onMessage (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/tinypool@1.0.0/node_modules/tinypool/dist/entry/process.js:54:20)"}' />

### 放送列表 <Site url="bgm.tv/calendar" size="sm" />

<Route namespace="bangumi" :data='{"path":"/tv/calendar/today","categories":["anime"],"example":"/bangumi/tv/calendar/today","parameters":{},"features":{"requireConfig":false,"requirePuppeteer":false,"antiCrawler":false,"supportBT":false,"supportPodcast":false,"supportScihub":false},"radar":[{"source":["bgm.tv/calendar"]}],"name":"放送列表","maintainers":["magic-akari"],"url":"bgm.tv/calendar","location":"tv/calendar/today.ts"}' :test='{"code":0}' />

### 条目的通用路由格式 <Site url="bangumi.moe" size="sm" />

<Route namespace="bangumi" :data='{"path":"/tv/subject/:id/:type?/:showOriginalName?","categories":["anime"],"example":"/bangumi/tv/subject/328609/ep/true","parameters":{"id":"条目 id, 在条目页面的地址栏查看","type":"条目类型，可选值为 `ep`, `comments`, `blogs`, `topics`，默认为 `ep`","showOriginalName":"显示番剧标题原名，可选值 0/1/false/true，默认为 false"},"features":{"requireConfig":false,"requirePuppeteer":false,"antiCrawler":false,"supportBT":false,"supportPodcast":false,"supportScihub":false},"radar":[{"source":["bgm.tv/subject/:id"],"target":"/tv/subject/:id"}],"name":"条目的通用路由格式","maintainers":["JimenezLi"],"description":":::warning\n  此通用路由仅用于对路由参数的描述，具体信息请查看下方与条目相关的路由\n  :::","location":"tv/subject/index.ts"}' :test='{"code":0}' />

:::warning
  此通用路由仅用于对路由参数的描述，具体信息请查看下方与条目相关的路由
  :::

### 现实人物的新作品 <Site url="bangumi.moe" size="sm" />

<Route namespace="bangumi" :data='{"path":"/tv/person/:id","categories":["anime"],"example":"/bangumi/tv/person/32943","parameters":{"id":"人物 id, 在人物页面的地址栏查看"},"features":{"requireConfig":false,"requirePuppeteer":false,"antiCrawler":false,"supportBT":false,"supportPodcast":false,"supportScihub":false},"radar":[{"source":["bgm.tv/person/:id"]}],"name":"现实人物的新作品","maintainers":["ylc395"],"location":"tv/person/index.ts"}' :test='{"code":0}' />

### 小组话题的新回复 <Site url="bangumi.moe" size="sm" />

<Route namespace="bangumi" :data='{"path":"/tv/topic/:id","categories":["anime"],"example":"/bangumi/tv/topic/367032","parameters":{"id":"话题 id, 在话题页面地址栏查看"},"features":{"requireConfig":false,"requirePuppeteer":false,"antiCrawler":false,"supportBT":false,"supportPodcast":false,"supportScihub":false},"radar":[{"source":["bgm.tv/group/topic/:id"]}],"name":"小组话题的新回复","maintainers":["ylc395"],"location":"tv/group/reply.ts"}' :test='{"code":0}' />

### 小组话题 <Site url="bangumi.moe" size="sm" />

<Route namespace="bangumi" :data='{"path":"/tv/group/:id","categories":["anime"],"example":"/bangumi/tv/group/boring","parameters":{"id":"小组 id, 在小组页面地址栏查看"},"features":{"requireConfig":false,"requirePuppeteer":false,"antiCrawler":false,"supportBT":false,"supportPodcast":false,"supportScihub":false},"radar":[{"source":["bgm.tv/group/:id"]}],"name":"小组话题","maintainers":["SettingDust"],"location":"tv/group/topic.ts"}' :test='{"code":0}' />

### 用户日志 <Site url="bangumi.moe" size="sm" />

<Route namespace="bangumi" :data='{"path":"/tv/user/blog/:id","categories":["anime"],"example":"/bangumi/tv/user/blog/sai","parameters":{"id":"用户 id, 在用户页面地址栏查看"},"features":{"requireConfig":false,"requirePuppeteer":false,"antiCrawler":false,"supportBT":false,"supportPodcast":false,"supportScihub":false},"radar":[{"source":["bgm.tv/user/:id"]}],"name":"用户日志","maintainers":["nczitzk"],"location":"tv/user/blog.ts"}' :test='{"code":1,"message":"AssertionError: expected 333244690626 to be less than 311040000000\n    at checkDate (/home/runner/work/RSSHub/RSSHub/lib/routes.test.ts:36:46)\n    at checkRSS (/home/runner/work/RSSHub/RSSHub/lib/routes.test.ts:61:13)\n    at processTicksAndRejections (node:internal/process/task_queues:95:5)\n    at /home/runner/work/RSSHub/RSSHub/lib/routes.test.ts:80:17\n    at runTest (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/@vitest+runner@2.0.4/node_modules/@vitest/runner/dist/index.js:955:11)\n    at async Promise.all (index 93)\n    at runSuite (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/@vitest+runner@2.0.4/node_modules/@vitest/runner/dist/index.js:1097:13)\n    at runSuite (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/@vitest+runner@2.0.4/node_modules/@vitest/runner/dist/index.js:1111:15)\n    at runFiles (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/@vitest+runner@2.0.4/node_modules/@vitest/runner/dist/index.js:1168:5)\n    at startTests (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/@vitest+runner@2.0.4/node_modules/@vitest/runner/dist/index.js:1177:3)\n    at file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/vitest@2.0.4_@types+node@20.14.12_jsdom@24.1.1_bufferutil@4.0.8_utf-8-validate@5.0.10_/node_modules/vitest/dist/chunks/runtime-runBaseTests.Dq_sJZq9.js:132:11\n    at withEnv (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/vitest@2.0.4_@types+node@20.14.12_jsdom@24.1.1_bufferutil@4.0.8_utf-8-validate@5.0.10_/node_modules/vitest/dist/chunks/runtime-runBaseTests.Dq_sJZq9.js:94:5)\n    at run (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/vitest@2.0.4_@types+node@20.14.12_jsdom@24.1.1_bufferutil@4.0.8_utf-8-validate@5.0.10_/node_modules/vitest/dist/chunks/runtime-runBaseTests.Dq_sJZq9.js:117:3)\n    at runBaseTests (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/vitest@2.0.4_@types+node@20.14.12_jsdom@24.1.1_bufferutil@4.0.8_utf-8-validate@5.0.10_/node_modules/vitest/dist/vendor/base.Csk7BT3h.js:31:3)\n    at ForksBaseWorker.executeTests (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/vitest@2.0.4_@types+node@20.14.12_jsdom@24.1.1_bufferutil@4.0.8_utf-8-validate@5.0.10_/node_modules/vitest/dist/workers/forks.js:25:7)\n    at execute (file:///home/runner/work/RSSHub/RSSHub/node_modules/.pnpm/vitest@2.0.4_@types+node@20.14.12_jsdom@24.1.1_bufferutil@4.0.8_utf-8-validate@5.0.10_/node_modules/vitest/dist/worker.js:116:5)"}' />

### 用户想看 <Site url="bangumi.moe" size="sm" />

<Route namespace="bangumi" :data='{"path":"/tv/user/wish/:id","categories":["anime"],"example":"/bangumi/tv/user/wish/sai","parameters":{"id":"用户 id, 在用户页面地址栏查看"},"features":{"requireConfig":false,"requirePuppeteer":false,"antiCrawler":false,"supportBT":false,"supportPodcast":false,"supportScihub":false},"radar":[{"source":["bgm.tv/anime/list/:id/wish"]}],"name":"用户想看","maintainers":["honue"],"location":"tv/user/wish.ts"}' :test='{"code":0}' />

