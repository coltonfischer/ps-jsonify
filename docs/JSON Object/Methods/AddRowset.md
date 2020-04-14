---
title: AddRowset
parent: JSON Object Methods
grand_parent: JSON Object
nav_order: 120
---

### [](#header-3)Syntax

**AddRowset**(_name_, _rowset_)

### [](#header-3)Description

Use this method to add a Rowset object to the JSON Object.

### [](#header-3)Parameters

| Name           | Description                                                                      |
|:---------------|:---------------------------------------------------------------------------------|
| name           | Specifies the name of the rowset that needs to be added as a string.             |
| rowset         | Specifies the rowset to add to the JSON Object as a Rowset object.               |


### [](#header-3)Returns

None.

### [](#header-3)Example

```java
Local Rowset &rsOperDefn = CreateRowset(Record.PSOPRDEFN);
&rsOperDefn.Fill("WHERE OPRID = 'PS'");
   
Local PSM_JSON:Object &oObject = create PSM_JSON:Object();
   
&oObject.AddRowset("MyRowset", &rsOperDefn);
```
