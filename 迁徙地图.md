library(devtools)
#install_github('lchiffon/REmap')
library(REmap)
Sys.setlocale("LC_CTYPE","English_United Kingdom.1252")
set.seed(125)
origin = rep("北京",10)
destination = c('上海','广州','大连','南宁','南昌',
                '拉萨','长春','包头','重庆','常州')
dat = data.frame(origin,destination)
out = remap(dat,title = "REmap绘制迁徙地图",subtitle = "theme:Dark")
out
