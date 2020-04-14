---
title: AddClass
parent: JSON Object Methods
grand_parent: JSON Object
nav_order: 25
---

### [](#header-3)Syntax

**AddClass**(_name_, _class_object_)

### [](#header-3)Description

Use this method to add an Application Class object to the JSON Object.

### [](#header-3)Parameters

| Name           | Description                                                                      |
|:---------------|:---------------------------------------------------------------------------------|
| name           | Specifies the name of the class that needs to be added as a string.              |
| class_object   | Specifies the class to add to the JSON Object as an Application Class object.    |


### [](#header-3)Returns

None.

### [](#header-3)Example

```java
Local PTPP_COLLECTIONS:Shortcut &oCref;
&oCref = create PTPP_COLLECTIONS:Shortcut(%Portal, "PT_CHANGE_PASSWORD_GBL");
   
Local PSM_JSON:Object &oObject = create PSM_JSON:Object();
   
&oObject.AddClass("MyClass", &oCref);
```
