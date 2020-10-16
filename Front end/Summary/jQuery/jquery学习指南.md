# jQuery入门使用（结合jQuery离线手册使用）

离线手册方法获取底部 结合百度示例学习更好（本资源主要是让你有目标有方向的学习）

### 	day01

##### 		jQuery课程概述

##### 		jQuery核心

```js
自调用函数: 自己调用自己

(function (形参){
  // 代码
}(实参))

(function(形参){})(实参)

```

​		jQuery中的核心对象: $或者jQuery
​		jQuery中的jQuery函数 是jQuery官方早就给我定义好的
​		既可以作为函数调用
​		也可以作为对象去调用jQuery官方定义好的方法

​		jQuery的核心函数$()
​		你给$()这个方法传入什么样的参数 就会有不同的功能

###### 	jQuery核心对象

​		$.each()



##### 		jQuery选择器

##### 		jQuery操作元素属性

### 	day02

##### 		jQuery操作CSS

​		

```js
$('a').css({
    width:40px;
    height:40px;
});
```

​		

##### 		jQuery获取/设置标签的位置

​		相对于当前页面的位置

```js
 // jQuery对象.offset()  此方法只对可见元素有效
    // 相对于页面左上角的top $('选择器').offset().top;
    // 相对于页面左上角的left $('选择器').offset().left;

    $('button').click(function () {
      console.log($('.inner').offset().left, $('.inner').offset().top)
    })
```

​		相对于父元素左上角的位置

```js
   //  jQuery对象.position()  此方法只对可见元素有效
    // 相对于父元素左上角的top $('选择器').position().top;
    // 相对于父元素左上角的left $('选择器').position().left;

    $('button').click(function () {
      console.log($('.inner').position().left, $('.inner').position().top)
    })

    // 整型: 整数  20 402

    // 浮点型: 小数 20.001 20.1

```

​		卷曲出去的距离

```js
 // 点击按钮 获取div中卷曲的内容的高度
    // 获取匹配元素相对滚动条顶部的偏移。
    // 此方法对可见和隐藏元素均有效。

    // 也可以设置 $('元素').scrollTop(值)

    $('button').click(function () {
      // console.log($('div').scrollTop(), $('div').scrollLeft())
      $('div').scrollTop(300);
    })

```

##### jQuery获取/设置标签的尺寸

获取元素计算后的height和width

```js
  $('button').click(function () {
      // 取得匹配元素当前计算的高度值（px）。
      // 取得第一个匹配元素当前计算的宽度值（px）。
      // 在 jQuery 1.2 以后可以用来获取 window 和 document 的宽
      console.log($('.inner').width(), $('.inner').height())
    })
```

​	包括内边距但不包括边框的宽度

```js
 // 获取匹配元素不包括边框 包括内边距的宽度
    // 返回的对象包含两个整型属性:top和left.为精确计算结果,请在补白 边框 和填充属性上使用像素单位
    $('button').click(function () {
      console.log($('.inner').innerWidth(), $('.inner').innerHeight())
    })
```

​		包括内边距和边框的宽度

```js
  // outerHeight()
  // outerWidth()
 $('button').click(function () {
      console.log($('.inner').outerHeight(), $('.inner').outerWidth())
    })

```



### 	day03

##### 		添加节点

​		把元素添加到某个元素里面(清空里面的内容)

```js
  // 方法1: $('html标签')
    // 方法2: $('元素').html('html标签')

    // 给button添加点击事件
    // $('button').click(function () {
      // 创建一个b标签
      // let b = $('<b>你好</b>');
      // console.log(b);
      // 把b标签写入box这个div中
      // $('div').html(b);


      // 最简单的方法
      // $('div').html('<b>你好</b>')
    // })

```

##### 		把元素插入到元素里面的后面

```js
 // jQuery中
    // 方法1: $('html标签')
    // 方法2: $('元素').html('html标签')
    // 方法3: 插入到元素里面的后面
    // append(content)  父元素.append(子元素)
    // appendTo(content) 子元素.appendTo(父元素)

    // $('button').click(function () {
    //   $('.box').append('<a href="http://www.baidu.com">百度</a>')
    // })
```

##### 		把元素插入到元素里面的前面

```js
 // 父元素.prepend(子元素)
    $('button').click(function () {
      $('.box').prepend('<strong>我在b前面</strong')
    })
    // 子元素.prependTo(父元素)
```

​		把元素插入到某个元素的前面/后面

```js
// 方法5: 插入到某个元素外面的后面/前面
    // 插入到某个元素外面的后面 after
    // 插入到某个元素外面的前面 before
    $('button').click(function () {
      // 添加到box后面
      $('.box').after(`<a href="http://www.baidu.com">百度</a>`)
      // 添加到box前面
      $('.box').before(`<a href="http://www.itcast.cn">传智播客</a>`)
    })
```



##### 		替换节点

```js
 // 点击按钮  把b标签换成 a标签
    $('button').click(function () {
      // 元素.replaceWith(替换元素)
      $('b').replaceWith('<a href="http://www.baidu.com">百度</a>')
    })
```

