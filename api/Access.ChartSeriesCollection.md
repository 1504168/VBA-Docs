---
title: ChartSeriesCollection Object (Access)
keywords: vbaac10.chm14751
f1_keywords:
- vbaac10.chm14751
ms.prod: access
api_name:
- Access.ChartSeriesCollection
ms.date: 05/02/2018
---


# ChartSeriesCollection Object (Access)

A collection of all the **[ChartSeries](Access.ChartSeries.md)** objects in the specified chart.


## Using ChartSeriesCollection

The following example displays the name of each **ChartSeries** instance in a collection.

```vb
With myChart
 For Each series In .ChartSeriesCollection
  MsgBox (series.Name)
 Next
End With
```

## See also

- [Chart object](Access.Chart.md)