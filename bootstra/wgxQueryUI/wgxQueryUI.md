# wgxQueryUI全局样式说明文档
## 清空默认样式

## 布局
.g-container 设置为容器 ：水平方向居中 宽度部位100% 左右内边距为15px 高度没有
.g-container-fluid 宽度为100% 的容器 没有外边距 内边距15px 上下0px 没高度


## 按钮  g-btn
成功    g-btn-success
失败    g-btn-fail
警告    g-btn-warining
错误    g-btn-error
取消    g-btn-cancel
确定    g-btn-sure
默认    g-btn-default
危险    g-btn-danger
首选    g-btn-primany
一般信息    g-btn-info
禁止按钮    g-btndisable
百搭按钮    g-btnnormal
暖色按钮    g-btn-warm



#### 渐变按钮样式
成功    g-btn-success-rgb
失败    g-btn-fail-rgb
警告    g-btn-warining-rgb
错误    g-btn-error-rgb
取消    g-btn-cancel-rgb
确定    g-btn-sure-rgb
默认    g-btn-default-rgb
危险    g-btn-danger-rgb
首选    g-btn-primany-rgb
一般信息    g-btn-info-rgb
禁止按钮    g-btndisable-rgb
百搭按钮    g-btnnormal-rgb
暖色按钮    g-btn-warm-rgb


#### 伪类按钮样式




- 型号

大  g-btn-bgl
小  g-btn-sm
中  g-btn-md


- 圆角按钮 g-btn-radius



#### 伪类按钮样式

## 表单样式组件
1：只有表单样式，分为基础样式与可选择样式 如果有特殊需要请自定义
2：变淡没有进行验证处理 有对验证效果样式处理：statice 状态。
3：表单的验证需要js 正则完成 
注意：正则必须写基础正则，不要写新的正则，因为IE和火狐部分版本不兼容
<!-- 基础表单 -->
.form-gorup 表示表单组件
.form-control 表示表单控件
.form-label 表示input的提示信息 只能应用在label
#### 可选项表单样式
.form-inline 表示横向表单
.form-horizontal    纵向表单
### 表单中控件
.form-check 选择框组件 在ul 中使用
.form-check-item 表示多选择项 在li中使用
.form-content 表示的文本描述

## 滑块

## select选择框

## 表格 .g-table
.g-table 表示基础表格；必须在table标签中使用；表示只有列边框的表格
.g-tableStriped 表示条状表格；表体的偶数行；有一定的背景颜色
.g-table-column 表示半边框样式
.g-tableHover    表示悬浮biaoge
.g-tableCondensed 紧缩表格
.g-tableBorder  边框表格
.g-tableInverse 背景色为黑色的表格。
.g-tableInverse_striped 黑色条形的表格
.g-tableInverse_hover   黑色悬浮样式 需要依赖.g-tableInverse或者.g-tableInverse_striped
.g-tableResponsive   移动端表格 可以有横向滚动条效果    .g-tableResponsive  需要.g-table 的父容器添加
.g-table-control 表示控制列 固定其他列可以滚动 .g-table-control 必须给 标签添加组级元素添加而不是给父元素添加

状态表格 给tr添加类名
.success 成功
.info    通过
.warning  警告
.danger  危险
.primary 首选
.warm    暖色


## 栅格系统 .col
栅格系统是横向布局的处理
提示信息：如果父容器不适用.row 那么自己清除浮动计算父容器高度
### 容器 .row
将.row容器等分为12份
### 屏幕
.col-xs-xx  768px   以下的尺寸
.col-sm-xx  768以上 992以下
.col-md-xx  992px以上   1200以下
.col-lg-xx  1200以上

#### 分的份数   小数点后 7位数
1-  8.33333333%
2-  16.6666667%
3-  25%
4-  33.3333333%
5-  41.6666667%
6-  50%
7-  58.3333333%
8-  66.6666667%
9-  75%
10- 83.3333333%
11- 91.6666667%
12- 100%



### 列偏移 
通过改变position：relative left 实现列偏移
*表示 1 2 3 4 5 6  7 8 9 10 11 12 
.col-xs-offset-*
.col-sm-offset-*
.col-md-offset-*
.col-lg-offset-*
### 列偏移量
1
2
3
4
5
6
7
8
9
10
11
12
### 排列
.col-xs-pull-*相对元素位置右边多(往左走)
.col-xs-push-*





