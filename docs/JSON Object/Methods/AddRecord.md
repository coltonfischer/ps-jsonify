---
title: AddRecord
parent: JSON Object Methods
grand_parent: JSON Object
nav_order: 100
---

### [](#header-3)Syntax

**AddRecord**(_name_, _record_)

### [](#header-3)Description

Use this method to add a Record object to the JSON Object.

### [](#header-3)Parameters

| Name           | Description                                                                      |
|:---------------|:---------------------------------------------------------------------------------|
| name           | Specifies the name of the record that needs to be added as a string.             |
| record         | Specifies the record to add to the JSON Object as a Record object.               |


### [](#header-3)Returns

None.

### [](#header-3)Example

```java
Local Record &rPsOptions = CreateRecord(Record.PSOPTIONS);
&rPsOptions.SelectByKey();
   
Local PSM_JSON:Object &oObject = create PSM_JSON:Object();
   
&oObject.AddRecord("PSOPTIONS", &rPsOptions);
```
