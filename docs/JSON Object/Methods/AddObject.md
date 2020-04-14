---
title: AddObject
parent: JSON Object Methods
grand_parent: JSON Object
nav_order: 95
---

### [](#header-3)Syntax

**AddObject**(_name_, _object_)

### [](#header-3)Description

Use this method to add an Object to the JSON Object.  If you provide an unsupported object type to `AddObject`, then the object name string will be added to the JSON Object.  See the list of supported data types for more details.

### [](#header-3)Parameters

| Name           | Description                                                                      |
|:---------------|:---------------------------------------------------------------------------------|
| name           | Specifies the name of the object that needs to be added as a string.             |
| object         | Specifies the object to add to the JSON Object as an Object type.                |


### [](#header-3)Returns

None.

### [](#header-3)Example

```java
Local object &oValue = %Response;
   
If Int(Rand() * 10) > 5 Then
   &oValue = %Request;
End-If;
   
Local PSM_JSON:Object &oObject = create PSM_JSON:Object();
   
&oObject.AddObject("TheRequestOrResponse", &oValue);
```
