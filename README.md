# HTML CSS学习

## HTML基础

#### 标题标签

h1-h6

```html
<h1>...</h1>
```

#### 段落标签

```html
<p>...</p>
```

#### 换行标签

```html
<br/>
```



#### 文本格式化标签

| 语义   | 标签                             | 示例                  |
| :----- | -------------------------------- | --------------------- |
| 加粗   | `<strong></strong>`或者`<b></b>` | <strong>加粗</strong> |
| 倾斜   | `<em></em>`或者`<i></i>`         | <em>倾斜</em>         |
| 删除线 | `<del></del>`或者`<s></s>`       | <del>删除线</del>     |
| 下划线 | `<ins></ins>`或者`<u><u>`        | <ins>下划线</ins>     |



#### `<div>`和`<span>`标签

```html
<div>...</div>
<span>...</span>
```

`<div>`和`<span>`是没有语义的，它们就是一个子，用来装内容的。

特点：
1.`<div>`标签用来布局，但是现在一行只能放一个`<dv>`。大盒子
2.`<span>`标签用来布局，一行上可以多个`<span>`。小盒子



#### 图像标签

```html
<img src="图像url" alt="文本" title="文本">
```

图像标签的属性：

| 属性   | 属性值   | 说明                                 |
| ------ | -------- | ------------------------------------ |
| src    | 图片路径 | 必须属性                             |
| alt    | 文本     | 替换文本，图像不能显示的文字         |
| title  | 文本     | 提示文本，鼠标放到图像上，显示的文字 |
| width  | 像素     | 设置图像的宽度                       |
| height | 像素     | 设置图像的高度                       |
| border | 像素     | 设置图像的边框粗细                   |



#### 链接标签

```html
<a href="跳转目标"target="目标窗口的弹出方式">文本或图像</a>
```

target属性：

​	_self:本窗口打开

​	_blank:新窗口打开

锚点链接：用于跳转到页面指定位置

```html
<a href="#名称"></a>

目标位置：
<h1 id="名称">...</h1>
```



#### HTML特殊字符

| HTML 原代码 | 显示结果 | 描述                   |
| ----------- | -------- | ---------------------- |
| &lt；       | <        | 小于号或显示标记       |
| &gt；       | \>       | 大于号或显示标记       |
| &amp；      | &        | 可用于显示其它特殊字符 |
| &quot；     | “        | 引号                   |
| &reg；      | ®        | 已注册                 |
| &trade；    | ™        | 商标                   |
| &ensp；     |          | 半个空白位             |
| &emsp；     |          | 一个空白位             |
| &nbsp；     |          | 不断行的空白           |



#### 表格标签

```html
<table>
    <tr>
        <td>单元格内的文字</td>
        ...
    </tr>
    ...
</table>
```

表头单元格标签：`<th>`

一般表头单元格位于表格的第一行或第一列，表头单元格里面的文本内容粗居中显示

```html
<table>
    <tr>
        <th>文本</th>
        ...
    </tr>
</table>
```

表格属性：

| 属性名      | 属性值              | 描述                                             |
| ----------- | ------------------- | ------------------------------------------------ |
| align       | left、center、right | 规定表格相对周围元素的对齐方式。                 |
| border      | 1或""               | 规定表格单元是否拥有边框，默认为""，表示没有边框 |
| cellpadding | 像素值              | 规定单元边沿与其内容之间的空白，默认1像素。      |
| cellspacing | 像素值              | 规定单元格之间的空白，默认2像素。                |
| width       | 像素值或百分比      | 规定表格的宽度。                                 |

表格结构标签

```html
<thead>...</thead>
<tbody>...</tbody>
```

合并单元格：

跨行合并：rowspan="合并单元格的个数
跨列合并：colspan="合并单元格的个数"

示例：

```html
<table align="center" border="2" height="150" width="200" cellspacing="0">
    <tr>
        <td></td>
        <td colspan="2"></td>
    </tr>
    <tr>
        <td rowspan="2"></td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td></td>
        <td></td>
    </tr>
</table>
```

<table align="center" border="2" height="150" width="200" cellspacing="0">
    <tr>
        <td></td>
        <td colspan="2"></td>
    </tr>
    <tr>
        <td rowspan="2"></td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td></td>
        <td></td>
    </tr>
</table>



#### 列表标签

1.无序列表

```html
<ul>
    <1i>列表项1</1i>
    <11>列表项2</1i>
    <1i>列表项3</1i>
    …
</u1>
```

2.有序列表

```html
<o1>
    <1i>列表项1</1i>
    <1i>列表项2</1i>
    <1i>列表项3</1i>
    …
</o1>
```

3.自定义列表

```html
<d1>
    <dt>名词1</dt>
    <dd>名词1解释1</dd>
    <dd>名词1解释2</dd
</d1>
```



#### 表单标签

表单域：

```html
<form>
    ...
</form>
```

##### `<input>`输入表单元素：

```html
<form>
    <input type="text">
</form>
```

`<input>`type属性：

| 属性值   | 描述                                                         |
| -------- | ------------------------------------------------------------ |
| button   | 定义可点击按钮(多数情况下，用于通过JavaScript启动脚本)。     |
| checkbox | 定义复选框。                                                 |
| file     | 定义输入字段和"浏览"按钮，供文件上传。                       |
| hidden   | 定义隐藏的输入字段。                                         |
| image    | 定义图像形式的提交按钮。                                     |
| password | 定义密码字段。该字段中的字符被掩码。                         |
| radio    | 定义单选按钮。                                               |
| reset    | 定义重置按钮。重置按钮会清除表单中的所有数据。               |
| submit   | 定义提交按钮。提交按钮会把表单数据发送到服务器。             |
| text     | 定义单行的输入字段，用户可在其中输入文本。默认宽度为20个字符。 |

