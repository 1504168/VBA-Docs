---
title: ObjectFrame.Locked property (Access)
keywords: vbaac10.chm11584
f1_keywords:
- vbaac10.chm11584
ms.prod: access
api_name:
- Access.ObjectFrame.Locked
ms.assetid: 0769b9c9-ea0b-33c8-b258-e7d775bee9e6
ms.date: 02/22/2019
ms.localizationpriority: medium
---


# ObjectFrame.Locked property (Access)

The **Locked** property specifies whether you can edit data in a control in Form view. Read/write **Boolean**.


## Syntax

_expression_.**Locked**

_expression_ A variable that represents an **[ObjectFrame](Access.ObjectFrame.md)** object.


## Remarks

The default setting of the **Locked** property is **True**. This setting allows editing, adding, and deleting data.

Use the **Locked** property to protect data in a field by making it read-only. For example, you might want a control to only display information without allowing editing, or you might want to lock a control until a specific condition is met.


## Example

The following example toggles the **Enabled** property of a command button and the **Enabled** and **Locked** properties of a control, depending on the type of employee displayed in the current record. If the employee is a manager, the **SalaryDetails** button is enabled and the **PersonalInfo** control is unlocked and enabled.

```vb
Sub Form_Current() 
 If Me!EmployeeType = "Manager" Then 
 Me!SalaryDetails.Enabled = True 
 Me!PersonalInfo.Enabled = True 
 Me!PersonalInfo.Locked = False 
 Else 
 Me!SalaryDetails.Enabled = False 
 Me!PersonalInfo.Enabled = False 
 Me!PersonalInfo.Locked = True 
 End If 
End Sub
```


[!include[Support and feedback](~/includes/feedback-boilerplate.md)]