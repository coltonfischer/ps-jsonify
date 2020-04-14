---
title: AddResponse
parent: JSON Object Methods
grand_parent: JSON Object
nav_order: 105
---

### [](#header-3)Syntax

**AddResponse**(_name_, _response_)

### [](#header-3)Description

Use this method to add a Response object to the JSON Object.

### [](#header-3)Parameters

| Name           | Description                                                                      |
|:---------------|:---------------------------------------------------------------------------------|
| name           | Specifies the name of the response that needs to be added as a string.           |
| response       | Specifies the response to add to the JSON Object as a Response object.           |


### [](#header-3)Returns

None.

### [](#header-3)Example

```java
Local PSM_JSON:Object &oObject = create PSM_JSON:Object();
   
&oObject.AddResponse("MyResponse", %Response);
```
