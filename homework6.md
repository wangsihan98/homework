#### “垃圾”作业图

- 原图

![image](https://github.com/wangsihan98/homework/blob/master/homework4-picture3.jpg)

- R中做的图


- 代码




#### “未成年人犯罪”图

- 原图

![image](https://github.com/wangsihan98/homework/blob/master/homework5-picture2.png)

- R中做的图

- 代码
library(ggplot2)

setwd("D:/大学/可视化软件工具与应用/第十一周/第二张图")

datatwo <- read.csv("未成年人犯罪.csv")

View(datatwo)

pa <- ggplot(datatwo, aes(x =年份, y = 未成年人犯罪数量)) + 

  geom_line(colour = "#1d6996")
  
pa

pa +

	ggtitle("1990-2017年中国未成年人犯罪数量变化") +
	
	ylim(0, max(datatwo$未成年人犯罪数量)) +
	
	geom_point(colour ="#1d6996") +
	
	geom_vline(aes(xintercept = 2008), colour = "black",linetype = "dashed", size = 0.5) +
	
	geom_vline(aes(xintercept = 2011), colour = "black",linetype = "dashed", size = 0.5) +
	
	annotate("text", x = 2007, y = 50000, label = "2008", size = 4) +
	
	annotate("text", x = 2012, y = 37500, label = "2011", size = 4) +
	
	theme(plot.title = element_text(size = 16))
	
