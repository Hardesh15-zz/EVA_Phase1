## Calculation for RF # 224 * 224
<b>N(output)</b> = ( ( N(input) + 2 * (Padding) - K )/S ) + 1 <br>
<b>RF(output)</b> = RF(input) + (K-1) * Jump(input) <br>
<b>Jump(output)</b> = Jump(input) * Stride

|  Layer  | K,P,S  | Input|Output| RF             |  Jump    |
| ------  | ------ |------|------|--------------  |--------- |
|Conv     | 7,0,2  |224   |110   | 3              | 1        |
|MaxPool  | 3,0,2  |110   |55    |3+(7-1)* 1 = 9 |1 * 2 = 2 |
|Conv     | 3,0,1  |55    |53    |9+(3-1)* 2 = 13|2 * 2 = 4 |
|MaxPool  | 3,0,2  |53    |27    |13+(3-1)* 4 =21|4 * 1 = 4 |
|MaxPool  | 3,0,2  |27    |14    |21+(3-1)* 4 =29|4 * 2 = 8 |
|MaxPool  | 3,0,2  |14    |07    |29+(3-1)* 8 =45 |8 * 2 = 16|
|Avg.Pool | 7,0,1  |07    |00    |45+(3-1)* 16 =77|16 * 2 = 32|
|         |        |00    |00    |77+(7-1)* 32 =269|32 * 1 = 32|
<br>
<i>Note- Considering 0.5 value as 1.
