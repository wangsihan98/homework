## 选择的数据集：IMDB Movies Dataset

这个数据集里共14762条数据，清洗数据（去掉信息不全的数据，去掉类别为游戏和电视节目）后，共有10822条数据。

数据集中统计了每条数据的如下性质：电影名称（words In Title）、imdb网址链接（url）、评分（imdb Rating）、打分人数（rating Count）、时长（duration）、年份（year）、类别（type）、获奖数量（nr Of Wins）、提名数量（nr Of Nominations）、照片数量（nr Of Photos）、新闻报道数量（nr Of News Articles）、用户评论数量（nr Of User Reviews）、类型数量（nr Of Genre）。后几列分别是类型的名称：Action、Adult	、Adventure、Animation、Biography、Comedy、Crime、Documentary、Drama、Family、Fantasy、Film Noir、Game Show、History、Horror、Music、Musical、Mystery、News、Reality TV、Romance、Sci-Fi、Short、Sport、Talk Show、Thriller、War、Western。

## 使用的工具、呈现和使用体会

- Hanabi

! [image] (https://github.com/wangsihan98/homework/blob/master/homework3-picture1.jpg)

我用Hanabi中的饼图呈现了IMDB中各类型的电影数量。

在使用过程中，我觉得Hanabi这款可视化工具比较简单，容易操作，但难以呈现出复杂的图表，只能导入表格，得出信息量较少的折线图、条形图、饼图、气泡图等。数据图表的呈现也较为固定，不够灵活，无法自己绘制更为美观的图表。


- 图表秀

! [image] (https://github.com/wangsihan98/homework/blob/master/homework3-picture2.png)

我用图表秀中的气泡图呈现了IMDB黑色电影（Film Noir）的评分与获奖情况，气泡的大小代表参与评分的人数。

图表秀中的图表样式比Hanabi多，简单，易操作，但其中有些模板的使用需要付费。

- Echarts





## 免费可视化图表工具

#### 纯可视化图表生成类

- Echart

一个纯Javascript的数据可视化库，百度的产品，常应用于软件产品开发或网页的统计图表模块。可在Web端高度定制可视化图表，图表种类多，动态可视化效，各类图表各类形式都完全开源免费。能处理大数据量和进行3D绘图。Echart多用于一些开发场景，它也衍生了一个0代码的图表生成器—“百度图说”，操作基本上就是选择图标，把数据复制过去，然后生成图表，保存为图或者代码嵌入。

- AntV

AntV是蚂蚁金服出品（阿里系）的一套数据可视化语法，貌似是国内第一个采用The grammar Of Graphics这套理论的可视化库。antv带有一系列的数据处理API，简单数据的数据归类，分析的能力，被很多大公司用作自己BI平台的底层工具。

- Highcharts

Highcharts同样是可视化库，只不过是国外的，商用的话需要付费。其优势是文档详细, 实例也很很详细，文档中依赖哪些js脚本，css都十分详细，学习和开发都比较省时省力，相应的产品稳定性较强。

- Hanabi

在线数据可视化图表工具，操作简单，图标多样。

- 图表秀

和Hanabi类似，在线制作图表工具，数据可视化工具。选择图表、导入数据、修改属性三步完成可视化图表。

#### 商业智能分析类

- Tableau

几乎是数据分析师人人会提的工具，内置常用的分析图表，和一些数据分析模型，可以快速的探索式数据分析，制作数据分析报告。因为是商业智能，解决的问题更偏向商业分析，用 Tableau可以快速地做出动态交互图，并且图表和配色也非常拿得出手。

- FineBI

是一款成熟的数据分析产品。内置丰富图表，不需要代码调用，可直接拖拽生成。可用于业务数据的快速分析，制作dashboard，也可构建可视化大屏。有别于Tableau的是，它更倾向于企业应用，从内置的ETL功能以及数据处理方式上看出，侧重业务数据的快速分析以及可视化展现。可与大数据平台，各类多维数据库结合，所以在企业级BI应用上广泛，个人使用免费。

- PowerBI

继Excel之后推出的BI产品，可以和Excel无缝连接使用，创建个性化的数据看板。

#### 可视化大屏类

- 阿里DataV

是阿里云的拖拽式可视化工具，主要用于业务数据与地理信息融合的大数据可视化，像一些展览中心，企业管控中心用。不需要编程，通过简单的拖拽配置就能生成可视化大屏或者仪表盘。

- FineReport

它也能做可视化报表，也能做大屏。因为后端通常连接业务系统数据，所以可以实时连接业务数据，做企业的一些经营数据展示。比如展览中心、BOSS驾驶舱，还有城市交通管控中心、交易大厅等。

- 数字冰雹

专注于做数据图像、三维处理、数据分析等相关业务，通过图像可视化方式呈现数据分析，在智慧城市、工业监控用的比较多。

#### 数据地图类

- Power Map 2016

- 地图慧

较为快速，内置的是百度地图，选择模板、上传数据、保存地图很简单的3步。

- 很多工具都能实现数据地图，比如Echarts、finereport、tableau等

#### 数据挖掘编程语言类

- R-ggplot2

- Python

- D3

D3代表数据驱动文档，是一个JavaScript库，它将任意数据绑定到文档对象模型（DOM），然后将数据驱动的转换应用于文档。尽管D3可能会更多地吸引程序员，因为这个工具涉及到代码的创建，但引人入胜的是，D3能够在网页中构建一系列真正吸引人的图表、地图、图表等。



