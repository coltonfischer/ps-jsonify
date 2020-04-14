---
title: AddProperty
parent: JSON Object Methods
grand_parent: JSON Object
nav_order: 45
---

### [](#header-3)Syntax

**AddProperty**(_name_, _property_)

### [](#header-3)Description

Use this method to add a property to the JSON Object.  If you provide an unsupported object type to `AddProperty`, then the object name string will be added to the JSON Object.  See the list of supported data types for more details.

### [](#header-3)Parameters

| Name           | Description                                                                      |
|:---------------|:---------------------------------------------------------------------------------|
| name           | Specifies the name of the property that needs to be added as a string.           |
| property       | Specifies the property to add to the JSON Object as an Any type.                 |


### [](#header-3)Returns

None.

### [](#header-3)Example

```java
Local any &aValue = "hello";
   
If Int(Rand() * 10) > 5 Then
   &aValue = True;
End-If;
   
Local PSM_JSON:Object &oObject = create PSM_JSON:Object();
   
&oObject.AddProperty("MyProperty", &aValue);
```
