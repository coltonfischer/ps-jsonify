---
title: FromJsonString
parent: JSON Object Methods
grand_parent: JSON Object
nav_order: 10
---

### [](#header-3)Syntax

**FromJsonString**(_json_string_)

### [](#header-3)Description

Use this method to populate the JSON Object from a json object represented as a string.

### [](#header-3)Parameters

| Name           | Description                                              |
|:---------------|:---------------------------------------------------------|
| json_string    | Specifies a Json object as a string.                     |


### [](#header-3)Returns

None.

### [](#header-3)Example

```java
Local string &sJsonObject;

&sJsonObject = "{""test"": ""hello"", ""another"": ""val""}";
Local PSM_JSON:Object &oObject = create PSM_JSON:Object();
   
&oObject.FromJsonString(&sJsonObject);
```
