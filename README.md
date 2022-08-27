# SQL-1st-KhanAcademy-project

QUESTION : Create your own store! Your store should sell one type of things, like clothing or bikes, whatever you want your store to specialize in. 
You should have a table for all the items in your store, and at least 5 columns for the kind of data you think you'd need to store.
You should sell at least 15 items, and use select statements to order your items by price and show at least one statistic about the items.

Soultion : 

CREATE TABLE Cloths(id INTEGER PRIMARY KEY, cloth_type TEXT, color TEXT , Size TEXT , quatity INTEGER , price INTEGER , aisle INTEGER);

INSERT into Cloths VALUES(1,"Tshirt","Red","M",30,500,1);
INSERT into Cloths VALUES(2,"Tshirt","Blue","S",10,300,3);
INSERT into Cloths VALUES(3,"Tshirt","Black","L",20,1000,6);
INSERT into Cloths VALUES(4,"shirt","Red","M",40,700,9);
INSERT into Cloths VALUES(5,"skirt","Blue","S",90,1000,10);
INSERT into Cloths VALUES(6,"Saree","Black","L",60,4000,1);

SELECT * FROM Cloths order by price;
SELECT aisle , SUM(price) from Cloths GROUP BY aisle;
SELECT SUM(Price)from Cloths;
