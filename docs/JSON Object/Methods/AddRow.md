---
title: AddRow
parent: JSON Object Methods
grand_parent: JSON Object
nav_order: 115
---

### [](#header-3)Syntax

**AddRow**(_name_, _row_)

### [](#header-3)Description

Use this method to add a Row object to the JSON Object.

### [](#header-3)Parameters

| Name           | Description                                                                      |
|:---------------|:---------------------------------------------------------------------------------|
| name           | Specifies the name of the row that needs to be added as a string.                |
| row            | Specifies the row to add to the JSON Object as a Row object.                     |


### [](#header-3)Returns

None.

### [](#header-3)Example

```java
Local Rowset &rsOperDefn = CreateRowset(Record.PSOPRDEFN);
&rsOperDefn.Fill("WHERE OPRID = 'PS'");
   
Local Row &rOperDefn = &rsOperDefn.GetRow(1);
   
Local PSM_JSON:Object &oObject = create PSM_JSON:Object();
   
&oObject.AddRow("MyRow", &rOperDefn);
```
