HTML DOM是HTML Document Object Model(文档对象模型)的缩写，定义了访问和操作 HTML 文档的标准方法

DOM 以树结构表达 HTML 文档。

#### 什么是 DOM？
DOM 是 W3C（万维网联盟）的标准。
DOM 定义了访问 HTML 和 XML 文档的标准：

"W3C 文档对象模型 （DOM） 是中立于平台和语言的接口，它允许程序和脚本动态地访问和更新文档的内容、结构和样式。"

#### W3C DOM 标准被分为 3 个不同的部分：
核心 DOM - 针对任何结构化文档的标准模型<br>
XML DOM - 针对 XML 文档的标准模型<br>
HTML DOM - 针对 HTML 文档的标准模型

DOM 是 Document Object Model（文档对象模型）的缩写。

#### 什么是 XML DOM？
XML DOM 定义了所有 XML 元素的对象和属性，以及访问它们的方法

#### 什么是 HTML DOM？
HTML DOM 是：<br>
HTML 的标准对象模型<br>
HTML 的标准编程接口<br>
W3C 标准

HTML DOM 定义了所有 HTML 元素的对象和属性，以及访问它们的方法。
换言之，HTML DOM 是关于如何获取、修改、添加或删除 HTML 元素的标准

#### HTML DOM 节点
在 HTML DOM 中，所有事物都是节点。DOM 是被视为节点树的 HTML。

#### DOM 节点
根据 W3C 的 HTML DOM 标准，HTML 文档中的所有内容都是节点: <br>
整个文档是一个文档节点<br>
每个 HTML 元素是元素节点<br>
HTML 元素内的文本是文本节点<br>
每个 HTML 属性是属性节点<br>
注释是注释节点<br>

#### 节点父、子和同胞
节点树中的节点彼此拥有层级关系。

父（parent）、子（child）和同胞（sibling）等术语用于描述这些关系。父节点拥有子节点。同级的子节点被称为同胞（兄弟或姐妹）。

在节点树中，顶端节点被称为根（root）<br>
每个节点都有父节点、除了根（它没有父节点）<br>
一个节点可拥有任意数量的子节点<br>
同胞是拥有相同父节点的节点<br>

DOM 处理中的常见错误是希望元素节点包含文本。<br>
在本例中：<title>DOM 教程</title>，元素节点 <title>，包含值为 "DOM 教程" 的文本节点。<br>
可通过节点的 innerHTML 属性来访问文本节点的值。

### DOM方法
HTML DOM方法是我们可以在节点（HTML 元素）上执行的动作

#### 编程接口
可通过 JavaScript （以及其他编程语言）对 HTML DOM 进行访问。<br>
所有 HTML 元素被定义为对象，而编程接口则是对象方法和对象属性。<br>
方法是您能够执行的动作（比如添加或修改元素）。<br>
属性是您能够获取或设置的值（比如节点的名称或内容）。

#### getElementById() 方法
getElementById() 方法返回带有指定 ID 的元素

#### HTML DOM 对象 - 方法和属性
一些常用的 HTML DOM 方法：<br>
getElementById(id) - 获取带有指定 id 的节点（元素）<br>
appendChild(node) - 插入新的子节点（元素）<br>
removeChild(node) - 删除子节点（元素）<br>

一些常用的 HTML DOM 属性：<br>
innerHTML - 节点（元素）的文本值<br>
parentNode - 节点（元素）的父节点<br>
childNodes - 节点（元素）的子节点<br>
attributes - 节点（元素）的属性节点

#### 一些 DOM 对象方法

getElementById() &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;	返回带有指定 ID 的元素。<br>
getElementsByTagName()	&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;返回包含带有指定标签名称的所有元素的节点列表（集合/节点数组）。<br>
getElementsByClassName()	&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;返回包含带有指定类名的所有元素的节点列表。<br>
appendChild()	&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;把新的子节点添加到指定节点。<br>
removeChild()&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;	删除子节点。<br>
replaceChild()&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;	替换子节点。<br>
insertBefore()	&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;在指定的子节点前面插入新的子节点。<br>
createAttribute()	&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;创建属性节点。<br>
createElement()&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;	创建元素节点。<br>
createTextNode()&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;	创建文本节点。<br>
getAttribute()&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;	返回指定的属性值。<br>
setAttribute()&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;	把指定属性设置或修改为指定的值。<br>

### HTML DOM 属性
属性是节点（HTML 元素）的值，您能够获取或设置。

#### 编程接口
可通过 JavaScript （以及其他编程语言）对 HTML DOM 进行访问。<br>
所有 HTML 元素被定义为对象，而编程接口则是对象方法和对象属性。<br>
方法是您能够执行的动作（比如添加或修改元素）。<br>
属性是您能够获取或设置的值（比如节点的名称或内容）。

#### innerHTML 属性
获取元素内容的最简单方法是使用 innerHTML 属性。
innerHTML 属性对于获取或替换 HTML 元素的内容很有用。


innerHTML 属性可用于获取或改变任意 HTML 元素，包括 \<html> 和 \<body>。

#### nodeName 属性规定节点的名称。
nodeName 是只读的<br>
元素节点的 nodeName 与标签名相同<br>
属性节点的 nodeName 与属性名相同<br>
文本节点的 nodeName 始终是 #text<br>
文档节点的 nodeName 始终是 #document<br>

注意事项： <br>
nodeName 始终包含 HTML 元素的大写字母标签名。

#### nodeValue 属性
nodeValue 属性规定节点的值。<br>
元素节点的 nodeValue 是 undefined 或 null<br>
文本节点的 nodeValue 是文本本身<br>
属性节点的 nodeValue 是属性值

#### 获取元素的值

