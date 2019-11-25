#### “垃圾”作业图

- 原图

![image](https://github.com/wangsihan98/homework/blob/master/homework4-picture3.jpg)

- R中做的图


- 数据

- 代码




#### “未成年人犯罪”图

- 原图

![image](https://github.com/wangsihan98/homework/blob/master/homework5-picture2.png)

- R中做的图

- 数据

- 代码
```R
	library(ggplot2)<br>
	setwd("D:/大学/可视化软件工具与应用/第十一周/第二张图")<br>
	datatwo <- read.csv("未成年人犯罪.csv")<br>
	View(datatwo)<br>
	pa <- ggplot(datatwo, aes(x =年份, y = 未成年人犯罪数量)) + <br>
  	&ensp;&ensp;geom_line(colour = "#1d6996")<br>
	pa<br>
	pa +<br>
	&ensp;&ensp;ggtitle("1990-2017年中国未成年人犯罪数量变化") +<br>
	&ensp;&ensp;ylim(0, max(datatwo$未成年人犯罪数量)) +<br>
	&ensp;&ensp;geom_point(colour ="#1d6996") +<br>
	&ensp;&ensp;geom_vline(aes(xintercept = 2008), colour = "black",linetype = "dashed", size = 0.5) +<br>
	&ensp;&ensp;geom_vline(aes(xintercept = 2011), colour = "black",linetype = "dashed", size = 0.5) +<br>
	&ensp;&ensp;annotate("text", x = 2007, y = 50000, label = "2008", size = 4) +<br>
	&ensp;&ensp;annotate("text", x = 2012, y = 37500, label = "2011", size = 4) +<br>
	&ensp;&ensp;theme(plot.title = element_text(size = 16))
```
