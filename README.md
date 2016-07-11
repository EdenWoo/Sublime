# Sublime

开始使用Sublime Text：
Sublime Text有Dev版本，推荐使用，(下载地址：http://www.sublimetext.com/dev），再次提醒一下，公主号不支持外链，请将地址复制到浏览器打开。一般推荐下载便携版本（Portable version），这样拿来拿去很方便，也不用安装，而且插件和主体在一个目录下，便携。
网盘下载地址： https://yunpan.cn/OcB66ygkJ3fYCW （提取码：046c）
Sublime Text 快捷键：
Ctrl+Shift+P：打开命令面板
Ctrl+P：搜索项目中的文件
Ctrl+G：跳转到第几行
Ctrl+W：关闭当前打开文件
Ctrl+Shift+W：关闭所有打开文件
Ctrl+Shift+V：粘贴并格式化
Ctrl+D：选择单词，重复可增加选择下一个相同的单词
Ctrl+L：选择行，重复可依次增加选择下一行
Ctrl+Shift+L：选择多行
Ctrl+Shift+Enter：在当前行前插入新行
Ctrl+X：删除当前行
Ctrl+M：跳转到对应括号
Ctrl+U：软撤销，撤销光标位置
Ctrl+J：选择标签内容
Ctrl+F：查找内容
Ctrl+Shift+F：查找并替换
Ctrl+H：替换
Ctrl+R：前往 method
Ctrl+N：新建窗口
Ctrl+K+B：开关侧栏
Ctrl+Shift+M：选中当前括号内容，重复可选着括号本身
Ctrl+F2：设置/删除标记
Ctrl+/：注释当前行
Ctrl+Shift+/：当前位置插入注释
Ctrl+Alt+/：块注释，并Focus到首行，写注释说明用的
Ctrl+Shift+A：选择当前标签前后，修改标签用的
F11：全屏
Shift+F11：全屏免打扰模式，只编辑当前文件
Alt+F3：选择所有相同的词
Alt+.：闭合标签
Alt+Shift+数字：分屏显示
Alt+数字：切换打开第N个文件
Shift+右键拖动：光标多不，用来更改或插入列内容
鼠标的前进后退键可切换Tab文件
按Ctrl，依次点击或选取，可需要编辑的多个位置
按Ctrl+Shift+上下键，可替换行
Sublime Text 设置：
Setting User
以下是我使用的
"font_face": "courier new",
"font_size": 11,
"highlight_line": true,
"scroll_past_end": false,
"tab_size": 4,
"word_wrap": true
Sublime Text 插件：
建议先启用Package Control 
作用是安装插件时很方便，启用方法：菜单栏 – View – Show Console，贴入以下代码并回车，然后重启Sublime。如果你所在的网络无法启用，则无法使用，手动搜索下载去吧（话说你的网也被封了？）。
import urllib.request,os; pf = 'Package Control.sublime-package'; ipp = sublime.installed_packages_path(); 
urllib.request.install_opener( urllib.request.build_opener( 
urllib.request.ProxyHandler()) );
 open(os.path.join(ipp, pf), 'wb').write(urllib.request.urlopen( 
'http://sublime.wbond.net/' + pf.replace(' ','%20')).read()) 
 
若没有安装成功或没有显示，请使用以下方法：
第一步：下载Package Control。( https://yunpan.cn/OcB66VqwL2EB4D （提取码：da46），解压命名文件夹为Package Control。(注意大小写)
第二步：下载Package Control。（https://yunpan.cn/OcB66mqiIdHK8S （提取码：908a），解压后覆盖到刚刚的Package Control中，完成插件API函数的更新。
 第二步：打开Sublime Text 3，选择菜单：Preference-->Browse Package... 浏览插件

第三步：把package control复制到此目录，重启 Sublime text 3。
然后菜单Preferences就会多了两个Package..的东西如下： Package Control 安装成功

第四步：
点击菜单Preference-->Package Control
点击Install Package
 
等待几秒后再弹出如下内容，敲键盘emmet，选择如下：

在 Emmet 安装完成后，会显示如下屏幕：然后会自动安装PyV8，安装完成，重启 Sublime Text 3。

至此emmet插件安装完成。
搜索框没有emmet相关内容，手动把emmet插件放入第二步打开的文件夹，emmet插件下载>>


开始安装一些其他非常实用的插件吧，Ctrl+Shift+P（菜单 – Tools – Command Paletter），输入 install 选中Install Package并回车，输入或选择你需要的插件回车就安装了（注意左下角的小文字变化，会提示安装成功），安装其它插件也是这个方法，非常快速。
ZenCoding
不得不用的一款前端开发方面的插件，Write less , show more.安装后可直接使用，Tab键触发，Alt+Shift+W是个代码机器。
Alignment
代码对齐，如写几个变量，选中这几行，Ctrl+Alt+A，哇，齐了。
Prefixr
写 CSS可自动添加 -webkit 等私有词缀，Ctrl+Alt+X触发。
Tag
Html格式化，右键Auto-Format Tags on Ducument。
Clipboard History
剪贴板历史记录，显示更多历史复制，Ctrl+Shift+V触发。
SideBarEnhancements
侧栏右键功能增强，非常实用
Theme – Soda
完美的编码主题，用过的都说好，Setting user里面添加”theme”: “Soda Dark.sublime-theme”
GBK to UTF8
将文件编码从GBK转黄成UTF8，菜单 – File里面找
SFTP
直接编辑 FTP 或 SFTP 服务器上的文件，绝对FTP浮云
WordPress
集成一些WordPress的函数，对于像我这种经常要写WP模版和插件的人特别有用
PHPTidy
整理排版PHP代码
YUI Compressor
压缩JS和CSS文件
 
Sublime Prefixr
Prefixr，CSS3 私有前缀自动补全插件，显然也很有用哇
JS Format
一个JS代码格式化插件。
SublimeLinter
一个支持lint语法的插件，可以高亮linter认为有错误的代码行，也支持高亮一些特别的注释，比如“TODO”，这样就可以被快速定位。（IntelliJ IDEA的TODO功能很赞，这个插件虽然比不上，但是也够用了吧）
Placeholders
故名思意，占位用，包括一些占位文字和HTML代码片段，实用。
Sublime Alignment
用于代码格式的自动对齐。传说最新版Sublime 已经集成。

Clipboard History
粘贴板历史记录，方便使用复制/剪切的内容。
DetectSyntax
这是一个代码检测插件。
Nettuts Fetch
如果你在用一些公用的或者开源的框架，比如 Normalize.css或者modernizr.js，但是，过了一段时间后，可能该开源库已经更新了，而你没有发现，这个时候可能已经不太适合你的项目了，那么你就要重新折腾一遍或者继续用陈旧的文件。Nettuts Fetch可以让你设置一些需要同步的文件列表，然后保存更新。

JsMinifier
该插件基于Google Closure compiler，自动压缩js文件。
Sublime CodeIntel
代码自动提示
Bracket Highlighter
类似于代码匹配，可以匹配括号，引号等符号内的范围。

Hex to HSL
自动转换颜色值，从16进制到HSL格式，快捷键 Ctrl+Shift+U

GBK to UTF8
将文件编码从GBK转黄成UTF8，快捷键Ctrl+Shift+C
Git
该插件基本上实现了git的所有功能。
