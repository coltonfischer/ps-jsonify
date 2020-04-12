---
title: GetElement
parent: JSON Array Methods
grand_parent: JSON Array
nav_order: 145
---

### [](#header-3)Syntax

**GetElement**(_index_)

### [](#header-3)Description

Use this method to return the element value at the index location.

### [](#header-3)Parameters

| Name           | Description                                                                    |
|:---------------|:-------------------------------------------------------------------------------|
| index          | Specifies the index in the JSON Array as an integer.                           |


### [](#header-3)Returns

Any.

### [](#header-3)Example

```java
Local Record &rPsOptions = CreateRecord(Record.PSOPTIONS);
&rPsOptions.SelectByKey();
   
Local PSM_JSON:Array &oArray = create PSM_JSON:Array();
   
&oArray.AddRecord(&rPsOptions);
   
Local JsonObject &joJson = &oArray.GetElement(1);
```
