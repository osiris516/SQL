# SQL
SQL Portfolio

--CREATE a Candy Store DataBase

CREATE TABLE Candy_Store(id INTEGER PRIMARY KEY, item TEXT, price INTEGER, quantity INTEGER, total_sold INTEGER);

INSERT INTO Candy_Store VALUES (1,"M&M",0.98,34,11);
INSERT INTO Candy_Store VALUES (2,"Skittles",0.75,65,17);
INSERT INTO Candy_Store VALUES (3,"Hersheys",0.65,72,81);
INSERT INTO Candy_Store VALUES (4,"Starburst",0.50,54,41);
INSERT INTO Candy_Store VALUES (5,"Fishes",1.25,81,34);
INSERT INTO Candy_Store VALUES (6,"Twislers",2.99,10,2);
INSERT INTO Candy_Store VALUES (7,"Airheads",0.65,12,5);
INSERT INTO Candy_Store VALUES (8,"Gummiebears",1.50,57,34);
INSERT INTO Candy_Store VALUES (9,"KitKat",1.05,24,12);
INSERT INTO Candy_Store VALUES (10,"kisses",0.35,89,52);
INSERT INTO Candy_Store VALUES (11,"Gummieworms",1.85,92,61);
INSERT INTO Candy_Store VALUES (12,"Reeses",0.55,43,18);
INSERT INTO Candy_Store VALUES (13,"Snickers",1.75,78,24);
INSERT INTO Candy_Store VALUES (14,"LifeSavers",1.99,54,53);
INSERT INTO Candy_Store VALUES (15,"JollyRanchers",0.25,95,9);

Display the DATE order by price.
SELECT * FROM Candy_Store
ORDER BY price DESC;

What are the 3 most sold items 
SELECT item, price, sold 
FROM Candy_Store
ORDER BY total_sold DESC
LIMIT 3;
