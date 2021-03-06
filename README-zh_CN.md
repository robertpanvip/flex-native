# flex-native
 [English](./README.md)|简体中文 
### 🔗 内容列表
- [背景](#背景)
- [环境支持](#-环境支持)
- [安装](#-安装)
- [使用](#-使用)
- [贡献者](#-贡献者)

### 背景
- 由于之前写项目大多都使用flex布局 ，到了一家新公司后开始做ie9的兼容、而flex布局又只支持ie10+，在ie9中实现一个居中布局就不是那么方便、虽然也能用其他布局实现、但是不是这么熟练、开发效率减少了不少、
- 在网上找了不少关于在ie9中使用flex布局的库，几乎都不理想就想着自己实现一个支持flexbox布局的库


### 🖥 环境支持
 - 现代浏览器和 ie9+

| [<img src="https://raw.githubusercontent.com/alrra/browser-logos/master/src/edge/edge_48x48.png" alt="IE / Edge" width="24px" height="24px" />](http://godban.github.io/browsers-support-badges/)<br>IE / Edge | [<img src="https://raw.githubusercontent.com/alrra/browser-logos/master/src/firefox/firefox_48x48.png" alt="Firefox" width="24px" height="24px" />](http://godban.github.io/browsers-support-badges/)<br>Firefox | [<img src="https://raw.githubusercontent.com/alrra/browser-logos/master/src/chrome/chrome_48x48.png" alt="Chrome" width="24px" height="24px" />](http://godban.github.io/browsers-support-badges/)<br>Chrome | [<img src="https://raw.githubusercontent.com/alrra/browser-logos/master/src/safari/safari_48x48.png" alt="Safari" width="24px" height="24px" />](http://godban.github.io/browsers-support-badges/)<br>Safari |
| --- | --- | --- | --- |
| IE9+, Edge | 3.5+ | all | all |

 由于使用了transform 属性去计算位置 所以只要是支持transform属性的浏览器都支持
### 📦 安装
```bash
npm install flex-native
```
### 🔨 使用
- 在普通的HTML中使用
```javascript
<script src='https://unpkg.com/flex-native@latest'>
```
- 在模块化中使用
```javascript
import('flex-native');
```
   使用时请在CSS中的任何`display: flex`声明之前添加一个 `-js-display: flex`声明，
或在构建过程中使用[PostCSS Flexibility](https://github.com/7rulnik/postcss-flexibility)自动添加-js前缀。
- Css中
	<br>
	.wrapper{     
		-js-display:flex;<br>
        display:flex;<br>
		align-items:center;<br>
		justify-content:center;<br>
		}
		
- 元素上
       <br>
        &lt;div style='display:flex;align-items:center' /&gt;
       <br>
	
总的来说和普通写css没有区别

### 🤝 贡献者
[@robertpanvip](https://github.com/robertpanvip)
<br>
[@1844877065](https://github.com/1844877065)
