---
title: AddJsonObject
parent: JSON Object Methods
grand_parent: JSON Object
nav_order: 75
---

### [](#header-3)Syntax

**AddJsonObject**(_name_, _json_object_)

### [](#header-3)Description

Use this method to add a JsonObject to the JSON Object.

### [](#header-3)Parameters

| Name           | Description                                                                      |
|:---------------|:---------------------------------------------------------------------------------|
| name           | Specifies the name of the Json object that needs to be added as a string.        |
| json_object    | Specifies the Json object to add to the JSON Object as a JsonObject object type. |


### [](#header-3)Returns

None.

### [](#header-3)Example

```java
Local JsonObject &joJson = CreateJsonObject();
   
/* Populate Json Object ... */
   
Local PSM_JSON:Object &oObject = create PSM_JSON:Object();
   
&oObject.AddJsonObject("MyJsonObject", &joJson);
```
