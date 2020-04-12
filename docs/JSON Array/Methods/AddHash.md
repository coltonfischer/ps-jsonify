---
title: AddHash
parent: JSON Array Methods
grand_parent: JSON Array
nav_order: 55
---

### [](#header-3)Syntax

**AddHash**(_hash_)

### [](#header-3)Description

Use this method to add a Hash value to the JSON Array.

### [](#header-3)Parameters

| Name           | Description                                                                    |
|:---------------|:-------------------------------------------------------------------------------|
| hash           | Specifies the hash to add to the JSON Array as a Hash type.                    |


### [](#header-3)Returns

None.

### [](#header-3)Example

```java
Local Hash &hHash = CreateHash();
&hHash.SetValue("tst", "hello");
&hHash.SetValue("val", True);
&hHash.SetValue("what", 2);
   
Local PSM_JSON:Array &oArray = create PSM_JSON:Array();
   
&oArray.AddHash(&hHash);
```
