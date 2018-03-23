# krangl


```java
// hellp
import krangl.*

// Read data-frame from disk
val iris = DataFrame.readCSV("data/iris.txt")


// Create data-frame in memory
val df: DataFrame = dataFrameOf(
    "first_name", "last_name", "age", "weight")(
    "Max", "Doe", 23, 55,
    "Franz", "Smith", 23, 88,
    "Horst", "Keanes", 12, 82
)
```