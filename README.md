# DSG_drybean
A  detailed analysis of dry bean data set. At first, a new data set is copied from original data set to protect it from any damage or alteration. Then, a new column `color_code` is added in alphatical order for 
each bean type. This makes the analysis of class based on other variable more easy and accurate.

| Bean class | color_code |
|------------|------------|
|BARBUNYA|0|
|BOMBAY|1|
|CALI|2|
|DERMASON|3|
|HOROZ|4|
|SEKER|5|
|SIRA|6|

## Data summary
Int64Index: 13543 entries, 0 to 13610.\
Data columns (total 18 columns):

|    | Column         |  Non-Null Count | Dtype |          
|--- | ------         | --------------  |  -----|  
| 0  | Area           | 13543 non-null  |int64  |
| 1  | Perimeter      |  13543 non-null |float64|
| 2  | MajorAxisLength| 13543 non-null  |float64|
| 3  | MinorAxisLength|  13543 non-null |float64|
| 4  | AspectRation   |  13543 non-null |foat64 |
| 5  | Eccentricity   |  13543 non-null |foat64 |
| 6  | ConvexArea     |  13543 non-null |int64  |
| 7  | EquivDiameter  |  13543 non-null |float64|
| 8  | Extent         |  13543 non-null |float64|
| 9  | Solidity       |  13543 non-null |float64|
| 10 | roundness      |  13543 non-null |float64|
| 11 | Compactness    |  13543 non-null |float64|
| 12 | ShapeFactor1   |  13543 non-null |float64|
| 13 | ShapeFactor2   |  13543 non-null |float64|
| 14 | ShapeFactor3   |  13543 non-null |float64|
| 15 | ShapeFactor4   |  13543 non-null |float64|
| 16 | Class          |  13543 non-null |object |
| 17 | Color_code     |  13543 non-null |int64  |

dtypes: float64(14), int64(3), object(1)\
memory usage: 2.0+ MB

## Univariate Analysis

### 1. Numerical analysis
|  |Area|	Perimeter|	MajorAxisLength| MinorAxisLength|	AspectRation|	Eccentricity|	ConvexArea|	EquivDiameter|Extent|Solidity|roundness|Compactness|ShapeFactor1|ShapeFactor2|ShapeFactor3|ShapeFactor4|Color_code|
|--|---|-----------|-----------------|----------------|-------------|-------------|-----------|--------------|------|--------|---------|-----------|------------|------------|------------|------------|----------|
|count|13543.000000|13543.000000|13543.000000|13543.000000|13543.000000|13543.000000|13543.000000|13543.000000|13543.000000|13543.000000|13543.000000|13543.000000|13543.000000|13543.000000|13543.000000|13543.000000|13543.000000|
|mean|	53048.460385|	854.993406|	319.895602|	202.365321|	1.581075|	0.750315|	53767.986709|	253.034094|	0.749829|	0.987152|	0.873671|	0.800352|	0.006561|	0.001719|	0.644341|0.995078|3.530311|
|std|	29392.438324|	214.722684|	85.809260|	45.051632|	0.245245|	0.091858|	29844.248525|	59.307709|	0.048939|	0.004650|	0.059393|	0.061464|	0.001130|	0.000595|	0.098653|	0.004347|1.832994|
|min|	20420.000000|	524.736000|	183.601165|	122.512653|	1.024868|	0.218951|	20684.000000|	161.243764|	0.555315|	0.919246|	0.489618|	0.640577|	0.002778|	0.000564|	0.410339|	0.947687|0.000000|
|25%|	36282.500000|	703.230000|	253.086806|	175.886357|	1.430662|	0.715144|	36673.000000|	214.933277|	0.718735|	0.985678|	0.833410|	0.763228|	0.005893|	0.001158|	0.582517|	0.993720|2.000000|
|50%|	44580.000000|	793.896000|	296.404589|	192.491117|	1.549860|	0.763997|	45122.000000|	238.245711|	0.759903|	0.988288|	0.883490|	0.801514|	0.006643|	0.001700|	0.642424|	0.996393|3.000000|
|75%|	61382.000000|	977.146500|	376.312489|	217.245403|	1.703916|	0.809671|	62360.000000|	279.560351|	0.786849|	0.990019|	0.917031|	0.834470|	0.007270|	0.002173|	0.696341|	0.997891|5.000000|
|max|	254616.000000|	1985.370000|	738.860153|	460.198497|	2.430306|	0.911423|	263261.000000|	569.374358|	0.866195|	0.994677|	0.990685|	0.987303|	0.010451|	0.003665|	0.974767|	0.999733|6.000000|

### 2. Pie chart
![piechart](https://user-images.githubusercontent.com/62436345/114299359-54211600-9ad8-11eb-929a-1988c9df00a3.png)

### 3. Histograph
![histogram](https://user-images.githubusercontent.com/62436345/114299406-892d6880-9ad8-11eb-9a61-d9796e99e110.png)

## Bivariate analysis

### 1. Correlation matrix
![correlation matrix](https://user-images.githubusercontent.com/62436345/114299442-dc9fb680-9ad8-11eb-9cff-50f73d310724.png)

### 2. Scatterplot(Perimeter v/s Area)
![scatterplot](https://user-images.githubusercontent.com/62436345/114299488-1ec8f800-9ad9-11eb-9ebf-5d3b3e3994e1.png)

### 3. Boxplot(Area)
![boxplot](https://user-images.githubusercontent.com/62436345/114299524-5d5eb280-9ad9-11eb-8c5b-c2abfc61bff2.png)
