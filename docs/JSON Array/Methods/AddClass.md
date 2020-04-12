---
title: AddClass
parent: JSON Array Methods
grand_parent: JSON Array
nav_order: 25
---

### [](#header-3)Syntax

**AddClass**(_class_object_)

### [](#header-3)Description

Use this method to add an Application Class object to the JSON Array.

### [](#header-3)Parameters

| Name           | Description                                                                    |
|:---------------|:-------------------------------------------------------------------------------|
| class_object   | Specifies the class to add to the JSON Array as an Application Class object.   |


### [](#header-3)Returns

None.

### [](#header-3)Example

```java
Local PTPP_COLLECTIONS:Shortcut &oCref;
&oCref = create PTPP_COLLECTIONS:Shortcut(%Portal, "PT_CHANGE_PASSWORD_GBL");
   
Local PSM_JSON:Array &oArray = create PSM_JSON:Array();
   
&oArray.AddClass(&oCref);
```
