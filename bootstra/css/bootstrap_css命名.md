# bootstrap
### 布局
.container
.container-gluid


.form-group  表单组建；默认宽度100%
.form-inline 横向表单 display inlink-blcok
.form-conttrol 表单控件
.examInputEmail  邮箱
.examInputPassword 密码
.examInputUsername  用户名
.select  选择框
.selectFile 选择文件
.inputSubmit  按钮提交
.help-block 文件路径提示信息
.input-group 输入框组件
  - input-group-addcon
  - input-group-add加
  - input-group-decaleine 减少
  - input-group-addIcon 添加图标

水平排列表单
.from-horizontal 可以使Label 水平排列


内联单选多选框 .Checkbox-inline
多选：
.inlineCheckbox
单选：
.inlineRadioOption

不带文本的选择框 
.checkbox
正方形 
.blankcheckbox
圆形    
.blankradio


静态控件
.control-label
.form-control-static
禁止输入 #disableInput

效验样式
.has-success 成功   字体边框    绿色
.has-warning 警告   字体边框    黄色
.has-error 失败     字体边框    红色

尺寸
.input-lg 大输入框
.input-sm 小输入框


 ### 图片命名方式
 img-rounded 圆角
 img-circle  圆形图片
 img-thumbnail 有边框样式

 ###  辅助类：
 text-muted  默认
 text-suceess
 text-primary
 text-info
 text-danger
 text-warning 
 ~~~CSS
  /* 样式 */
  p{
      margin: 0 0 10px;
  }
  .text-muted{
    color:#777
  }
  .text-success{
       color:green;
  }
~~~

 ### 情景背景色
 .bg-info
 .bg-success
 .bg-primary 
 .bg-warning  
 .bg-danger
~~~css
.bg-xxx{
  /*yellow是可以被改变的值+-  */
  background-color:yellow
}

~~~

### 关闭按钮
.close  浮动到右侧 
button.close

### 三角
.caret

### 快速浮动
.pull-left !improtant   左浮动
.pull-right !improtant  右浮动

### 让容器块居中
.cener-block
~~~css
.center-block{
  display:block;
  margin:0 auto;
}
~~~

### 清除浮动
.clearfix 使用伪类清除浮动  ——————>自己封装

### 强制显示隐藏
.show   显示  !improtant  display:block;
.hidden 隐藏  !improtant  display:none;
.invisible  visibility: hidden;


### 文字隐藏
~~~CSS
.text-hide {
    font: 0/0 a;
    color: transparent;
    text-shadow: none;
    background-color: transparent;
    border: 0;
}
~~~ 

### 排版
.text-left    文字左对齐
.text-center  文字居中对齐
.text-right   文字右对齐
.text-justiyf 两端对齐
.text-nowrap  不换行

.text-lowercase  小写英文
.text-uppercase  大写英文
.text-capitalize 首字母英文大写

