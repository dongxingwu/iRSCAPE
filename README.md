
library(zoo)
library(Rssa)
path <- 'I:/paper2/code/iSCAPEAllMethods/'
x <- list.files(path)
for(i in 1:length(x)){
	print(i)
	source(paste0(path,x[i]))
}
##
dat <- getQ10(runif(1000,1,10),runif(1000,1,300),15,10,90,-1,0,'SSA',NULL,NULL,FALSE,FALSE)
