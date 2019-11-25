#### “垃圾”作业图

- 原图

![image](https://github.com/wangsihan98/homework/blob/master/homework4-picture3.jpg)

- R中做的图

![image](https://github.com/wangsihan98/homework/blob/master/homework6-picture1.png)

- 代码
```R
library(ggplot2)
install.packages("ggrepel")
library(ggrepel)
setwd("D:/大学/可视化软件工具与应用/第十一周/第一张图")
dataone <- read.csv("气泡图.csv")
View(dataone)
pb <- ggplot(dataone, aes(x = 居民人均消费支出增长率, y = 城市垃圾人均产生量)) +
	geom_point(aes(colour = 城市, size = 居民人均消费支出))
pb
pb + 
	ggtitle("2017年城市生活垃圾人均产生量与人均消费支出的关系") +
	theme(plot.title = element_text(size = 16)) +
	scale_size_area(max_size = 17, guide = FALSE) +
	geom_text(aes(label = 城市), size = 3) +
	xlab("居民人均消费支出增长率（单位：%）") +
	ylab("城市垃圾人均产生量（单位：千克）") +
	theme_classic() +
	theme(panel.grid.major.y = element_line(linetype = "dashed", size = 0.1, colour = "gray70"))
```

#### “未成年人犯罪”图

- 原图

![image](https://github.com/wangsihan98/homework/blob/master/homework5-picture2.png)

- R中做的图

![image](https://github.com/wangsihan98/homework/blob/master/homework6-picture2.png)

- 代码
```R
library(ggplot2)
setwd("D:/大学/可视化软件工具与应用/第十一周/第二张图")
datatwo <- read.csv("未成年人犯罪.csv")
View(datatwo)
pa <- ggplot(datatwo, aes(x = 年份, y = 未成年人犯罪数量)) + 
	geom_line(colour = "#1d6996")
pa
pa +
	ggtitle("1990-2017年中国未成年人犯罪数量变化") +
	ylab("未成年人犯罪数量（单位：人）") +
	ylim(0, max(datatwo$未成年人犯罪数量)) +
	geom_point(colour ="#1d6996") +
	geom_vline(aes(xintercept = 2008), colour = "black",linetype = "dashed", size = 0.5) +
	geom_vline(aes(xintercept = 2011), colour = "black",linetype = "dashed", size = 0.5) +
	annotate("text", x = 2007, y = 50000, label = "2008", size = 4) +
	annotate("text", x = 2012, y = 37500, label = "2011", size = 4) +
	theme(plot.title = element_text(size = 16))
```
