# QuantJet: Financial Time Series Mining Library  <img src="https://github.com/jirotubuyaki/QuantJet/blob/master/images/jet.png" align="right" width="230px">

## Vision  
QuantJet is an open source library for monitoring and analysis financial time series in the stock market. we plan to develop functions like an advanced data manipulation and advanced statistical methods. We use C++ ad Boost C++ Library. License is MIT Licence.


## Data Object  
Data object stores financial time series data. Its object construct from an array. Its object contains Date, Open Price, High, Low , Close Price, Volume.

example	

```
  Data = new Data(data_arry);
```					
				

## Data Manipulation  
We will implement basic data manipulation functions. They are inspired from SQL, Spark. We will develop special methods for financial time series data.

example

```					
  Data_1 = Data.select(2020-01-01, 2020-04-30);
  Data_1 = Data.select(monday, 2020-01-01, 2020-04-30);

  Data_1 = Data.add(data);
  Data_1 = Data.update(2020-04-01,120);
  Data_1 = Data.delete(2020-04-01);

  Data_1.persist();
  Data_1.unpersist();
```					
				
Several other methods are planned.



## Basic Statistical Methods  
We implement basic statistical methods. We develop special methods like a Copula across Many time series datas.

example

```					
  Data_1 = Data.mean(2020-01-01, 2020-04-30);
  Data_1 = Data.var(2020-01-01, 2020-04-30);
  Data_1 = Data.corr(Data_1, Data_2);
```					
				

## Brownian Motion  
We develop Brownian motion analysis functions.

example

```					
  Data_1 = Data.brown_var(2020-01-01, 2020-04-30);
  Data_1 = Data.brown_drift(2020-01-01, 2020-04-30);
```					
				

## Jump and Regime Switch models  
We plan to implements books and academic papers below.


* Komatsu, T., & Tsuda, H. (n.d.). Saiteki toshi senryaku: Potoforio tekunoroji no riron to jissen. Asakurashoten.  

* Shreve. (2004). Stochastic Calculus Models for Finance: Volume 2: Continuous Time Models. New York, NY: Springer Verlag New York.  

## Time Series Clustering  
We plan to implements books and academic papers below.


* Nieto-Barajas, L. E., & Contreras-Cristán, A. (2014). A Bayesian Nonparametric Approach for Time Series Clustering. Bayesian Analysis, 9(1), 147-170. doi:10.1214/13-ba852  

* Müller, P. (2015). Bayesian nonparametric data analysis. Cham: Springer.  

## Contribution  
The QuantJet project welcome developers. Please see my Github pages.


## License  
 The QuantJet license is a MIT License suitable for use in both free software and proprietary applications, imposing no constraints at all on the use of the library. We use C++ and Boost C++ libraries.
