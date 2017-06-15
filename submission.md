###Find all rows that have an ingredient name of Brussels sprouts.
```sql
SELECT * FROM ingredients WHERE name = 'Brussels sprouts';
```
![alt](https://drive.google.com/open?id=0Bz2OPrCQMZeVTVlOZ2Y3NWtlT1U)
###With index:
![alt](https://drive.google.com/open?id=0Bz2OPrCQMZeVZmxQQ1VMVGxMWXM)

###Calculate the total count of rows of ingredients with a name of Brussels sprouts.
```sql
SELECT COUNT (*) FROM ingredients WHERE name = 'Brussels sprouts';
```
![alt](https://drive.google.com/open?id=0Bz2OPrCQMZeVblYteWhyYXNNaTQ)
###WIth index:
![alt](https://drive.google.com/open?id=0Bz2OPrCQMZeVQ21JUHpFZE5LZGc)

###Find all Brussels sprouts ingredients having a unit type of gallon(s).
```sql
SELECT * FROM ingredients WHERE unit = 'gallon(s)' AND name = 'Brussels sprouts';
```
![alt](https://drive.google.com/open?id=0Bz2OPrCQMZeVRjdWSnN0RkYtRVk)
###With index:
![alt](https://drive.google.com/open?id=0Bz2OPrCQMZeVaFRVR3BLeHktNnc)

###Find all rows that have a unit type of gallon(s), a name of Brussels sprouts or has the letter j in it.
```sql
SELECT * FROM ingredients WHERE unit ='gallon(s)' OR name = 'Brussels sprouts' OR name LIKE '%j%';
```
![alt](https://drive.google.com/open?id=0Bz2OPrCQMZeVb0poOFNUN1dCejQ)
###With index:
![alt](https://drive.google.com/open?id=0Bz2OPrCQMZeVZVFFYnVTU1RMQjA)
```sql
CREATE INDEX ON ingredients(name);
```
