**The different between ROW_NUMBER, RANK and DENSE_RANK.**

*ROW_NUMBER*: Returns a unique number for each row starting with 1. For rows that have duplicate values,numbers are arbitarily assigned.

*Rank* : Assigns a unique number for each row starting with 1,except for rows that have duplicate values,in which case the same ranking is assigned and a gap appears in the sequence for each duplicate ranking.

*DENSE_Rank* : Assigns a unique number for each row starting with 1,except for rows that have duplicate values,in which case the same ranking is assigned and **no** gap appears in the sequence for each duplicate ranking.

Here is a example of those window funtion's results.

|ID       |RANK      |ROW_NUMBER      |DENSE_RANK|
|-------- |--------- |--------------- |--------- |
|1        |1         |1               |1         |
|1        |1         |2               |1         |
|1        |1         |3               |1         |
|2        |4         |4               |2         |
