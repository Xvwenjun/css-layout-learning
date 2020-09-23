# 学习布局
## Flow布局（默认文档流）/Layer布局（定位）/Float浮动/Flex布局

### 定位
绝对定位`position：absolute；`  会脱离文档流

`z-index` 仅对定位元素有效

### Float
* 设置了`float` 也会脱离文档流，float的设计初衷是用于文字环绕。

* 设置了`float`的元素宽度会变为内容的宽度，而不是默认的屏幕宽度，但其dispaly样式依旧没变，仍然是block。

* `float`清空格：由于img是block元素，多个<img>之间浏览器会将其识别为空格。当设置为`float`布局后，多个排列的img之间的空格就会被清除。（本质原因是float让元素都脱离了文档流，以前的格式将会失效)



### 实战
1、info-box列表消息盒子    

2、hidden-info-pannels滑动隐藏面板  

* `label` 和 `input` 可以通过 `for` 属性来绑定`id`，来联系`input`和表单元素。
 这样，可以通过点击input元素的label来选择这个input盒子，就像点击了这个input一样。
 （具体了解checkbox hack技术，无js实现点击按钮的动画效果）
 


3、flex-box弹性盒子
* `order`属性： 默认值为0，按照order值的大小，flex项按照从小到大的顺序依次排列，相同值则按照源代码的顺序显示

4、sticky-positioning滚动索引页面

********************
* 三种外边距重叠
https://developer.mozilla.org/zh-CN/docs/Web/CSS/CSS_Box_Model/Mastering_margin_collapsing

* BFC 块级格式化内容（ Block formatting contexts ）
https://developer.mozilla.org/zh-CN/docs/Web/Guide/CSS/Block_formatting_context

* haslayout
 

* 四种选择器
1、 后代选择器
2、 > 直接后代选择器
3、 + 相邻兄弟选择器
4、 ~ 后续兄弟选择器


# 网页布局
## 一列布局
直接使用`margin：0 auto；`

## 两列布局 （左左浮动、左右浮动）
使用`float`实现（需要及时清除浮动）
1、父元素必须要确定高度，否则要用`overflow：hidden；` 来为父元素清除浮动影响

2、对于相邻的元素，使用`clear：both；`清除浮动影响

## 三列布局：两侧定宽，中间自适应
1、（左左右浮动、或都左浮动）

`calc` 动态计算宽度，宽度自适应

2、父元素设置relative，子元素设置absolute


## 混合布局



