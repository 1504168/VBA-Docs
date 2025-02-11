---
title: ColorFormat.BaseRGB property (Publisher)
keywords: vbapb10.chm2555906
f1_keywords:
- vbapb10.chm2555906
ms.prod: publisher
api_name:
- Publisher.ColorFormat.BaseRGB
ms.assetid: c8096661-9a5a-2769-fd88-72d38d383095
ms.date: 06/06/2019
ms.localizationpriority: medium
---


# ColorFormat.BaseRGB property (Publisher)

Returns or sets a **[PbColorType](publisher.pbcolortype.md)** constant that represents the original RGB color format before color-changing properties, such as tinting and shading, are applied. Read/write.


## Syntax

_expression_.**BaseRGB**

_expression_ A variable that represents a **[ColorFormat](Publisher.ColorFormat.md)** object.


## Return value

PbColorType



## Example

This example creates a shape, sets the fill color and lightens the color, and then creates a second shape and applies the original RGB color of the first shape to the second shape.

```vb
Sub SetBaseRGB() 
 Dim shpOne As Shape 
 
 With ActiveDocument.Pages(1).Shapes 
 Set shpOne = .AddShape(Type:=msoShapeHeart, _ 
 Left:=150, Top:=150, Width:=300, Height:=300) 
 With shpOne.Fill.ForeColor 
 .RGB = RGB(Red:=160, Green:=0, Blue:=255) 
 .TintAndShade = 0.9 
 End With 
 .AddShape(Type:=msoShapeRectangle, Left:=62, _ 
 Top:=500, Width:=488, Height:=100).Fill _ 
 .ForeColor.RGB = shpOne.Fill.ForeColor.BaseRGB 
 End With 
End Sub
```

[!include[Support and feedback](~/includes/feedback-boilerplate.md)]