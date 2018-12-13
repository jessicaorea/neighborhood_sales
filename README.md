# neighborhood_sales
this is the one i'm using for the project 
 setwd("~/Desktop")
 DOF<-read.csv("DOF__Summary_of_Neighborhood_Sales_for_the_Bronx_for_Class_1-__2-_and_3-Family_homes_-_2009.csv")
 str(DOF)

 mu_hat1=mean(DOF$LOWEST.SALE.PRICE)
 mu_hat1
 sigma_hat1=sd(DOF$LOWEST.SALE.PRICE)
 sigma_hat1
 n=nrow(DOF)
 n
 alpha=0.05
 critical_value=qt(alpha/2,n-1)
 critical_value
 U1=mu_hat1+critical_value*sigma_hat1/sqrt(n)
 U1
 L1=mu_hat1-critical_value*sigma_hat1/sqrt(n)
 L1
 critical_value*sigma_hat1/sqrt(n)




 mu_hat2=mean(DOF$MEDIAN.SALE.PRICE)
 mu_hat2
 sigma_hat2=sd(DOF$MEDIAN.SALE.PRICE)
 sigma_hat2
 U2=mu_hat2+critical_value*sigma_hat2/sqrt(n)
 U2
 L2=mu_hat2-critical_value*sigma_hat2/sqrt(n)
 L2
 critical_value*sigma_hat2/sqrt(n)


 mu_hat3=mean(DOF$HIGHEST.SALE.PRICE)
 mu_hat3
 sigma_hat3=sd(DOF$HIGHEST.SALE.PRICE)
 sigma_hat3
 U3=mu_hat3+critical_value*sigma_hat3/sqrt(n)
 U3
 L3=mu_hat3-critical_value*sigma_hat3/sqrt(n)
 L3
 critical_value*sigma_hat3/sqrt(n)
