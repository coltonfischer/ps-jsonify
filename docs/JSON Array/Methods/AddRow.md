---
title: AddRow
parent: JSON Array Methods
grand_parent: JSON Array
nav_order: 115
---

### [](#header-3)Syntax

**AddRow**(_row_)

### [](#header-3)Description

Use this method to add a Row object to the JSON Array.

### [](#header-3)Parameters

| Name           | Description                                                                    |
|:---------------|:-------------------------------------------------------------------------------|
| row            | Specifies the row to add to the JSON Array as a Row object.                    |


### [](#header-3)Returns

None.

### [](#header-3)Example

```java
Local Rowset &rsOperDefn = CreateRowset(Record.PSOPRDEFN);
&rsOperDefn.Fill("WHERE OPRID = 'PS'");
   
Local Row &rOperDefn = &rsOperDefn.GetRow(1);
   
Local PSM_JSON:Array &oArray = create PSM_JSON:Array();
   
&oArray.AddRow(&rOperDefn);
```
