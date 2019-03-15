# 瀑布流demo
## 预览地址： https://therest0.github.io/waterfull
## 懒加载原理
页面中的img元素，如果没有src属性，浏览器就不会发出请求去下载图片，真正的路径存在元素的“data-url”属性里，要用的时候就取出来，再设置一旦通过javascript设置了图片路径，浏览器才会送请求。
## 瀑布流原理
通过计算出一排能够容纳几列元素，然后寻找各列之中所有元素高度之和的最小者，并将新的元素添加到该列上，然后继续寻找所有列的各元素之和的最小者，继续添加至该列上，如此循环下去，直至所有元素均能够按要求排列为止；
## 实现原理
通过ajax获取到图片等数据，再拼接字符串渲染到页面上，ajax获取的图片先放到data-src中
