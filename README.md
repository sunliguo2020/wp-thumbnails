# WP-Thumbnails

WordPress 缩略图插件，支持 PHP 8+。

## 插件特色

- **自动提取文章图片**：自动扫描文章内容，提取图片并生成缩略图
- **多种显示方式**：
  - **首页缩略图**：在首页、分类页、标签页、搜索页自动显示文章缩略图
  - **全排列缩略图**：将文章内所有图片以缩略图形式排列显示
  - **智能模式**：根据图片数量自动选择单张或多张显示
  - **随机缩略图**：显示随机文章的缩略图
  - **相关缩略图**：根据标签相关性显示相关文章的缩略图
  - **分类缩略图**：显示指定分类下的文章缩略图
  - **标签缩略图**：显示指定标签下的文章缩略图
  - **热门缩略图**：根据访客点击数显示最热门文章的缩略图（需 WP-PostViews 插件）
- **外链图片支持**：自动下载远程图片到本地并生成缩略图，支持 Picasa、Flickr、Yupoo 等相册
- **视频缩略图**：支持优酷、酷6、土豆三大视频网站的缩略图提取
- **远程图片本地化**：自动将文章中的远程图片替换为本地图片
- **文章短代码**：通过 shortcode 将缩略图插入到文章中的任意位置
- **摘要截断**：自动截断文章摘要，支持自定义摘要长度和结尾文字
- **高度可定制**：后台提供丰富的设置选项，包括尺寸、裁剪方式、显示位置、链接目标等
- **PHP 8+ 兼容**：已修复所有 PHP 8+ 兼容性问题

## 安装

1. 将插件上传到 /wp-content/plugins/ 目录
2. 在 WordPress 后台启用插件
3. 进入 设置 → WP-Thumbnails 进行配置

## 调用代码

`php
// 首页缩略图（单张）
<?php if(function_exists('wp_thumbnails_for_homepage')) { wp_thumbnails_for_homepage(); } ?>

// 全排列缩略图（多张）
<?php if(function_exists('wp_thumbnails_for_single_post')) { wp_thumbnails_for_single_post(); } ?>

// 智能模式
<?php if(function_exists('wp_thumbnails_for_smart_homepage')) { wp_thumbnails_for_smart_homepage(); } ?>

// 随机缩略图
<?php if(function_exists('wp_thumbnails_for_random_posts')) { wp_thumbnails_for_random_posts(); } ?>

// 最新缩略图
<?php if(function_exists('wp_thumbnails_for_recent_posts')) { wp_thumbnails_for_recent_posts(); } ?>

// 相关缩略图
<?php if(function_exists('wp_thumbnails_for_related_posts')) { wp_thumbnails_for_related_posts(); } ?>

// 分类缩略图
<?php if(function_exists('wp_thumbnails_for_category')) { wp_thumbnails_for_category(); } ?>

// 热门缩略图
<?php if(function_exists('wp_thumbnails_for_popular_posts')) { wp_thumbnails_for_popular_posts(); } ?>

// 标签缩略图
<?php if(function_exists('wp_thumbnails_for_tag')) { wp_thumbnails_for_tag(); } ?>
`

## 更新日志

详见 [CHANGELOG.md](CHANGELOG.md)

## 作者

- **布谷鸟** (9000birds@gmail.com)
- 插件主页：[http://niaolei.org.cn/wp-thumbnails](http://niaolei.org.cn/wp-thumbnails)
- 鸟类网：[http://niaolei.org.cn/](http://niaolei.org.cn/)
