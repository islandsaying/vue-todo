# vue-todo
### step1 完成两个练习
1. 练习一
- 在send方法中判断: 无值提示输入内容,有值才发送成功
- 核心代码`!this.count`
2. 练习二
- 使用v-if来决定元素是否被渲染
- 核心代码`v-if="count"`
### 编辑todo
1. 双击当前的todo进行编辑
2. 创建一个对象,为其添加属性暂存编辑前todo状态,用户如果取消编辑,则返回之前状态
3. 根据初始值editedTodo是否为null来判断是否在编辑状态
4. 不要this.editedTodo = todo简单的进行复制,这样复制了引用地址,任何对todo的修改都会反应出来,所以创建新对象
5. 解决双击后所有编辑框都弹出的问题
6. 双向绑定输入框和todo的title
7. 绑定enter实现编辑完成,并自动隐藏编辑框
8. 绑定esc键位实现取消后还原为todo编辑前的状态,并自动隐藏编辑框
9. 用户回车后判断:如果没有内容,则删除这条todo
10. 自定义指令实现自动聚焦directives
11. 全部标记为已完成使用map遍历改变completed
12. 计算未完成的todo个数,使用filter筛选
### 筛选功能
1. 增加一个data属性--intention,来记录用户的意图(包括三种:all,ongoing,completed)
### 批量清除功能