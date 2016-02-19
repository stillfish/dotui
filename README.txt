# Powereasy initial template

标准化后的标签、模板整理。

可用于**全新项目**制作前，批量覆盖更新一些老旧标签，并使用标准化后的模板。

## 使用方式

直接覆盖项目 `Template` 文件夹下的各同名目录即可。

**特殊说明：**标签覆盖后要到后台检查一下有没有重复标签，一般有可能出现重复的标签是 `网站头部` 和 `网站底部`，删除原有文件即可。

## 目录介绍

### Skin
存放样式文件。这里仅剩一些没有做到 [Powereasy-initial-styles](https://git.oschina.net/laomao800/Powereasy-initial-styles) 的基础文件。

### 分页标签库
删除默认的 `url_方块样式分页` 内置烦人的css。

### 标签库
标准化标签，其中部分个人更新过。

### 模板库
覆盖时注意项目模板库文件夹有随机字符后缀，需手动复制进去。  
`PE-定制模板` 内，`文章-内容页`、`通用-单页` 有是否有侧栏2个版本可以选择，`留言-内容页`有是否有头像可以选择，视情况而用。

## 特殊目录（以~开头的文件夹）

### ~根目录
`Config/SearchConfig.config` 删除了全文检索结果配置文件中的“到动易论坛求助”字样。  
`Government/Interview/Video.aspx` 默认政府版缺少访谈视频动态页。  
`JS` 某些版本系统会丢失图片内容页需要的2个js文件。  
`UploadFiles` 替换默认丑陋的 nopic.gif。

### ~模板库-内页path在最顶部
默认模板的path的结构是：
```html
...
<div class="mainContent">
    <div class="cateHead">
        <div class="cateName"></div>
        <div class="path"></div>
    </div>
</div>
...
```
但位置栏处于最上方，占位通栏的布局也是很常见：
```html
...
<div class="cateHead">
    <div class="cateName"></div>
    <div class="path"></div>
</div>
...
<div class="mainContent"></div>
<div class="side"></div>
...
```
尽管改结构不难但是影响模板众多，稍不注意就有遗漏。因此如果有这种布局的内页则使用上面的标准模板覆盖后，再用这个目录下的文件覆盖上一步的文件即可。

### ~图片-内容页-样式2
一个做过2次的不同于默认的图片内容页，顺手就整理进来了。  
（但感觉不需要存在于这个标准初始化项目内，再考虑下要不要删除这个…………）