---
title: SetRecord
parent: JSON Node Methods
grand_parent: JSON Node
nav_order: 35
---

### [](#header-3)Syntax

**SetRecord**(_record_value_)

### [](#header-3)Description

Use this method to set the record value of the JSON Node.

### [](#header-3)Parameters

| Name            | Description                                                                    |
|:----------------|:-------------------------------------------------------------------------------|
| record_value    | Specifies the record value of the JSON Node as a Record object.                |


### [](#header-3)Returns

None.

### [](#header-3)Example

```java
Local Record &rPsOptions = CreateRecord(Record.PSOPTIONS);
&rPsOptions.SelectByKey();
   
Local PSM_JSON:Node &oNode = create PSM_JSON:Node();
   
&oNode.SetRecord(&rPsOptions);
```
