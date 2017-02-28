# CSS Flags

CSS3 实现各国国旗

##预览

![flags](https://cloud.githubusercontent.com/assets/22977253/23391962/98b456b8-fdb3-11e6-962a-e3c861ba6b53.png)


## 动力

提高CSS3的使用能力，同时得到[singlediv](http://a.singlediv.com/)和[one-div](http://one-div.com/)的启发，在此感谢。


## 已完成

- [x] 部分国家（中国等）


## 计划

- [ ] 剩余国家

##资源

国旗参考:[flagpeida](http://flagpedia.net/),感谢!

##贡献

规则:

>尽量一个div元素完成国旗的绘制

代码格式:

HTML:

    <div class="flags-content">
        <h3>China</h3>
        <div class="country china"></div>
    </div>
    
CSS代码:

    .country{
        box-sizing: border-box;
        width: 600px;
        height: 400px;
        position: relative;
        border:1px solid #ccc;
    }
    
    /*china*/
    
    .china{
        background:#CE1126;
    }
    .china:before,.china:after{
        content: "★";
        position: absolute;
        color:#FCD116;
    }
    .china:before{
        font-size: 90px;
        top: 60px;
        left: 50px;
    }
    .china:after{
        left: 160px;
        top: 30px;
        font-size: 33px;
        text-shadow:#FCD116 40px 50px 0,#FCD116 40px 100px 0,#FCD116 0 150px 0 ;
    }

在线预览: https://codepen.io/wakawei/pen/yMYOaE
