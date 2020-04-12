---
title: AddJsonNode
parent: JSON Array Methods
grand_parent: JSON Array
nav_order: 70
---

### [](#header-3)Syntax

**AddJsonNode**(_json_node_)

### [](#header-3)Description

Use this method to add a JsonNode to the JSON Array.

### [](#header-3)Parameters

| Name           | Description                                                                  |
|:---------------|:-----------------------------------------------------------------------------|
| json_node     | Specifies the Json node to add to the JSON Array as a JsonNode data type.     |


### [](#header-3)Returns

None.

### [](#header-3)Example

```java
Local JsonNode &jnJson = CreateJsonNode();
   
/* Populate Json Node ... */
   
Local PSM_JSON:Array &oArray = create PSM_JSON:Array();
   
&oArray.AddJsonNode(&jnJson);
```
