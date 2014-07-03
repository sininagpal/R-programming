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