`<input>`其他常用属性：

| 属性      | 属性值       | 描述                                  |
| --------- | ------------ | ------------------------------------- |
| name      | 由用户自定义 | 定义input元素的名称。                 |
| value     | 由用户自定义 | 规定input元素的值。                   |
| checked   | checked      | 规定此input元素首次加载时应当被选中。 |
| maxlength | 正整数       | 规定输入字段中的字符的最大长度。      |

示例：

```html
<form action="xxx.php" method="get">
    <!-- text 文本框 用户可以里面输入任何文字 -->
    用户名: <input type="text" name="username" value="请输入用户名" maxlength="6">   <br> 
    <!-- password 密码框 用户看不见输入的密码 -->
    密码: <input type="password" name="pwd" >  <br> 
    <!-- radio 单选按钮  可以实现多选一 -->
    <!-- name 是表单元素名字 这里性别单选按钮必须有相同的名字name 才可以实现多选1 -->
    <!-- 单选按钮和复选框可以设置checked 属性, 当页面打开的时候就可以默认选中这个按钮 -->
    性别: 男 <input type="radio" name="sex" value="男"> 女  <input type="radio" name="sex" value="女" checked="checked"> 人妖   <input type="radio" name="sex" value="人妖">   <br> 
    <!-- checkbox 复选框  可以实现多选 -->
    爱好: 吃饭 <input type="checkbox" name="hobby" value="吃饭"> 睡觉 <input type="checkbox" name="hobby">  打豆豆 <input type="checkbox" name="hobby" checked="checked"> 
    <br> 
    <!-- 点击了提交按钮,可以把 表单域 form 里面的表单元素 里面的值 提交给后台服务器 -->
    <input type="submit" value="免费注册">
    <!-- 重置按钮可以还原表单元素初始的默认状态 -->
    <input type="reset" value="重新填写">
    <!-- 普通按钮 button  后期结合js 搭配使用-->
    <input type="button" value="获取短信验证码"> <br>
    <!-- 文件域 使用场景 上传文件使用的 -->
    上传头像:  <input type="file" >
</form>

```

<form action="xxx.php" method="get">
         <!-- text 文本框 用户可以里面输入任何文字 -->
        用户名: <input type="text" name="username" value="请输入用户名" maxlength="6">   <br> 
        <!-- password 密码框 用户看不见输入的密码 -->
        密码: <input type="password" name="pwd" >  <br> 
        <!-- radio 单选按钮  可以实现多选一 -->
        <!-- name 是表单元素名字 这里性别单选按钮必须有相同的名字name 才可以实现多选1 -->
        <!-- 单选按钮和复选框可以设置checked 属性, 当页面打开的时候就可以默认选中这个按钮 -->
        性别: 男 <input type="radio" name="sex" value="男"> 女  <input type="radio" name="sex" value="女" checked="checked"> 人妖   <input type="radio" name="sex" value="人妖">   <br> 
        <!-- checkbox 复选框  可以实现多选 -->
        爱好: 吃饭 <input type="checkbox" name="hobby" value="吃饭"> 睡觉 <input type="checkbox" name="hobby">  打豆豆 <input type="checkbox" name="hobby" checked="checked"> 
        <br> 
        <!-- 点击了提交按钮,可以把 表单域 form 里面的表单元素 里面的值 提交给后台服务器 -->
        <input type="submit" value="免费注册">
        <!-- 重置按钮可以还原表单元素初始的默认状态 -->
        <input type="reset" value="重新填写">
        <!-- 普通按钮 button  后期结合js 搭配使用-->
        <input type="button" value="获取短信验证码"> <br>
        <!-- 文件域 使用场景 上传文件使用的 -->
        上传头像:  <input type="file" >
    </form>



##### `<label>`标签：

`<label>`标签为input元素定义标注（标签）。
`<label>`标签用于绑定一个表单元素，当点击`<label>`标签内的文本时，浏览器就会自动将焦点（光标转到或者
选择对应的表单元素上，用来增加用户体验。

```html
<label for="text">用户名：</label><input type="text"id="text">
<input type="radio"id="nan"name="sex"><label for="nan">男</label>
<input type="radio"id="nv"name="sex"><label for="nv">女</label>
```

<form>
    <label for="text">用户名：</label><input type="text"id="text">
    <input type="radio"id="nan"name="sex"><label for="nan">男</label>
    <input type="radio"id="nv"name="sex"><label for="nv">女</label>
</form>



##### `<select>`下拉表单元素：

```html
<select>
    <option>选项1</option>
    <option selected="selected">选项2</option>
    <option>选项3</option>
</select>
```

<form>
    选项：
    <select>
        <option>选项1</option>
        <option selected="selected">选项2</option>
        <option>选项3</option>
    </select>
</form>



##### `<textarea>`文本域元素：

使用场景：当用户输入内容较多的情况下，我们就不能使用文本框表单了，此时我们可以使用`<textarea>`标签。
在表单元素中，`<textarea>`标签是用于定义多行文本输入的控件。

```html
<textarea rows="3"cols="20">
    文本内容
</textarea>
```

<form>
    <textarea rows="3"cols="20">文本内容</textarea>
</form>

cols=“每行中的字符数”，rows=“显示的行数”，我们在实际开发中不会使用，都是用CSS来改变大小。

