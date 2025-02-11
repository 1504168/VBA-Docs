---
title: Form.ActiveControl property (Access)
keywords: vbaac10.chm13493
f1_keywords:
- vbaac10.chm13493
ms.prod: access
api_name:
- Access.Form.ActiveControl
ms.assetid: 0bb3cac4-fc88-cdd3-6bc4-1057b02d4eb5
ms.date: 03/09/2019
ms.localizationpriority: medium
---


# Form.ActiveControl property (Access)

Use the **ActiveControl** property together with the **[Screen](Access.Screen.md)** object to identify or refer to the control that has the focus. Read-only **Control** object.


## Syntax

_expression_.**ActiveControl**

_expression_ A variable that represents a **[Form](Access.Form.md)** object.


## Remarks

This property setting contains a reference to the **Control** object that has the focus at run time.

Use the **ActiveControl** property to refer to the control that has the focus at run time together with one of its properties or methods. The following example assigns the name of the control with the focus to the `strControlName` variable.

```vb
Dim ctlCurrentControl As Control 
Dim strControlName As String 
Set ctlCurrentControl = Screen.ActiveControl 
strControlName = ctlCurrentControl.Name
```

If no control has the focus when you use the **ActiveControl** property, or if all of the active form's controls are hidden or disabled, an error occurs.


## Example

The following example assigns the active control to the `ctlCurrentControl` variable, and then takes different actions depending on the value of the control's **Name** property.

```vb
Dim ctlCurrentControl As Control 
 
Set ctlCurrentControl = Screen.ActiveControl 
If ctlCurrentControl.Name = "txtCustomerID" Then 
 . 
 . ' Do something here. 
 . 
ElseIf ctlCurrentControl.Name = "btnCustomerDetails" Then 
 . 
 . ' Do something here. 
 . 
End If
```




[!include[Support and feedback](~/includes/feedback-boilerplate.md)]
