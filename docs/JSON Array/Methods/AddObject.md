---
title: AddObject
parent: JSON Array Methods
grand_parent: JSON Array
nav_order: 95
---

### [](#header-3)Syntax

**AddObject**(_object_)

### [](#header-3)Description

Use this method to add an Object to the JSON Array.  If you provide an unsupported object type to `AddObject`, then the object name string will be added to the JSON Array.  See the list of supported data types for more details.

### [](#header-3)Parameters

| Name           | Description                                                                    |
|:---------------|:-------------------------------------------------------------------------------|
| object         | Specifies the object to add to the JSON Array as an Object type.               |


### [](#header-3)Returns

None.

### [](#header-3)Example

```java
Local object &oValue = %Response;
   
If Int(Rand() * 10) > 5 Then
   &oValue = %Request;
End-If;
   
Local PSM_JSON:Array &oArray = create PSM_JSON:Array();
   
&oArray.AddObject(&oValue);
```
