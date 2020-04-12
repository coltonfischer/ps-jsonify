---
title: AddRequest
parent: JSON Array Methods
grand_parent: JSON Array
nav_order: 110
---

### [](#header-3)Syntax

**AddRequest**(_request_)

### [](#header-3)Description

Use this method to add a Request object to the JSON Array.

### [](#header-3)Parameters

| Name           | Description                                                                    |
|:---------------|:-------------------------------------------------------------------------------|
| request        | Specifies the request to add to the JSON Array as a Request object.            |


### [](#header-3)Returns

None.

### [](#header-3)Example

```java
Local PSM_JSON:Array &oArray = create PSM_JSON:Array();
   
&oArray.AddRequest(%Request);
```
