---
title: GetJsonNode
parent: JSON Object Methods
grand_parent: JSON Object
nav_order: 155
---

### [](#header-3)Syntax

**GetJsonNode**(_name_)

### [](#header-3)Description

Use this method to return the Json node mentioned by the input parameter from the JSON Object.

### [](#header-3)Parameters

| Name           | Description                                                                    |
|:---------------|:-------------------------------------------------------------------------------|
| name           | Specifies the name of the Json node as a string                                |


### [](#header-3)Returns

JsonNode.

### [](#header-3)Example

```java
Local any &aValue = "hello";
   
If Int(Rand() * 10) > 5 Then
    &aValue = True;
End-If;
   
Local PSM_JSON:Object &oObject = create PSM_JSON:Object();
   
&oObject.AddProperty("MyProperty", &aValue);
   
Local JsonNode &joJson = &oObject.GetJsonNode("MyProperty");
/* Evaluate &joJson.GetValueType() for type ... */
```
