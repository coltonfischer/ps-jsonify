---
title: SetResponse
parent: JSON Node Methods
grand_parent: JSON Node
nav_order: 40
---

### [](#header-3)Syntax

**SetResponse**(_response_value_)

### [](#header-3)Description

Use this method to set the response value of the JSON Node.

### [](#header-3)Parameters

| Name            | Description                                                                    |
|:----------------|:-------------------------------------------------------------------------------|
| response_value  | Specifies the response value of the JSON Node as a Response object.            |


### [](#header-3)Returns

None.

### [](#header-3)Example

```java
Local PSM_JSON:Node &oNode = create PSM_JSON:Node();
   
&oNode.SetResponse(%Response);
```
