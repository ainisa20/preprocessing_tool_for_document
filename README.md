## RAG文档预处理小工具

1、总体流程

先将PDF文档转换为html格式文件（可以100%还原），然后通过爬虫工具将内容转为markdown格式，图片会自动转为URL链接，同时支持负责的页面样式，如分块的论文格式、文章中的表格等，通过该方式预处理后可以得到效果极佳的.md文档

2、软件安装

2.1 pdf2htmlEX下载和安装

地址：https://github.com/pdf2htmlEX/pdf2htmlEX/releases

版本：pdf2htmlEX-0.18.8.rc1-master-20200630-Ubuntu-bionic-x86_64.deb

安装命令：
-- 方式1:本地安装，系统ubuntu20.04
sudo apt install ./pdf2htmlEX-0.18.8.rc1-master-20200630-Ubuntu-bionic-x86_64.deb

 sudo dpkg -i pdf2htmlEX-0.18.8.rc1-master-20200630-Ubuntu-bionic-x86_64.deb
 
  apt-get install -f

-- 方式2:docker 安装
docker pull bwits/pdf2htmlex

2.2、firecrawl 下载和安装

地址：https://github.com/mendableai/firecrawl/blob/main/CONTRIBUTING.md
同样推荐用docker安装

firecrawl在线体验地址：https://www.firecrawl.dev/

jina在线体验地址：https://jina.ai/reader/


2.3、PDF转换与内容提取系统

简单代码仓代码
