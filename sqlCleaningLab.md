### SECTION 1. 

> SELECT Accel FROM evCars

>  SELECT Accel, RTRIM(Accel, 'sec')
FROM evCars

> UPDATE evCars 
SET Accel = RTRIM(Accel, ' sec')

> SELECT Accel FROM evCars

> ALTER TABLE evCars RENAME Accel TO AccelSec

 ### SECTION 2.

 > SELECT TopSpeed, Range, Efficiency, FastCharge
FROM evCars
LIMIT 10

> SELECT TopSpeed FROM evCars;


> SELECT TopSpeed, RTRIM(TopSpeed, ' km/h')
FROM evCars


> SELECT TopSpeed FROM evCars

> UPDATE evCars
SET TopSpeed = RTRIM(Topspeed, ' km/h');

> SELECT TopSpeed FROM evCars

> SELECT TopSpeed, ROUND(TopSpeed * 0.621371, 1)
FROM evCars

> UPDATE evCars
SET TopSpeed = TopSpeed * ROUND(TopSpeed * 0.621371, 1)

> SELECT * FROM evCars

> ALTER TABLE evCars RENAME TopSpeed TO topSpeedMPH

> SELECT * FROM evCars


### SECTION 3.

> SELECT Range FROM evCars;


> SELECT Range, RTRIM(Range, ' km')
FROM evCars


> SELECT Range FROM evCars

> UPDATE evCars
SET Range = RTRIM(Range, ' km');

> SELECT Range FROM evCars

> SELECT Range, ROUND(Range * 0.621371, 1)
FROM evCars

> UPDATE evCars
SET Range = Range * ROUND(Range * 0.621371, 1)

> SELECT * FROM evCars

> ALTER TABLE evCars RENAME Range TO rangeMiles

> SELECT * FROM evCars


### SECTION 4.

> SELECT Efficiency, FastCharge FROM evCars;


> SELECT Efficiency, RTRIM(Efficiency, ' Wh/km'), FastCharge, RTRIM(FastCharge, 'km/h')
FROM evCars


> SELECT Efficiency, FastCharge FROM evCars

> UPDATE evCars
SET Efficiency = RTRIM(Efficiency, ' Wh/km'),
 FastCharge = RTRIM(FastCharge, 'km/h');

> SELECT * FROM evCars

> SELECT FastCharge, ROUND(FastCharge * 0.621371, 1)
FROM evCars

> UPDATE evCars
SET FastCharge = ROUND(FastCharge * 0.621371, 1)


> ALTER TABLE evCars 
RENAME FastCharge TO OneHourFastChargeMiles;

> ALTER TABLE evCars 
RENAME Efficiency TO efficiencyWHperKM;

> SELECT * FROM evCars


### SECTION 5.1

> SELECT RapidCharge, count(*) 
FROM evCars
GROUP BY RapidCharge

### SECTION 5.2 

> UPDATE evCars SET RapidCharge = 'TRUE'
WHERE RapidCharge = 'Rapid charging possible'

> UPDATE evCars SET RapidCharge = 'FALSE'
WHERE RapidCharge = 'Rapid charging not possible'

> SELECT RapidCharge FROM evCars;

### SECTION 5.3 

* 1.For the purpose of this exercise, if the car's RapidCharge value equals _________________ then I want you to change the value to 'Yes'

* 2.If the RapidCharge value equals _______________ then I want you to change the value to 'No'.

> UPDATE evCars
SET RapidCharge = 'Yes'
WHERE RapidCharge = 'TRUE'

> UPDATE evCars
SET RapidCharge = 'No'
WHERE RapidCharge = 'FALSE'

### SECTION 6.1

> SELECT PowerTrain, Count(*) 
FROM evCars
GROUP BY PowerTrain; 

### SECTION 6.2

If the PowerTrain equals ____41__________ then I want you to change the value to 'AWD'
If the PowerTrain equals ___37___________ then I want you to change the value to 'RWD'
If the PowerTrain equals ___25___________ then I want you to change the value to 'FWD'

### SECTION 6.3

> > UPDATE evCars 
SET PowerTrain = 'AWD'
WHERE PowerTrain = 'All Wheel Drive'

> UPDATE evCars 
SET PowerTrain = 'RWD'
WHERE PowerTrain = 'Rear Wheel Drive'

> UPDATE evCars 
SET PowerTrain = 'FWD'
WHERE PowerTrain = 'Front Wheel Drive'

### SECTION 6.4
SELECT * FROM evCars

### SECTION 7.1

 > SELECT PriceEuro, ROUND(PriceEuro * 1.09, 2)
FROM evCars

### SECTION 7.2

>  UPDATE evCars
SET PriceEuro = ROUND(PriceEuro * 1.09, 2)


### SECTION 7.3

 > ALTER TABLE evCars RENAME PriceEuro TO PriceUSD
