# PixivisionDownloader
 Pixivision Illustrations Crawler And Downloader.<br>
 [Pixivision](http://www.pixivision.net/)原pixiv Spotlight，以特辑的形式展示Pixiv经典作品（包括 插画、漫画、小说等），支持日语、英语、中文（繁体·简体），共4种语言<br>
 
* 项目主要用于 Pixivision的插画特辑信息爬取和图片下载<br>
	支持图片质量：普通图和原图|大图下载<br>
      	支持以下下载方式：<br>
          1.  Pixivision插画特辑列表页<br>
          2.  Pixivision插画特辑详情页<br>
          3.  Pixiv插画url<br>
          4.  Pixiv插画ID<br>
 
* 核心配置文件__pixiv_config.py__<br>
     1.  修改__CRAWLER_HEADER__中__Accept-Language__，获取4中不同语言的特辑描述。<br>
     2.  修改__IMAGE_SVAE_BASEPATH__，指定图片存储位置。<br>
     3.  修改__IMAGE_QUALITY__，指定下载的图片质量。<br>
     4.  修改__USE_FILTER__,True时，启动RedisFilter，自动过滤重复下载的特辑，为False时会重复下载会覆盖原文件。<br>
     
~~~
python launcher.py
~~~
