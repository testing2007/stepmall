[TOC]

#### 原型参考

地址：https://www.axureshop.com/a/1107151.html

* 账号：13**3 或通过 微信 登录
* 密码：K~4

#### 自动代码

- 官方社区：[renren.io](http://www.renren.io/)

- 代码地址：

  * 后端地址：https://gitee.com/renrenio/renren-fast

  - 前端地址：https://gitee.com/renrenio/renren-fast-vue
  - 代码生成器：https://gitee.com/renrenio/renren-generator

##### 后端代码

idea2022 pom.xml 需要修改：

```xml
<lombok.version>1.18.22</lombok.version>
```

##### 前段代码

* ESLint设置（.eslintrc.js文件）

```js
// https://eslint.org/docs/user-guide/configuring

module.exports = {
  root: true,
  parser: 'babel-eslint',
  parserOptions: {
    sourceType: 'module'
  },
  env: {
    browser: true,
  },
  // https://github.com/standard/standard/blob/master/docs/RULES-en.md
  extends: 'standard',
  // required to lint *.vue files
  plugins: [
    'html'
  ],
  // add your custom rules here
  rules: {
    "space-before-function-paren": 'off',
    // allow async-await
    'generator-star-spacing': 'off',
    // allow debugger during development
    'no-debugger': process.env.NODE_ENV === 'production' ? 'error' : 'off'
  }
}


```





#### 代码框架

https://github.com/PanJiaChen/vue-element-admin/tree/v4.0.0

```bash
# clone the project
git clone https://github.com/PanJiaChen/vue-element-admin.git

# enter the project directory
cd vue-element-admin

# install dependency
npm install

# develop
npm run dev
```

问题（npm install 错误 fatal: ）：

https://github.com/PanJiaChen/vue-element-admin/issues/3945

参考文章（/s r c/views/documentation/index.vue）：

​      articleList: [

​        { title: '基础篇', href: 'https://juejin.im/post/59097cd7a22b9d0065fb61d2' },

​        { title: '登录权限篇', href: 'https://juejin.im/post/591aa14f570c35006961acac' },

​        { title: '实战篇', href: 'https://juejin.im/post/593121aa0ce4630057f70d35' },

​        { title: 'vue-admin-template 篇', href: 'https://juejin.im/post/595b4d776fb9a06bbe7dba56' },

​        { title: 'v4.0 篇', href: 'https://juejin.im/post/5c92ff94f265da6128275a85' },

​        { title: '自行封装 component', href: 'https://segmentfault.com/a/1190000009090836' },

​        { title: '优雅的使用 icon', href: 'https://juejin.im/post/59bb864b5188257e7a427c09' },

​        { title: 'webpack4（上）', href: 'https://juejin.im/post/59bb864b5188257e7a427c09' },

​        { title: 'webpack4（下）', href: 'https://juejin.im/post/5b5d6d6f6fb9a04fea58aabc' }

​      ]