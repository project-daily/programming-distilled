# Webpack

## Loaders

### 脚本

### 样式

#### css-loader

[css-loader](https://github.com/webpack-contrib/css-loader) 用于拦截并处理 CSS 中的各种加载语法，比如 `@import` 和 `url()`。推荐与 `style-loader` 配合使用。

示例：

```js
module: {
  rules: [
    {
      test: /\.css$/,
      use: [
        'style-loader',
        'css-loader'
      ]
    }
  ]
}
```

#### style-loader

[style-loader](https://github.com/webpack-contrib/style-loader) 用于在 DOM 中注入 &lt;style> 标签来添加 CSS。推荐与 `css-loader` 配合使用。

示例：

```js
module: {
  rules: [
    {
      test: /\.css$/,
      use: [
        'style-loader',
        'css-loader'
      ]
    }
  ]
}
```

#### postcss-loader

[postcss-loader](https://github.com/postcss/postcss-loader) 使用 [PostCSS](https://postcss.org/) 来处理 CSS。推荐与 `css-loader` 配合使用。

示例：

```js
module: {
  rules: [
    {
      test: /\.css$/,
      use: [
        'style-loader',
        'css-loader',
        'postcss-loader'
      ]
    }
  ]
}
```
