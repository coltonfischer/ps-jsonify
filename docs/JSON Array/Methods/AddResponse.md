---
title: AddResponse
parent: JSON Array Methods
grand_parent: JSON Array
nav_order: 105
---

### [](#header-3)Syntax

**AddResponse**(_response_)

### [](#header-3)Description

Use this method to add a Response object to the JSON Array.

### [](#header-3)Parameters

| Name           | Description                                                                    |
|:---------------|:-------------------------------------------------------------------------------|
| response       | Specifies the response to add to the JSON Array as a Response object.          |


### [](#header-3)Returns

None.

### [](#header-3)Example

```java
Local PSM_JSON:Array &oArray = create PSM_JSON:Array();
   
&oArray.AddResponse(%Response);
```
