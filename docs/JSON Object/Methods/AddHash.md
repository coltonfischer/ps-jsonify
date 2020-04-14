---
title: AddHash
parent: JSON Object Methods
grand_parent: JSON Object
nav_order: 55
---

### [](#header-3)Syntax

**AddHash**(_name_, _hash_)

### [](#header-3)Description

Use this method to add a Hash value to the JSON Object.

### [](#header-3)Parameters

| Name           | Description                                                                      |
|:---------------|:---------------------------------------------------------------------------------|
| name           | Specifies the name of the hash that needs to be added as a string.               |
| hash           | Specifies the hash to add to the JSON Object as a Hash type.                     |


### [](#header-3)Returns

None.

### [](#header-3)Example

```java
Local Hash &hHash = CreateHash();
&hHash.SetValue("tst", "hello");
&hHash.SetValue("val", True);
&hHash.SetValue("what", 2);
   
Local PSM_JSON:Object &oObject = create PSM_JSON:Object();
   
&oObject.AddHash("MyHash", &hHash);
```
