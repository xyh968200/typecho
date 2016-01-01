# Terse

更适合程序员的typecho博客主题。

演示地址： https://biezhi.me

## 特性

* 兼容PC和手机
* 界面简洁美观
* 可配置图标和头像
* 可配置多说

## 预览

电脑：

![](http://i.imgur.com/XPPVlbF.png)

手机：

![](http://i.imgur.com/31vhhJD.png)

## 使用说明

1. 安装、启用主题

	将下载的压缩包解压，放至 `/usr/themes/` 文件夹下

2. 安装插件

	友链插件：[Links](https://github.com/biezhi/terse/releases/download/0.0.1/Links.zip)，解压放至 `/usr/plugins` 目录下

3. 修改多说评论

	在 `comments.php` 文件中修改 `{short_name:"blog-biezhi"}` 为你自己的

4. 归档页面(可选项)
	
	新建页面，选择归档页发布即可

5. 显示音乐(可选项)

	在 `header.php` 中的首页链接下方添加代码：

	```php
	<a<?php if($this->is('category', 'music')): ?> class="current"<?php endif; ?> href="<?php $this->options->siteUrl('/index.php/music'); ?>"><?php _e('音乐'); ?></a>
	```

	这里你的分类名称也要是 `music`

	添加音乐：
	
	例如：`What Are Words` 这首歌
	
	在网易云音乐的 `http://music.163.com/#/outchain/2/1210496/` 页面复制html代码即可。
	
	我这里有一个样本你只需要把歌曲id修改即可：
	
	```html
	<iframe frameborder="no" border="0" marginwidth="0" marginheight="0" width=510 height=190 src="https://music.163.com/outchain/player?type=2&id=2529311&auto=0&height=90"></iframe>
	```


## 更新日志

### v0.0.2

	1. 添加代码高亮，去除默认的代码显示
	
### v0.0.1

	1. 去除在手机显示边距
	2. 调整翻页颜色
	3. 添加音乐展示页面
