---
title: GetProperty
parent: JSON Object Methods
grand_parent: JSON Object
nav_order: 145
---

### [](#header-3)Syntax

**GetProperty**(_name_)

### [](#header-3)Description

Use this method to return the property value mentioned by the input parameter.

### [](#header-3)Parameters

| Name           | Description                                                                    |
|:---------------|:-------------------------------------------------------------------------------|
| name           | Specifies the name of the property value as a string                           |


### [](#header-3)Returns

Any.

### [](#header-3)Example

```java
Local Record &rPsOptions = CreateRecord(Record.PSOPTIONS);
&rPsOptions.SelectByKey();
   
Local PSM_JSON:Object &oObject = create PSM_JSON:Object();
   
&oObject.AddRecord("Rec", &rPsOptions);
   
Local JsonObject &joJson = &oObject.GetProperty("Rec");
```
