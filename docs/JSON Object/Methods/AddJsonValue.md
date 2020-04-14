---
title: AddJsonValue
parent: JSON Object Methods
grand_parent: JSON Object
nav_order: 80
---

### [](#header-3)Syntax

**AddJsonValue**(_name_, _json_value_)

### [](#header-3)Description

Use this method to add a JsonValue to the JSON Object.

### [](#header-3)Parameters

| Name           | Description                                                                      |
|:---------------|:---------------------------------------------------------------------------------|
| name           | Specifies the name of the Json value that needs to be added as a string.         |
| json_value     | Specifies the Json value to add to the JSON Object as a JsonValue object type.   |


### [](#header-3)Returns

None.

### [](#header-3)Example

```java
Local JsonValue &jvJson = CreateJsonValue();
&jvJson.SetString("hello");
   
Local PSM_JSON:Object &oObject = create PSM_JSON:Object();
   
&oObject.AddJsonValue("MyJsonValue", &jvJson);
```
