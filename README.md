# Front-end-specification
  前端规范 Front end specification
所有有交互的加
```
cursor：pointer/text
```

## product 多环境配置推荐后台配置

## ip替代localhost 方便测试和UI实时查看

## ui库按需引入
如果以后遇到想用iview里面某一个组件，但是又发现这个组件（本身封装的问题）不能完全满足我们需求，可以去de_modules/iview/dist/components/的组件复制粘贴到项目目录下 c/components/_iviewc/components/下，就可以直接改他的源码了，使用的时候记得要
例如：
```
import Tabs from '@/components/_iview/components/tabs/index'

components: {
    Tabs
} 
```

## html里面尽量不要写逻辑

## proxy服务器统一
```
/mock/xxx
/local-weijia/xxx
/local-aixuan/xxx
/dev/xxx
/test/xxx
/product/xxx
```
## axios 封装 fetch

## 全局拦截处理：
## 增删改的msg提示，get的接口不用做处理
## loading

## 映射表：

## this.fetch.module['a']

## 静态data 提取到外面

## 建立公共库： css/js/功能组件

## 逻辑容错处理：&& if

## 命名规范：
	文件命名：
	class：
	function：

## 注释规范

## 百分比布局：

## html：
 标签嵌套规范

## css：
减少自带后代选择器使用
css属性顺序
z-index层级

## js：
多使用es6，7语法

## css预编译语言：
## sass
## stylus

## git工具使用规范：

## 开发环境多端查看：

## 静态页面缓存处理：
```
export default {
  name字段
  methods: {

    handle // 处理时间33
    get // 获取数据
  }
```
## destroyed的使用，例如营收分析页面图表自适应用到window.onresize要销毁

## mixins使用



## vuex使用规范：


## console.log调试完及时删掉

## 编辑器/插件/快捷键

## git命令


==================================================================
## mpvue
1.不支持自定义组件上添加v-show
2.不支持slot
3.data值或methods命名不能过长（30以内）
4.ui放在static内，每个页面用到就在对应main.json里写：
```
	{
  		"usingComponents": {
    			"i-icon": "../../../../static/iview-weapp/dist/icon/index",
    			"i-message": "../../../../static/iview-weapp/dist/message/index"
  		}
	}
```
5.app.json里面配置window：{导航条，标题，下拉刷新。。。}，networkTimeout：{配置超时时间}

==================================================================
## stylus-loader 难配置，无法使用~@引入静态资源

sass：
```
npm install node-sass sass-loader --save
```
直接下载就可以使用了
集成了redux/saga和css module，上手起来较快些











==================================================================
## yarn：
```
yarn global bin
yarn config get registry
yarn config set registry https://registry.npm.taobao.org
```
