---
title: Chart.PrimaryValuesAxisMinimum property (Access)
keywords: vbaac10.chm6120
f1_keywords:
- vbaac10.chm6120
ms.prod: access
api_name:
- Access.Chart.PrimaryValuesAxisMinimum
ms.date: 05/02/2018
---


# Chart.PrimaryValuesAxisMinimum property (Access)

Returns or sets the minimum value that can be represented on the primary values axis. Read/write **Single**.


## Syntax

 _expression_ . **PrimaryValuesAxisMinimum**

 _expression_ A variable that represents a **Chart** object.


## Remarks

**PrimaryValuesAxisMinimum** and **PrimaryValuesAxisMaximum** are enforced when the **PrimaryValuesAxisRange** 
property is set to **Fixed**.

A chart value may be less than the **PrimaryValuesAxisMinimum** but its representation in a chart (e.g. a bar in a 
bar chart) may be clipped according to the minimum.


## See also


#### Concepts


[PrimaryValuesAxisMaximum Property](Access.Chart.PrimaryValuesAxisMaximum.md)

[PrimaryValuesAxisRange Property](Access.Chart.PrimaryValuesAxisRange.md)

[Chart object](Access.Chart.md)