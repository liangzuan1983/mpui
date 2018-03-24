# WeUI for mpvue

> WeUI-mpvue 是一套基于 WeUI 开发的 mpvue 组件库，增加了一些新的特性和样式。

## 说明

组件库尽量以 Vue 组件形式实现，部分组件因 mpvue 尚不支持的语法而无法实现，详细见[不支持列表](http://mpvue.com/mpvue/#_14)。

## 安装

```bash
$ yarn add weui-mpvue
```

## 预览

```bash
$ git clone https://github.com/kankungyip/weui-mpvue
$ cd weui-mpvue
$ yarn example
```

用[微信web开发者工具](https://mp.weixin.qq.com/debug/wxadoc/dev/devtools/download.html)打开`weui-mpvue`项目目录。

## 使用
### 引入全局样式

```vue
<style lang="less">
@import "<project_dir>/node_modules/weui-mpvue/theme/weui";
</style>
```

### 使用组件

```vue
<template>
  <ui-button text="按钮" />
</template>

<script>
import uiButton 'weui-mpvue/components/button'

export default {
  components: {
    uiBUtton
  }
}
</script>
```

## 组件
### WeUI 重构状态
#### 表单

- [x] `Button`（_未完全组件化_：`.weui-btn-area`）
- [ ] `Input`
- [x] `List`（_未完全组件化_：`.weui-cells`、`.weui-cells__title`、`.weui-cells_after-title`）
- [x] `Slider`
- [ ] `Uploader`

#### 基础组件

- [ ] `Article`
- [ ] `Badge`
- [x] `Flex`（_未组件化_）
- [x] `Footer`
- [x] `Gallery`
- [x] `Grid`
- [x] `Icons`
- [x] `Loadmore`
- [ ] `Panel`
- [x] `Preview`
- [x] `Progress`

#### 操作反馈

- [x] `ActionSheet`
- [x] `Dialog`
- [x] `Msg`
- [x] `Picker`
- [x] `Toast`

#### 导航相关

- [ ] `Navbar`
- [x] `Tabbar`

#### 搜索相关

- [ ] `SearchBar`

### 组件新特性

- `Button` 添加图标
- `Grid` 自定义列数
- `Icons` 自定义图标，使用 iconfont.cn 图标

### 计划

- `Article` 组件自动解析 markdown 格式
- 添加 `Avatar` 组件
- 添加 `Ellipse` 组件
- 添加 `Tag` 组件
- 添加 `Price` 组件
- 添加 `Counter` 组件
- 添加 `Countdown` 组件
- 添加 `Steps` 组件
- 添加 `NoticeBar` 组件

## License

[The MIT License](http://opensource.org/licenses/MIT)

请自由地享受和参与开源