### 分页 .page
.pagination 实现分页样式 有ul li a 完成分页效果
.pagination-bgc 表示带有背景颜色的分页
.pagination-noBgc表示没有背景颜色
.pagination-inverse黑色分页

### 表单类
### 单选多选框样式
.circle-check   圆形选择框  .circle-check  需要给input[type=checkbox]的父元素添加
.square-check   方形选择框  .square-check  需要给input[type=checkbox]的父元素添加
~~~html
<!-- 示例代码 -->
 <div class="circle-check">
        <input type="checkbox">
    </div>
    <div class="square-check">
        <input type="checkbox">
    </div>
~~~
### 滑块    .sliderbar
.slider-wrap        表示进度条外围的容器
.sliderbar 表示 滑块的 条
.sliderbar-control  表示控制键
~~~html
<div class="sliderbar-box">
        <div class="sliderbar">
            <div class="sliderbar-control">
                55
            </div>
        </div>
    </div>
~~~
# 状态
.sliderbar-success绿
.sliderbar-info蓝
.sliderbar-primary红
.sliderbar-error灰

### 开关 .switch
.switch 开关样式的选择框 需要给input[type=checkbox].switch 才能实现效果
 - 绿色为开 input=checkbox 灰色为关 input=disable
 状态
 .switch-info 蓝开 灰关
 .switch-danger 红开灰关
 .switch-warm   橙色 灰关
 .switch-primary 蓝开红关

### 步骤组件    .step
.step-wrap  为外部容器 宽为55rem
.step-full  表示每个步骤的容器 包含内容 圈 线 还有文本
.step       具体进行的每一步 用的是input[type=checkbox],当有checked属性表示当前步骤已经完成.
.step-circle 表示圈
.stpe-line  表示线
.step-text  表示步骤内容

# 状态
.step-circle-info
.step-circle-success
.step-circle-primary
.step-circle-warm
.step-circle-error
.step-circle-danger



### 导航    .nav
注意：导航仅仅适用于pc端 应用；且只适应静态样式 导航中所有的样式都是操作li下的a标签

.nav-tabe       表示像table的导航条 需要依赖.nav
.nav-pills      胶囊式导航  需要依赖.nav
.nav-stacked    侧边导航栏
.nav-inverse    表示背景色为黑色的导航  需要依赖.nav
.nav-aside      表示侧边导航    需要依赖.nav
.nav-fixed-top  表示固定导航 在顶部 需要依赖.nav
.nav-fixed-left 表示固定导航 屏幕在左部 需要依赖.nav
.nav-fixed-right 表示固定导航 屏幕在右部    需要依赖.nav

### 导航条 .navnar
注意：兼容移动端

 兼容移动端样式设置规则：媒体查询最小宽度；写pc端样式；当小于这个宽度时候；使用浏览器默认样式
网站的导航条；到移动端时候可以折叠 

.navbar  导航条 兼容pc 移动 默认样式隐藏
.navbar-default 给导航条添加样式 【背景色】
.navbar-header 有媒体查询样式；做PC 端和移动端区分； 移动端宽度100%
.collapse  元素隐藏[移动端]
.nav-collapse.collapse 在pc 端【强制】显示
.navbar-nav 表示导航条下导航
.navbar-form 表示导航条中输入框
.navbar-left 让导航在导航条中左浮动【移动端无浮动】
.navbar-right 让导航有又浮动【移动端无浮动效果】
.navbar-toggle 表示显示隐藏列表导航栏，有【右浮动】效果

.navbar-fixed-top 固定顶部导航条
.navbar-inverse 黑色导航条 border-bottom:1px solid black
   .navbar .active  背景颜色黑色  字体白色

 .breadcrumb 表示路径导航；没有基础类  

  - 每个a 添加伪元素； content:"Z/\00a0"


## 规范：
1：清空所有html标签的默认样式

2：字体：标准14px 最大36px 最小12px

3：布局： 栅格系统 ：给一个父容器等分多少份
    12列
        每个子元素可以占12列中 1-12 最大12份
        col-12 占据12份



### 开发浏览器注意事项
1：如果您是IE7 8 请您更换浏览器
2：IE7 尽量全部使用div 例如
 - ul div.ul
 - li div.li
 - span div.span 设置display：inline

 3.IE7 8不支持浮动 清除浮动 css3百分之90的属性 