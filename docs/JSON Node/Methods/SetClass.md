---
title: SetClass
parent: JSON Node Methods
grand_parent: JSON Node
nav_order: 15
---

### [](#header-3)Syntax

**SetClass**(_class_object_)

### [](#header-3)Description

Use this method to set the class object of the JSON Node.

### [](#header-3)Parameters

| Name           | Description                                                                    |
|:---------------|:-------------------------------------------------------------------------------|
| class_object   | Specifies the class object of the JSON Node as an App Class Object type.       |


### [](#header-3)Returns

None.

### [](#header-3)Example

```java
Local PTPP_COLLECTIONS:Shortcut &oCref;
&oCref = create PTPP_COLLECTIONS:Shortcut(%Portal, "PT_CHANGE_PASSWORD_GBL");
   
Local PSM_JSON:Node &oNode = create PSM_JSON:Node();
   
&oNode.SetClass(&oCref);
```
