---
title: AddJsonNode
parent: JSON Object Methods
grand_parent: JSON Object
nav_order: 70
---

### [](#header-3)Syntax

**AddJsonNode**(_name_, _json_node_)

### [](#header-3)Description

Use this method to add a JsonNode to the JSON Object.

### [](#header-3)Parameters

| Name           | Description                                                                      |
|:---------------|:---------------------------------------------------------------------------------|
| name           | Specifies the name of the Json node that needs to be added as a string.          |
| json_node      | Specifies the Json node to add to the JSON Object as a JsonNode object type.     |


### [](#header-3)Returns

None.

### [](#header-3)Example

```java
Local JsonNode &jnJson = CreateJsonNode();
   
/* Populate Json Node ... */
   
Local PSM_JSON:Object &oObject = create PSM_JSON:Object();
   
&oObject.AddJsonNode("MyJsonNode", &jnJson);
```
