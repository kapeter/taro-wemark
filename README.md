# 微信小程序markdown渲染库-Taro框架适配版本

## 原版链接

GitHub地址：[https://github.com/TooBug/wemark](https://github.com/TooBug/wemark)

## 使用方法

#### 1、将src目录复制到自己的项目中，目录更名为taro-wemark。

#### 2、在页面中使用

    // 引入组件
    import Taro, { Component } from '@tarojs/taro'
    import TaroWemark from '../../components/taro-wemark/taro-wemark'

    export default class Index extends Component{

        constructor() {
            super();
            this.state = {
                content: '## hello, world'
            };

        }

        render () {
            return (
                // md为markdown内容
                <TaroWemark md={this.state.content}></TaroWemark> 
            )
        }
    }

## 感谢

[感谢原作者TooBug](https://github.com/TooBug)

## LICENSE
MIT