### 缩写
~~~css
abbr[title], abbr[data-original-title] {
    cursor: help;
    border-bottom: 1px dotted #777;
~~~

### 内联列表（横向列表项）
~~~css
.list-inline {
    padding-left: 0;
    margin-left: -5px;
    list-style: none;
}
.list-inline > li {
    display: inline-block;
    padding-right: 5px;
    padding-left: 5px;
}
~~~

### 用户输入
~~~css
kbd {
    padding: 2px 4px;
    font-size: 90%;
    color: #fff;
    background-color: #333;
    border-radius: 3px;
    -webkit-box-shadow: inset 0 -1px 0 rgba(0, 0, 0, .25);
    box-shadow: inset 0 -1px 0 rgba(0, 0, 0, .25);
  }
  ~~~

  ### 表格

  基础类
  .table 必须放在 table
  1:清空表格默认样式 条状表格
  ~~~css
  .table {
    width: 100%;
    max-width: 100%;
    margin-bottom: 20px;
  }
  .table {
    background-color: transparent;
  }

.table {
    border-spacing: 0;
    border-collapse: collapse;
  }
  /* *让表格有上边框线 选中所有的th td */
  ~~~css
.table > thead > tr > th, .table > tbody > tr > th, .table > tfoot > tr > th, .table > thead > tr > td, .table > tbody > tr > td, .table > tfoot > tr > td {
    padding: 8px;
    line-height: 1.42857143;
    vertical-align: top;
    border-top: 1px solid #ddd;
}
~~~

  ##### 条状表格
  .taable-striped
  ~~~css
  /* odd 奇数 even 偶数 选中标题奇数行加背景颜色 */
  .table-striped > tbody > tr:nth-of-type(odd) {
    background-color: #f9f9f9;
  }
  ~~~
  ##### 带边框表格
  .table-bordered
  ~~~css
  .table-bordered{
    border：1px soild #ccc
  }
  ~~~
  #### 表格悬停样式
  .table-hover
  ~~~css
  ~~~
  ### 紧缩表格
  .table-condensed 缩小表格列的内边距


 ### 状态

仅支持表格

~~~~css
.table > thead > tr > td.warning,
.table > tbody > tr > td.warning, 
.table > tfoot > tr > td.warning, 
.table > thead > tr > th.warning, 
.table > tbody > tr > th.warning, 
.table > tfoot > tr > th.warning, 
.table > thead > tr.warning > td, 
.table > tbody > tr.warning > td,
.table > tfoot > tr.warning > td, 
.table > thead > tr.warning > th, 
.table > tbody > tr.warning > th, 
.table > tfoot > tr.warning > th {
    background-color: #fcf8e3;
}
~~~~


### 总结
表格中独有的类名；是通过关系型选择器；选择的面面俱到；才可以使用
同理可证；表单；辅助等一样

### 响应式表格
.table-responsive
~~~css
@media screen and (max-width: 767px)
.table-responsive {
    width: 100%;
    margin-bottom: 15px;
    overflow-y: hidden;
    -ms-overflow-style: -ms-autohiding-scrollbar;
    border: 1px solid #ddd;
}
.table-responsive {
    min-height: .01%;
    overflow-x: auto;
}
/* 实现横向滚动条 */
@media screen and (max-width: 767px){
.table-responsive > .table > thead > tr > th,
    .table-responsive > .table > tbody > tr > th, 
    .table-responsive > .table > tfoot > tr > th, 
    .table-responsive > .table > thead > tr > td,
    .table-responsive > .table > tbody > tr > td, 
    .table-responsive > .table > tfoot > tr > td {
    white-space: nowrap;
}
~~~

### 栅格系统
1：栅格应用的是媒体查询技术；
2：间隔一个容器等分为12小份
3：应用在布局上

原理：主要通过设置元素的宽度完成百分比
  当一个元素只有一个col-xxx的时候不看屏幕尺寸只看元素宽度 col-12宽度为100%
  当一个元素有多个col-xxx的时候，先看屏幕尺寸再看元素宽度col-xxx宽度为50%
  栅格大类.col
  尺寸划分.col
  xs  <768px
  sm  >=768px
  md  >=992px
  lg  >=1200px
  元素宽度划分
  1   width=8.33333333%;
  2   width=16.66666667%;
  3   width=25%;
  4   width=33.33333333%;
  5   width=41.66666667%;
  6   width=50%;
  7   width=58.33333333%;
  8   width=66.66666667%;
  9   width=75%;
  10  width=83.33333333%;
  11  width=91.66666667%;
  12  width=100%
   

### 列偏移
原理： 通过设置元素左外边距移动元素
offset-1   width=8.33333333%;
offset-2   width=16.66666667%;
offset-3   width=25%;
offset-4   width=33.33333333%;
offset-5   width=41.66666667%;
offset-6   width=50%;
offset-7   width=58.33333333%;
offset-8   width=66.66666667%;
offset-9   width=75%;
offset-10  width=83.33333333%;
offset-11  width=91.66666667%;
offset-12  width=100%
   
   ### 相对定位
   因为.col-xx-num 都有posotion：relative；
   .col-xxx-push-num：设有left相对自身位置往右移动
   .col-xxx-pull-num：设有right相对自身位置往左移动
   所有：想要.col-xx-push-num  col-xx-pull-num 起效；必须填  col-xx-num
### 基础类 .container
row 行
column 列
可以嵌套
将容器进行份数等分
.col-xs-12  小于768px
.col-sm-12  大于768px
.col-md-12  
.col-lg-12  大于1200px
