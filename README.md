# AmazonSales_DataExploration


Summary:
Data Praparation/Transformation:
- Check/Assess missing values. Removed row with missing values (2 affected rows only).
	- .isnull()
	- .dropna()
- Removed columns unnecessary to the analysis
	- .drop([])
- Changed datatypes for some columns: object to int/float datatype
	- .astype()
- Remove/Replace unnecessary string characters (that hinders datatype transformations)
	- .str.replace()

Data Exploration
Key insights taken:
1. Electronic product category was identified to be mostly rated and reviewed with maximum rating of 4.7 and minimum rating of 2.8.

2. The top 5 most expensive "Electronics" products were: TV's and Cellphone
	- Sony Bravia 164 cm (65 inches) 4K Ultra HD Sma...
	- VU 164 cm (65 inches) The GloLED Series 4K Sma...
	- LG 139 cm (55 inches) 4K Ultra HD Smart LED TV...
	- Samsung Galaxy S20 FE 5G (Cloud Navy, 8GB RAM,...
	- Samsung 138 cm (55 inches) Crystal 4K Neo Seri...
   
   
   The bottom 5 (least expensive) "Electronics" products were: Cables and small batteries
	- Gizga Essentials Spiral Cable Protector Cord S...
	- ENVIE® (AA10004PLNi-CD) AA Rechargeable Batter...
	- Panasonic CR-2032/5BE Lithium Coin Battery - P...
	- Duracell Chhota Power AA Battery Set of 10 Pcs
	- Duracell CR2016 3V Lithium Coin Battery, 5 pcs...

3. You can get "Home and Kitchen" products with high rating (atleast 4.5) for as low as 230 to as much as 24999 (in Indian Rupee).

4. Most reviewed items were:
	0	AmazonBasics Flexible Premium HDMI Cable (Blac...	426973
	1	Amazon Basics High-Speed HDMI Cable, 6 Feet (2...	426973
	2	Amazon Basics High-Speed HDMI Cable, 6 Feet - ...	426973
	3	AmazonBasics Flexible Premium HDMI Cable (Blac...	426972
	4	boAt Bassheads 100 in Ear Wired Earphones with...	363713

5. Top discounted items were:
	0	rts [2 Pack] Mini USB C Type C Adapter Plug, T...	from 4999.0		to 294.0	94%off
	1	Fire-Boltt Ninja Call Pro Plus 1.83" Smart Wat...	from 19999.0	to 1799.0	91%off
	2	Fire-Boltt Ninja Call Pro Plus 1.83" Smart Wat...	from 19999.0	to 1799.0	91%off
	3	Fire-Boltt Ninja Call Pro Plus 1.83" Smart Wat...	from 19999.0	to 1799.0	91%off
	4	Fire-Boltt Ninja Call Pro Plus 1.83" Smart Wat...	from 19999.0	to 1799.0	91%off

6. Top discounted product with atleast 100,000 rating counts and atleast 4.3 rating value were: Cables, connectors and memory storages - These are the products you would likely to confidently recommend.
0	Amazon Basics High-Speed HDMI Cable, 6 Feet (2...	78	4.4	426973
1	Samsung EVO Plus 128GB microSDXC UHS-I U3 130M...	74	4.3	140035
2	Samsung EVO Plus 128GB microSDXC UHS-I U3 130M...	71	4.3	140036
3	AmazonBasics USB 2.0 Cable - A-Male to B-Male ...	70	4.5	107687
4	AmazonBasics USB 2.0 Cable - A-Male to B-Male ...	70	4.5	107686

7. Discount precentage has minimal-to-no correlation to the rating values.
