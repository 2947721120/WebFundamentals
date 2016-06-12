##CN 机器翻译,请参阅EN下原版理解
＃网络基础知识<高手> [！[构建Status](https://ci.cloudware.io/api/badges/google/WebFundamentals/status.svg)](https://ci.cloudware.io/google/WebFundamentals)

`master`的分期：https://web-central.appspot.com/web/
<HR>

网页基础是多设备网的技术文档中心
发展。我们的目标是建立现代Web开发人员的资源
这是因为策划的，彻底的developer.android.com或iOS开发中心。

＃安装依赖

要构建和运行这个项目，你需要有红宝石，节点和NPM。

＃＃ 苹果电脑

1.安装[XCode的命令行工具（https://developer.apple.com/xcode/downloads/）
1.安装节点
    * [https://nodejs.org/en/](https://nodejs.org/en/）
1.安装[RVM（https://rvm.io/rubies/default）
    *`卷曲-ssl https://get.rvm.io | bash`
1.设置RVM默认为2.2.0
    *`RVM安装Ruby-2.2.0`
    *`RVM --default使用2.2.0`
1.安装[Pygments来做]（http://pygments.org/）
    *`easy_install的pygments`
1.安装打捆
    *`创业板安装bundler`
1.安装[RubyGems的（https://rubygems.org/）依赖（[杰基尔（http://jekyllrb.com/）和[Kramdown]（http://kramdown.gettalong.org/））
    *`RVM。做捆绑install`
1.安装[咕嘟咕嘟CLI（http://gulpjs.com/）
    *`NPM安装-g gulp`
1.安装[NPM（https://www.npmjs.org）的依赖
    *`NPM install`
1.下载[App Engine的SDK（https://cloud.google.com/appengine/downloads），并解压到项目的根目录内的文件夹google_appengine。将它添加到您的路径相应的（在bash，`$ PATH = / google_appengine：$ PATH`）

＃运行网站

要运行站点：

    咽

这将编译样式和JavaScript和建立与哲基尔的网站。如果多数民众赞成
所有的工作，它将开始在端口7331（你可以在到达服务器
[HTTP：//本地主机：7331 /网络/]（HTTP：//本地主机：7331 /网络/））。


对文件的任何更改将导致相应的任务一饮而尽运行。

##快速构建杰基尔

为了使运行快，您可以定义一个网站的语言和/或部分
来构建。

如果你想建立一个单一的语言，然后运行这个：

    吞掉--lang恩

如果你想建立一个特定的部分，然后运行这个：

    吞掉--section节目

这些特性结合在一起，像这样：

    吞掉--lang恩--section节目

##更多地了解和杰基尔用于液体

我们有你可以在访问资源区[https://web-central.appspot.com/web/resources/?hl=en](https://web-central.appspot.com/web/resources/?hl=en)应该让你和运行了很多定制的和有用的信息的。

＃查看上演引入请求和分支机构

**注：此功能是实验性的**。

构建过程会自动创建网站举办对所有拉请求。

要访问临时站点pull请求：

1.打开`github.com`拉请求。
2.点击**显示所有检查**。
3.单击** **详情旁边的** **生成器检查。临时网站打开
   了一个新的标签。

您也可以直接访问每一个临时网站，使用以下网址：

    https：//开头PR- <编号> -dot-weasel-dot-web-central.appspot.com

其中`<编号>`是拉入请求数。例如，该URL为
PR＃1000将是：

    https://pr-1000-dot-weasel-dot-web-central.appspot.com

上演分支机构也可在：

    <枝> -dot-weasel-dot-web-central.appspot.com

其中`<分公司>`是分支的名称。

**为引入请求和分支机构可能会更改，恕不另行通知的URL模式。**

＃翻译

参见[我们的翻译指南（TRANSLATION.md）

＃楼节目

您需要蟒蛇[谷歌API客户端（https://developers.google.com/api-client-library/python/start/installation）

对于Linux：

    PIP安装--upgrade谷歌API的Python的客户端

＃内容计划

用于Web基础内容的计划是通过GitHub的问题和我们的[网站结构+内容清单（http://goo.gl/nWDD0M）文档跟踪

＃释放状态

该项目在四月下旬推出软在2014年6月正式推出V1我们现在已经搬到了六周滚动发布周期。

＃项目结构

这是一个哲基尔版本。

```
/ AppEngine上 - 配置 - 承载静态内容服务器
/吞掉任务 - 可用的任务吞掉按责任划分（样式，脚本等）
/ src目录 - 文档
  /内容 - 在每种语言的内容
    / EN - 基本语言的文件夹。子文件夹是该网站的部分
      /基本面
      /展示
      /节目
      ...等等...
    / <langcode> - 覆盖该语言的EN结构如下。
  /杰基尔 - 
    / _config - 这些是对页面的设置定义特定的设置文件
    / _data - 这些都是静态的字符串及其翻译
    / _includes - 这一个HTML的的一些片断您可以在一个页
    / _layouts - 有你可以在你的文档的YAML参考布局
    / _plugins - 这是网络基础知识的胆量。
  /静态的
    / IMGS - 在网络基础知识使用的图像
    /脚本 - 使用Javascript - 在WF只是本地的最终部署不使用
    /风格 - 萨斯为Web基本面
    /第三方
  /测试
  /工具
```

该网站是在`/ build`，这是从来没有在检查中产生。

＃贡献

网络基础知识是一个开源项目，我们欢迎您的贡献！
提交pull请求之前，请阅读[CONTRIBUTING.md]（CONTRIBUTING.md）
并确保没有提起描述修补程序或新的内容的问题。
如果没有完成这些步骤，我们将无法接受你拉入请求，对不起。


##EN
# Web Fundamentals <master> [![Build Status](https://ci.cloudware.io/api/badges/google/WebFundamentals/status.svg)](https://ci.cloudware.io/google/WebFundamentals)

`master` staging: https://web-central.appspot.com/web/
<hr>

Web Fundamentals is a technical documentation center for multi-device web
development.  Our goal is to build a resource for modern web developers
that’s as curated and thorough as developer.android.com or iOS Dev Center.

# Installing Dependencies

To build and run this project you need to have Ruby, Node and NPM.

## Mac

1. Install [XCode Command Line Tools](https://developer.apple.com/xcode/downloads/)
1. Install node
    * [https://nodejs.org/en/](https://nodejs.org/en/)
1. Install [RVM](https://rvm.io/rubies/default)
    * `curl -sSL https://get.rvm.io | bash`
1. Set RVM Default to 2.2.0
    * `rvm install ruby-2.2.0`
    * `rvm --default use 2.2.0`
1. Install [Pygments](http://pygments.org/)
    * `easy_install pygments`
1. Install bundler
    * `gem install bundler`
1. Install [RubyGems](https://rubygems.org/) dependencies ([Jekyll](http://jekyllrb.com/) and [Kramdown](http://kramdown.gettalong.org/))
    * `rvm . do bundle install`
1. Install the [Gulp CLI](http://gulpjs.com/)
    * `npm install -g gulp`
1. Install [npm](https://www.npmjs.org) dependencies
    * `npm install`
1. Get the [App Engine SDK](https://cloud.google.com/appengine/downloads) and unzip into the google_appengine folder inside the project root. Add it to your path accordingly (in bash, `$ PATH=./google_appengine:$PATH`)

# Running the site

To run the site:

    gulp

This will compile styles & javascript and build the site with Jekyll. If thats
all working, it will start a server on port 7331 (which you can reach at
[http://localhost:7331/web/](http://localhost:7331/web/)).


Any changes to files will result in the appropriate tasks be running in gulp.

## Faster Jekyll Builds

To make the build faster you can define a language and/or section of the site
be built.

If you want to build a single language then run this:

    gulp --lang en

If you want to build a specific section then run this:

    gulp --section shows

These can be combined like so:

    gulp --lang en --section shows

## Learning More About Jekyll and Liquid Used

We have a resource area which you can access at [https://web-central.appspot.com/web/resources/?hl=en](https://web-central.appspot.com/web/resources/?hl=en) that should get you up and running with a lot of the custom and useful info.

# View staged pull requests and branches

**Note: this feature is experimental.**

The build process automatically creates staging sites for all pull requests.

To access the staging site for a pull request:

1. Open the pull request on `github.com`.
2. Click **Show All Checks**.
3. Click **Details** next to the **Builder** check. The staging site opens
   up in a new tab. 

You can also access each staging site directly, using the following URL:

    https://pr-<NUMBER>-dot-weasel-dot-web-central.appspot.com

Where `<NUMBER>` is the pull request number. For example, the URL for
PR #1000 would be:

    https://pr-1000-dot-weasel-dot-web-central.appspot.com

Staged branches are also available at:

    <branch>-dot-weasel-dot-web-central.appspot.com

Where `<branch>` is the name of the branch. 

**The URL pattern for pull requests and branches may change without notice.**

# Translations

See [our translations guide](TRANSLATION.md)

# Building Shows

You need the python [Google API client](https://developers.google.com/api-client-library/python/start/installation)

For Linux:

    pip install --upgrade google-api-python-client

# Content plan

Content plan for Web Fundamentals is tracked through GitHub Issues and our [Site Structure + Content Inventory](http://goo.gl/nWDD0M) doc

# Release status

The project was soft launched in late April with a formal v1 launch in June 2014.  We've now moved to a six-week rolling release cycle.

# Project Structure

This is a Jekyll build.

```
/appengine-config - The server to host the static content
/gulp-tasks - The tasks available to Gulp split by responsibility (styles, scripts etc.)
/src - The documentation
  /content - The content in each language
    /en - The base language folder. Sub folders are sections of the site
      /fundamentals
      /showcase
      /shows
      ...etc...
    /<langcode> - Overrides for that language, following the en structure.
  /jekyll -
    /_config - These are files which define specific settings for the setup of the page
    /_data - These are static strings and their translations
    /_includes - These a snippets of HTML you can include in a page
    /_layouts - There are layouts you can reference in the YAML of your doc
    /_plugins - This is the guts of Web Fundamentals.
  /static
    /imgs - Images used in Web Fundamentals
    /scripts - Javascript - not used in final deployment of WF only local
    /styles - Sass for web fundamentals
    /third_party
  /tests
  /tools
```

The site is generated in `/build`, which is never checked in.

# Contributing

Web Fundamentals is an open source project and we welcome your contributions!
Before submitting a pull request, please review [CONTRIBUTING.md](CONTRIBUTING.md)
and make sure that there is an issue filed describing the fix or new content.
If you don't complete these steps, we won't be able to accept your pull request, sorry.
