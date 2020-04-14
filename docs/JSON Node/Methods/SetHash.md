---
title: SetHash
parent: JSON Node Methods
grand_parent: JSON Node
nav_order: 25
---

### [](#header-3)Syntax

**SetHash**(_hash_value_)

### [](#header-3)Description

Use this method to set the hash value of the JSON Node.

### [](#header-3)Parameters

| Name            | Description                                                                    |
|:----------------|:-------------------------------------------------------------------------------|
| hash_value      | Specifies the hash value of the JSON Node as a Hash object.                    |


### [](#header-3)Returns

None.

### [](#header-3)Example

```java
Local Hash &hHash = CreateHash();
&hHash.SetValue("tst", "hello");
&hHash.SetValue("val", True);
&hHash.SetValue("what", 2);
   
Local PSM_JSON:Node &oNode = create PSM_JSON:Node();
   
&oNode.SetHash(&hHash);
```
