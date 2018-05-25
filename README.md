## Build Setup

``` bash
# install dependencies
npm install

# serve with hot reload at localhost:8080
npm run dev

# build for production with minification
npm run build

```

## 参考指南
[VUE与TypeScript集成配置最简教程](https://blog.csdn.net/u014633852/article/details/73706459)

## 使用问题总结
### vue文件的引入
引入Vue文件的时候需要加上.vue后缀,否则编辑器识别不到

### 报错：使用Typescript开发编译
``` bash
// 使用Typescript开发Vue，一切准备就绪。但npm run dev时，提示

ERROR in ./src/main.ts
Module build failed: TypeError: Cannot read property 'afterCompile' of undefined错误。

// 解决方法
将ts-loader从4.0降低到3.1.1解决问题。是由于webpack和ts-loader版本不兼容造成的。
npm install ts-loader@3.1.1 --save-dev
```
