---
title: ToJsonString
parent: JSON Node Methods
grand_parent: JSON Node
nav_order: 60
---

### [](#header-3)Syntax

**ToJsonString**()

### [](#header-3)Description

Use this method to serialize the JSON Node to string.

### [](#header-3)Parameters

None.

### [](#header-3)Returns

String.

### [](#header-3)Example

```java
Local Exception &oException;
&oException = CreateException(0, 0, "An Error Occured");
   
Local PSM_JSON:Node &oNode = create PSM_JSON:Node();
   
&oNode.SetException(&oException);
   
Local string &sJson = &oNode.ToJsonString();
```
