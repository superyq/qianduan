<h1>html标签笔记</h1>

## html标签修饰

```
<html lang='en'></html>

en: 英文
zh-CN: 中文
ja-jp: 日文
```

## 文本标签

```
i: 倾斜
b: 加粗
ins: 下划线
sup: 上标
sub: 下标
del: 删除
```

## 语义化标签

```
section内容块，article独立内容，aside，header,footer，nav,figure,main
```

## hr属性

```
<hr color='red' width='50' align='left' noshade>

color: 颜色
width：宽度
align: 局左或右
noshade: 没有阴影
```

## 特殊符号

```
&lt: 左尖角
&gt: 右尖角
&nbsp: 空格（受字体影响）
&emsp: 空格（不受字体影响）
&cope: 版权
&trade,&reg: 商标
```

## 列表

```
ul > li: 无序列表
    type: disc, circle, square, none
ol > li: 有序列表
    type: 1,a,A,i,I  有序的类型
    start: 2         有序开始,只能是数字开始
dl > dt,dd: 自定义列表
```

## 图片属性

```
<img src='路径' title='标题' alt='加载失败显示' width='200px' height='200px'>
```

## 超链接标签

```
<a href='路径' title='提示信息' target='打开形式'></a>

target: _self默认直接跳转，_blank新开网页跳转
```

## 表格

```
table > tr > td

table
    width: 宽度
    height: 高度
    border: 边框
    bordercolor: 边框颜色
    bgcolor:  背景色
    align: 表格位置
    cellspacing: 单元格间距
    cellpadding: 单元格与内容之间的间隙
tr
    height: 高度
    bgcolor: 背景色
    align: 文字水平对齐 
    valign: 文字垂直对齐
td
    width: 宽度
    height: 高度
    bgcolor: 背景色
    align:  文字水平对齐
    valign:  文字垂直对齐
```

## 表单

```
<form method='get或post' action='向何处发送表单数据'>
    <input  type='text' placeholder='提示信息' name='必须设置，否则提交表单时不会发送到服务器' value=''/>
                text: 文本框
                password: 密码
                submit: 按钮
                reset: 清空
                radio: 单选框
                checkbox: 多选框
                file: 上传文件
                image: 上传文件
                color: 生成颜色选择表单
                tel: 唤起拨号盘表单
                search: 搜索意义的表单
                range: 滑动条表单
                number: 数值表单
                email: 输入email类型
                url: 必须输入url类型
                date: 必须输入日期
                month: 必须输入月类型
                week: 必须输入周类型
                time: 必须输入时间类型
                datetime-local: 选取本地时间
</form>
```

## h5新增标签

```
<video src='' controls></video> 视频
<audio src=''> 音频

controls: 控件
autopaly: 自动播放
loop: 循环播放
muted: 静音
poster: 下载显示影像
```