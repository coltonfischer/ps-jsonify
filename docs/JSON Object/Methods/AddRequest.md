---
title: AddRequest
parent: JSON Object Methods
grand_parent: JSON Object
nav_order: 110
---

### [](#header-3)Syntax

**AddRequest**(_name_, _request_)

### [](#header-3)Description

Use this method to add a Request object to the JSON Object.

### [](#header-3)Parameters

| Name           | Description                                                                      |
|:---------------|:---------------------------------------------------------------------------------|
| name           | Specifies the name of the request that needs to be added as a string.            |
| request        | Specifies the request to add to the JSON Object as a Request object.             |


### [](#header-3)Returns

None.

### [](#header-3)Example

```java
Local PSM_JSON:Object &oObject = create PSM_JSON:Object();
   
&oObject.AddRequest("MyRequest", %Request);
```
