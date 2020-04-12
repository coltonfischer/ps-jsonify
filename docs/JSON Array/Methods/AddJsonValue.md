---
title: AddJsonValue
parent: JSON Array Methods
grand_parent: JSON Array
nav_order: 80
---

### [](#header-3)Syntax

**AddJsonValue**(_json_value_)

### [](#header-3)Description

Use this method to add a JsonValue to the JSON Array.

### [](#header-3)Parameters

| Name           | Description                                                                    |
|:---------------|:-------------------------------------------------------------------------------|
| json_value     | Specifies the Json value to add to the JSON Array as a JsonValue data type.    |


### [](#header-3)Returns

None.

### [](#header-3)Example

```java
Local JsonValue &jvJson = CreateJsonValue();
&jvJson.SetString("hello");
   
Local PSM_JSON:Array &oArray = create PSM_JSON:Array();
   
&oArray.AddJsonValue(&jvJson);
```