#### nodeType 属性
nodeType 属性返回节点的类型，nodeType 是只读的<br>
下表是比较重要的节点类型：<br>

元素类型 &nbsp; NodeType <br>
元素	&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; 1<br>
属性	&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; 2<br>
文本	&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; 3<br>
注释	&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; 8<br>
文档	&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; 9

### HTML DOM访问
访问 HTML DOM - 查找 HTML 元素。

#### 访问 HTML 元素（节点）
访问 HTML 元素等同于访问节点

可以以不同的方式来访问 HTML 元素: <br>
通过使用 getElementById() 方法<br>
通过使用 getElementsByTagName() 方法<br>
通过使用 getElementsByClassName() 方法

#### getElementById() 方法
getElementById() 方法返回带有指定 ID 的元素：<br>
语法<br>
node.getElementById("id");

#### getElementsByTagName() 方法
getElementsByTagName() 返回带有指定标签名的所有元素。

语法<br>
node.getElementsByTagName("tagname"); 

#### The getElementsByClassName() Method
如果希望查找带有相同类名的所有 HTML 元素，可以使用这个方法进行查找<br>

#### The getElementsByClassName() Method
如果希望查找带有相同类名的所有 HTML 元素，可以使用这个方法进行查找<br>
document.getElementsByClassName("intro");

上面的例子返回包含 class="intro" 的所有元素的一个列表：<br>
注意事项：getElementsByClassName() 在 Internet Explorer 5,6,7,8 中无效

#### 修改 HTML 元素

修改 HTML DOM 意味着许多不同的方面：<br>
改变 HTML内容<br>
改变 CSS 样式<br>
改变 HTML 属性<br>
创建新的 HTML 元素<br>
删除已有的 HTML 元素<br>
改变事件（处理程序）

#### 创建 HTML 内容
改变元素内容，最简单的方法是使用 innerHTML 属性。

#### 改变 HTML 样式
通过 HTML DOM，您能够访问 HTML 元素的样式对象。

#### 创建新的 HTML 元素
如果需要向 HTML DOM 添加新元素，您首先必须创建该元素（元素节点），然后把它追加到已有的元素上。

#### HTML DOM - 修改 HTML 内容
通过 HTML DOM，JavaScript 能够访问 HTML 文档中的每个元素。

#### 改变 HTML 内容
改变元素内容的最简单的方法是使用 innerHTML 属性。

#### 改变 HTML 样式
通过 HTML DOM，您能够访问 HTML 对象的样式对象。

#### 使用事件
HTML DOM 允许您在事件发生时执行代码。

当 HTML 元素"有事情发生"时，浏览器就会生成事件：<br>
在元素上点击<br>
加载页面<br>
改变输入字段

#### 创建新的 HTML 元素 - appendChild()
如果需要向 HTML DOM 添加新元素，您首先必须创建该元素，然后把它追加到已有的元素上

#### 创建新的 HTML 元素 - insertBefore()

#### 删除已有的 HTML 元素
如果您需要删除 HTML 元素，您必须清楚该元素的父元素

能否在不引用父元素的情况下删除某个元素？<br>
很抱歉。DOM 需要了解您需要删除的元素，以及它的父元素。

提供一个常用的解决方法：找到您需要删除的子元素，然后使用 parentNode 属性来查找其父元素：<br>
var child=document.getElementById("p1");
child.parentNode.removeChild(child);

#### 替换 HTML 元素
如果您需要替换 HTML DOM 中的元素，请使用 replaceChild() 方法

### HTML DOM - 事件
HTML DOM 允许 JavaScript 对 HTML 事件作出反应。

### HTML 事件的例子：
当用户点击鼠标时<br>
当网页已加载时<br>
当图片已加载时<br>
当鼠标移动到元素上时<br>
当输入字段被改变时<br>
当 HTML 表单被提交时<br>
当用户触发按键时<br>

#### HTML 事件属性
如果您需要向 HTML 元素分配事件，您可以使用事件属性。

#### 使用 HTML DOM 来分配事件
HTML DOM 允许您使用 JavaScript 向 HTML 元素分配事件

#### onload 和 onunload 事件
当用户进入或离开页面时，会触发 onload 和 onunload 事件。<br>
onload 事件可用于检查访客的浏览器类型和版本，以便基于这些信息来加载不同版本的网页。<br>
onload 和 onunload 事件可用于处理 cookies。

#### onchange 事件
onchange 事件常用于输入字段的验证。

#### onmouseover 和 onmouseout 事件
onmouseover 和 onmouseout 事件可用于在鼠标指针移动到或离开元素时触发函数。

#### onmousedown、onmouseup 以及 onclick 事件
onmousedown、onmouseup 以及 onclick 事件是鼠标点击的全部过程。首先当某个鼠标按钮被点击时，触发 onmousedown 事件，然后，当鼠标按钮被松开时，会触发 onmouseup 事件，最后，当鼠标点击完成时，触发 onclick 事件。

#### HTML DOM 导航

通过 HTML DOM，您可以使用节点关系在节点树中导航。

#### HTML DOM 节点列表
getElementsByTagName() 方法返回节点列表。节点列表是一个节点数组。

#### HTML DOM 节点列表长度
length 属性定义节点列表中节点的数量。<br>
可以使用 length 属性来循环节点列表

#### 导航节点关系
您能够使用三个节点属性：parentNode、firstChild 以及 lastChild ，在文档结构中进行导航。

#### DOM 根节点
这里有两个特殊的属性，可以访问全部文档：<br>
document.documentElement - 全部文档<br>
document.body - 文档的主体

#### childNodes 和 nodeValue
除了 innerHTML 属性，您还可以使用 childNodes 和 nodeValue 属性来获取元素的内容。







