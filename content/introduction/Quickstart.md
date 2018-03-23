---
title: "Quickstart"
date: 2018-03-23T08:45:25+01:00
draft: false
---

How to get started?

```kotlin
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

// Or from csv
// val otherDF = DataFrame.readCSV("path/to/file")

val newTable = df.map{ data class Foo(val name:String)}

newTable.newCol
newTable.src.x

```