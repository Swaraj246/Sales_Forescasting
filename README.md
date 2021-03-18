# Sales_Forescasting
Repo for forecasting sales of 1M+ products from 1000+ Stores in Python using Facebook Prophet library

There are 2 datasets: 

1) Train.csv
-> It contains dataset of 1M+ products from stores. Due to size issues that dataset can be found at the following link:
https://drive.google.com/file/d/19kPL002kcA-blh1c94M4ubgcygJsdDzA/view?usp=sharing

Description of Data:

Id: transaction ID (combination of Store and date)

Store: unique store Id

Sales: sales/day, this is the target variable

Customers: number of customers on a given day

Open: Boolean to say whether a store is open or closed (0 = closed, 1 = open)

Promo: describes if store is running a promo on that day or not

StateHoliday: indicate which state holiday (a = public holiday, b = Easter holiday, c = Christmas, 0 = None)

SchoolHoliday: indicates if the (Store, Date) was affected by the closure of public schools


2) Store.csv

StoreType: categorical variable to indicate type of store (a, b, c, d)
Assortment: describes an assortment level: a = basic, b = extra, c = extended
CompetitionDistance (meters): distance to closest competitor store
CompetitionOpenSince [Month/Year]: provides an estimate of the date when competition was open
Promo2: Promo2 is a continuing and consecutive promotion for some stores (0 = store is not participating, 1 = store is participating)
Promo2Since [Year/Week]: date when the store started participating in Promo2
PromoInterval: describes the consecutive intervals Promo2 is started, naming the months the promotion is started anew. E.g. "Feb,May,Aug,Nov" means each round starts in February, May, August, November of any given year for that store
