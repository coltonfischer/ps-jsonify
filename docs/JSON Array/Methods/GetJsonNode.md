---
title: GetJsonNode
parent: JSON Array Methods
grand_parent: JSON Array
nav_order: 150
---

### [](#header-3)Syntax

**GetJsonNode**(_index_)

### [](#header-3)Description

Use this method to return the JsonNode at the index location.

### [](#header-3)Parameters

| Name           | Description                                                                    |
|:---------------|:-------------------------------------------------------------------------------|
| index          | Specifies the index in the JSON Array as an integer.                           |


### [](#header-3)Returns

JsonNode.

### [](#header-3)Example

```java
Local any &aValue = "hello";
   
If Int(Rand() * 10) > 5 Then
   &aValue = CreateArrayAny("test", True, 6, Null);
End-If;
   
Local PSM_JSON:Array &oArray = create PSM_JSON:Array();
   
&oArray.AddElement(&aValue);
   
Local JsonNode &jnJson = &oArray.GetJsonNode(1);
/* Evaluate JsonNode ... */
```
