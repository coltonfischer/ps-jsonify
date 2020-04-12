---
title: FromJsonString
parent: JSON Array Methods
grand_parent: JSON Array
nav_order: 10
---

### [](#header-3)Syntax

**FromJsonString**(_json_string_)

### [](#header-3)Description

Use this method to populate the JSON Array from a json array represented as a string.

### [](#header-3)Parameters

| Name           | Description                                              |
|:---------------|:---------------------------------------------------------|
| json_string    | Specifies a Json array as a string.                      |


### [](#header-3)Returns

None.

### [](#header-3)Example

```java
Local string &sJsonArray;

&sJsonArray = "[ {""test"": ""hello""}, {""another"": ""obj""} ]";
Local PSM_JSON:Array &oArray = create PSM_JSON:Array();
   
&oArray.FromJsonString(&sJsonArray);
```
