两个重要的组成部分：视图，脚本
el：id选择器
data：保存数据，赋值
生命周期：页面初始化前后，挂载前后各种灵活的函数都有相应的API调用，官网上有
模板语法 -插值：支持JS表达式（算数运算）  三元表达式（比较结果为真执行？后面代码，比较失败执行：后面代码），Html标签拼接，函数（.split()）
模板语法 -指令：v-if（条件显示） v-bind:href="url" 跳转  @click点击事件
Class 与 Style 绑定：动态显示样式
条件渲染：v-if 赋值是什么就显示什么
列表渲染：v-for 指令需要使用 item in items 形式的特殊语法，其中 items 是源数据数组，而 item 则是被迭代的数组元素的别名。
事件绑定: v-on 可以用 v-on 指令监听 DOM 事件，并在触发时运行一些 JavaScript 代码,提供了很多事件修饰符官网有  v-on可以绑定所有HTML事件（dblclike，双击事件）

表单输入绑定：可以用 v-model 指令在表单 <input>、<textarea> 及 <select> 元素上创建双向数据绑定。它会根据控件类型自动选取正确的方法来更新元素。尽管有些神奇，但 v-model 本质上不过是语法糖。它负责监听用户的输入事件以更新数据，并对一些极端场景进行一些特殊处理。
v-model 会忽略所有表单元素的 value、checked、selected attribute 的初始值而总是将 Vue 实例的数据作为数据来源。你应该通过 JavaScript 在组件的 data 选项中声明初始值。v-model 在内部为不同的输入元素使用不同的属性并抛出不同的事件：

text 和 textarea 元素使用 value 属性和 input 事件；
checkbox 和 radio 使用 checked 属性和 change 事件；
select 字段将 value 作为 prop 并将 change 作为事件。


组件基础：Vue.component组件注册  组件是可复用的 Vue 实例，且带有一个名字：在这个例子中是 <button-counter>。我们可以在一个通过 new Vue 创建的 Vue 根实例中，

组件注册 ：一般组件可以全局注册也可以局部注册  components 
new Vue({
  el: '#app',
  components: {
    'component-a': ComponentA,
    'component-b': ComponentB
  }
})

单文件组件：全局定义 (Global definitions) 强制要求每个 component 中的命名不得重复
字符串模板 (String templates) 缺乏语法高亮，在 HTML 有多行的时候，需要用到丑陋的 \
不支持 CSS (No CSS support) 意味着当 HTML 和 JavaScript 组件化时，CSS 明显被遗漏
没有构建步骤 (No build step) 限制只能使用 HTML 和 ES5 JavaScript, 而不能使用预处理器，如 Pug (formerly Jade) 和 Babel
