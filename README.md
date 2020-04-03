# hexo-theme-arknights

明日方舟的 Hexo 主题
开发中……

## 搭建开发环境

先装好 [nodejs](https://nodejs.org/) 和 [yarn](https://classic.yarnpkg.com/zh-Hans/) ，然后执行以下命令：
```bash
yarn global add hexo-cli yo generator-hexo-theme
hexo init <test>
cd <test>
yarn add hexo-server hexo-browsersync hexo-renderer-pug hexo-renderer-sass hexo-renderer-ts
cd <test>/themes
git clone https://github.com/Yue-plus/hexo-theme-arknights.git arknights
```
修改 `<test>/_config.yml` 中的 `theme:` 改为 `arknights`
然后,打开 `<test>/themes/arknights` 下编辑主题
```bash
hexo serve --debug
```
一个bug，修改 `.pug` 模板文件无法自动刷新页面。
解决方法：到 Hexo 目录下的
`./node_modules/hexo-renderer-pug/lib/pug.js`
中的
`pugRenderer.compile = pugCompile;`
注释掉。


### 点个 star 把~
给颗小星星吧 `(/▽＼)`