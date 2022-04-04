## PartAnimator 
PartAnimator 是一个 '极简' 且 '灵活' 的 CSS 过渡动画库，可快速复用于各种 **前端** 项目中。使用前只需要引入 CSS 文件。然后开始调用你想要的的类样式 ~ ，除了使用原生写法，还可以通过开发框架来调用。

当前总动画数为：**``41``** ，对于不同的样式类也可混合搭配使用。

### 快速上手
---
通过 link 引入 css
```
<link rel="stylesheet" href="https://partanimator.glumi.cn/PartAnimator.css">
```
或者 npm 安装
```
npm install part-animator
import 'part-animator/Part-Animator.css'
```

### 原生写法
---
```html
<body>
    <div class="part-enter-1">过度内容</div>
</body>

<style>
    body {
        display: flex;
        justify-content: center;
        align-items: center;
    }
</style>
```

### Vue.js
---
```vue
<template>
<div id="anim">
    <button @click="show=!show">显示/隐藏</button>
    <transition enter-active-class="part-enter-1" leave-active-class="part-leave-1">
    <h1 v-if="show">过渡内容</h1>
    </transition>
</div>
</template>

<script>
import css from 'part-animator/PartAnimator.css'
export default {
    data() {
        return {
            show: false
        }
    }
}
</script>

<style scoped>
    #anim {
        display: flex;
        justify-content: center;
        align-items: center;
    }
</style>
```
