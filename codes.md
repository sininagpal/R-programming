R-programming
=============

practice codes
f<-function(i){
i<=10
p<-1:i
return(p)
}
///f(2) f(3)////

> p<-c(1,2,3,5,6,7,NA,NA,NA,5,6,7,3,6,7,7,9,3,7,8)
> mymatrix<-matrix(p,nrow=5,ncol=4)
> patients<-c("k", "s", "p", "h", "t")
> mydata<-data.frame(patients,mymatrix)
> cnames<- c("patient", "age", "weight", "bp","tt")
> mydata[!is.na(mydata[,3]),]
  patients X1 X2 X3 X4
1        k  1  7  6  7
5        t  6  5  7  8
> 
> mydata
  patients X1 X2 X3 X4
1        k  1  7  6  7
2        s  2 NA  7  9
3        p  3 NA  3  3
4        h  5 NA  6  7
5        t  6  5  7  8

 
 
 airquality
 summary(airquality$Ozone)
   Min. 1st Qu.  Median    Mean 3rd Qu.    Max.    NA's 
   1.00   18.00   31.50   42.13   63.25  168.00      37 
> is.na(airquality$Ozone)
> floor(3.6)
[1] 3
> ceiling(3.6)
[1] 4
> sum(is.na(airquality$Ozone))
[1] 37
> if(sum(is.na(airquality$Ozone))>=30 & sum(is.na(airquality$Solar.R))>=30){
+ p<-airquality[!is.na(airquality$Ozone) & !is.na(airquality$Solar.R),]
+ }
> P



 
for(i in 1:153){
if(sum(is.na(airquality[i,]))>1)
  {

    new<-airquality[!is.na(airquality[i,]),]
  
  }
}
for(i in 1:153){
  + kl<-c(sum(is.na(airquality[i,])))
  + print(kl)
  + }
if(kl>1){
  mydt<-airquality[!is.na(airquality[-kl,]),]
}


