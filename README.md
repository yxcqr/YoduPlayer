# YoduPlayer

一款支持 instantclick 或者 pjax 的背景音乐播放器插件（typecho博客插件）

> 1，支持自定义播放器css

> 2，支持显示歌曲名称，歌手，封面等

> 3，无 JQ，要求使用现代浏览器。

网易云歌单配置在线生成器：https://logi.im/yoduplayer.html （不保证一直有效，需要长久使用建议访问下方链接获取源码自行搭建）

源码及作者链接：https://logi.im/blog/introduction-to-major-music-plugins-for-typecho.html

感谢 @LOGI 网友提供

**注意事项：** 由于歌曲信息是存在数据库的而数据库类型为`text`，所以歌曲信息的长度是有限制的，所以建议歌曲数量不易超过200首，如果无心触发这个问题首页和插件设置页将报错此时禁用插件重新启动即可。

### 使用方法

下载压缩包, 解压，得到名为YoduPlayer的文件夹，如果不是请将文件夹重命名为YoduPlayer，之后上传到你博客中的 /usr/plugins 目录，在后台启用即可

插件后台配置歌曲格式: 
```
{title:"xxx", artist:"xxx", cover:"http:xxxx", mp3:"http:xxxx",cover:"图片地址",} ，每个歌曲之间用英文,隔开。
```
**请保证歌曲列表里至少有一首歌**！
### 夜间模式自适应
适配夜间模式需要博客启动夜间模式时给`html`或者`body`加`class="dark"`

> 项目起始于2017年，2018年05月28日停止维护，后于2022年重新开始维护

### 更新历史

> 20220331使用svg替换默认的字体图标，简化js，删除残余php代码，修复某些情况返回时歌曲列表重复生成问题，加入歌曲列表展开动画，歌曲列表字体大小调整，火狐滚动条样式适配。

> 20220328发布2.3.3版本，暂停歌曲头像停止旋转时保持当前转动角度，优化歌曲列表歌曲名字过长导致的频繁换行影响美观的问题，php相关判断代码优化，歌手名字为空时样式优化，默认封面与音乐更换。

> 20220327发布2.3.1修复切换页面后歌手名字重复输出问题。

> 2022,03,26发布2.3.0版本，去除掉yodu主题相关定制功能，去除掉皮肤系统，去除掉自动播放设置，适配夜间模式需要博客启动夜间模式时给html或者body加class=”dark“，其他细节微调整。

> 2022,03,26，去除1.6版本之后开始的jq依赖，css简单优化，支持设置顶部间距，以及采纳 @daxiyun 出错调下一首歌曲的代码