##### 		删除节点

	$('button').click(function () {
	  //  元素.remove() 删除自己 逐个的删除
	  // $('b').remove();
	  // 父元素.empty() // 清空父元素中的所有子元素
	  // $('.box').empty();
	})
##### 		复制节点

```js
 $('button').click(function () {
      //  某个元素的其他兄弟元素
      // console.log($('b').siblings())

      $('.box').append($('b').clone(true))
```



##### 		查找节点

​		所有子元素 某个子元素

```js
   // children() 获取某个元素的所有子元素

    // 点击按钮  把b标签换成 a标签
    $('button').click(function () {
      console.log($('.box').children())
    })
```

### 	父节点 祖节点们

```js
  // parent() 某个元素的父元素
    // parents() 某个元素的祖元素

    // 点击按钮  把b标签换成 a标签
    $('button').click(function () {
      console.log($('b').parent());
      console.log($('b').parents());
    })
```

​		前面的兄弟元素 前一个兄弟元素

```js
   $('button').click(function () {
      // 某个元素前面的兄弟元素 一个
      console.log($('span').prev());
      // 某个元素前面的兄弟元素 所有
      console.log($('span').prevAll());
    })
```

### 	后面的兄弟元素 后一个兄弟元素

```js
  $('button').click(function () {
      // 某个元素后面的兄弟元素 一个
      // console.log($('strong').next());
      // // 某个元素后面面的兄弟元素 所有
      // console.log($('strong').nextAll());
    })
```

​		其他兄弟元素

```js
   $('button').click(function () {
      //  某个元素的其他兄弟元素
      // console.log($('b').siblings())
    })
```

​		CSS方法

```js
 // 点击按钮 获取一下box这个div的宽度
    // $('button').click(function () {
    //   console.log($('div').css('width'))
    // })


    // 点击按钮 给box设置一个背景色
    // $('button').click(function () {
    //   $('div').css('backgroundColor', 'red')
    // })


    // 点击按钮 给box设置 背景色 宽度 高度
    // $('button').click(function () {
    //   $('div').css({
    //     'backgroundColor': 'red',
    //     'width': 300,
    //     'height': '300px',
    //     'color': 'green'
    //   })
    // })
```

### day04

##### 		事件处理

###### 		事件的绑定

```js
	元素.on(事件类型,[触发事件的元素],事件处理函数) 可以触发多次
	// $('button').on('click', function () {
    //   console.log(11111);
    // })
	one(事件类型,事件处理函数) 只能触发一次
	// $('button').one('click', function () {
    //   console.log(11111);
    // })
	
```

######    	事件的解绑

  		元素.off(事件的名字,选择器)

```js
  // 首先我给butotn绑定一个click事件
    $('button').on('click', function () {
      console.log(111111);
    })

    $('button').on('mouseover', function () {
      console.log(2222);
    })
    // 当我点击div的时候 把button上的click事件给解绑了
    $('div').click(function () {
      $('button').off('click');
      $('button').off('mouseover');
    })

```

###### 常见事件类型

### 页面载入事件

```js
// 入口函数
$(function (){
  代码
})
$(document).ready(function(){
  //代码
})
```
##### 		事件切换

​		hover(overfn,outfn)

```js
 // 当我鼠标移入 让div的背景颜色变成green 鼠标移出 变成黄色
    // hover(overfn,outfn)

    $('div').hover(function () {
      $(this).css('backgroundColor', 'green');
    }, function () {
      $(this).css('backgroundColor', 'yellow');
    })
```

toggle()

```js
 // 点击按钮让div在显示和隐藏之间切换
    $('button').on('click', function () {
      $('div').toggle()
    })
```

在鼠标移入移出变化 hover()

在显示和隐藏之间变化 toggle()

##### 		事件坐标

​		  鼠标在元素内相对于元素上左边缘的坐标 e.offsetX e.offsetY
  		鼠标在元素内相对于可视区上左边缘的坐标 e.clientX e.clientY
  		鼠标在元素内相对于页面上左边缘的坐标 e.pageX e.pageY

  `	   注意: 如果页面没有滚动条 client和page一样

##### 		事件冒泡

​		 e.stopPropagation()

##### 		取消事件默认行为(阻止事件冒泡)

​		e.preventDefault();

### 	day05动画（直接看文档/使用手册，重点自定义动画：因为自定义动画是万能的）

##### 		滑动动画

##### 		淡入淡出动画

##### 		显示隐藏动画

##### 		自定义动画





### 	day06

##### 		扩展插件的方法（jQuery插件库，每个插件都有使用方法，用的多了就熟悉了）

jQuery插件库：http://www.jq22.com/

jQuery之家：http://www.htmleaf.com/

##### 		jQuery常用插件学习

推荐下载个jQuery离线手册 英文的版本新 中文版旧 (网上不咋好找，下载网站一般都有广告软件啥的。我QQ:3463426674，直接找我给你发也可以)（为啥不直接发，因为不是我写的，国内大佬写的其实属于公开资源）

