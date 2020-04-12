---
title: AddElement
parent: JSON Array Methods
grand_parent: JSON Array
nav_order: 45
---

### [](#header-3)Syntax

**AddElement**(_element_)

### [](#header-3)Description

Use this method to add an element to the JSON Array.  If you provide an unsupported object type to `AddElement`, then the object name string will be added to the JSON Array.  See the list of supported data types for more details.

### [](#header-3)Parameters

| Name           | Description                                                                    |
|:---------------|:-------------------------------------------------------------------------------|
| element        | Specifies the element to add to the JSON Array as an Any type.                 |


### [](#header-3)Returns

None.

### [](#header-3)Example

```java
Local any &aValue = "hello";
   
If Int(Rand() * 10) > 5 Then
   &aValue = True;
End-If;
   
Local PSM_JSON:Array &oArray = create PSM_JSON:Array();
   
&oArray.AddElement(&aValue);
```
