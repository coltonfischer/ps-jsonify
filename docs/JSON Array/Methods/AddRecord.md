---
title: AddRecord
parent: JSON Array Methods
grand_parent: JSON Array
nav_order: 100
---

### [](#header-3)Syntax

**AddRecord**(_record_)

### [](#header-3)Description

Use this method to add a Record object to the JSON Array.

### [](#header-3)Parameters

| Name           | Description                                                                    |
|:---------------|:-------------------------------------------------------------------------------|
| record         | Specifies the record to add to the JSON Array as a Record object.              |


### [](#header-3)Returns

None.

### [](#header-3)Example

```java
Local Record &rPsOptions = CreateRecord(Record.PSOPTIONS);
&rPsOptions.SelectByKey();
   
Local PSM_JSON:Array &oArray = create PSM_JSON:Array();
   
&oArray.AddRecord(&rPsOptions);
```
