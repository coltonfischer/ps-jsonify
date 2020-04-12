---
title: AddJsonObject
parent: JSON Array Methods
grand_parent: JSON Array
nav_order: 75
---

### [](#header-3)Syntax

**AddJsonObject**(_json_object_)

### [](#header-3)Description

Use this method to add a JsonObject to the JSON Array.

### [](#header-3)Parameters

| Name           | Description                                                                    |
|:---------------|:-------------------------------------------------------------------------------|
| json_object    | Specifies the Json object to add to the JSON Array as a JsonObject data type.  |


### [](#header-3)Returns

None.

### [](#header-3)Example

```java
Local JsonObject &joJson = CreateJsonObject();
   
/* Populate Json Object ... */
   
Local PSM_JSON:Array &oArray = create PSM_JSON:Array();
   
&oArray.AddJsonObject(&joJson);
```
