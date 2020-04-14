---
title: FromJsonObject
parent: JSON Object Methods
grand_parent: JSON Object
nav_order: 5
---

### [](#header-3)Syntax

**FromJsonObject**(_json_object_)

### [](#header-3)Description

Use this method to populate the JSON Object from an existing JsonObject object.

### [](#header-3)Parameters

| Name           | Description                                                                      |
|:---------------|:---------------------------------------------------------------------------------|
| json_object    | Specifies the Json object as a JsonObject object.                                |


### [](#header-3)Returns

None.

### [](#header-3)Example

```java
Local JsonObject &joJson = CreateJsonObject();
   
/* Populate JsonObject ... */
   
Local PSM_JSON:Object &oObject = create PSM_JSON:Object();
&oObject.FromJsonObject(&joJson);
```
