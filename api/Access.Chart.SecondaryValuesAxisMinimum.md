---
title: Chart.SecondaryValuesAxisMinimum property (Access)
keywords: vbaac10.chm6121
f1_keywords:
- vbaac10.chm6121
ms.prod: access
api_name:
- Access.Chart.SecondaryValuesAxisMinimum
ms.date: 05/02/2018
---


# Chart.SecondaryValuesAxisMinimum property (Access)

Returns or sets the minimum value that can be represented on the secondary values axis. Read/write **Single**.


## Syntax

 _expression_ . **SecondaryValuesAxisMinimum**

 _expression_ A variable that represents a **Chart** object.


## Remarks

**SecondaryValuesAxisMinimum** and **SecondaryValuesAxisMaximum** are enforced when the **SecondaryValuesAxisRange** 
property is set to **Fixed**.

A chart value may be less than the **SecondaryValuesAxisMinimum** but its representation in a chart (e.g. a bar in a 
bar chart) may be clipped according to the minimum.


## See also


#### Concepts


[SecondaryValuesAxisMaximum Property](Access.Chart.SecondaryValuesAxisMaximum.md)

[SecondaryValuesAxisRange Property](Access.Chart.SecondaryValuesAxisRange.md)

[Chart object](Access.Chart.md)