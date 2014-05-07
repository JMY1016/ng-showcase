Angular范例集
============
这是一个基于angular的界面元素范例程序，基于bootstrap 3框架，优先使用内置指令来完成。
其目标是做一个类似smartclient等控件包的showcase程序，展示angular的能力，同时作为精简的备查字典。

当前进展：刚刚开始

注意：

1. clone下去之后，请先确保有node环境，然后执行npm install和bower install命令，以便对grunt环境进行初始化。
之后就可以用grunt serve来启动服务器进行查看和调试了。
2. 如果使用windows系统，请用下列命令配置git： git config core.autocrlf input 我们统一使用unix的行结尾风格提交。

稍后会将它编译并发布到公网上。

总体原则
------------

1. 参照smartclient的demo实现
2. 优先使用内置指令实现，除非能证明有显著优势，否则不要封装自定义指令
3. 候选方案顺序 内置指令 > filter > service > 自定义指令
4. 任何会修改数据的操作均通过ng-model完成
5. css框架统一使用bootstrap 3
6. 复杂的控件尽量用封装适当的jquery控件或bootstrap控件的方式进行，但是不要依赖jquery-ui

组织方式
------------

1. 通过assign的方式主动认领任务

分工
------------

1. 构建基于github的CI环境，并支持自动发布
2. 开发一个界面框架，能让访客体验操作并现场查看源码，仿smartclient的demo
3. 所有人均可报名参加用户化测试
4. 产品组负责把关filter/directive等界面元素的描述性，并纠正命名不当等问题
5. 多语言组负责开发多语言界面

目标
------------

1. 基本输入指令
2. grid
3. treegrid
4. 校验指令
5. 对话框
