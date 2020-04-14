---
title: SetRow
parent: JSON Node Methods
grand_parent: JSON Node
nav_order: 45
---

### [](#header-3)Syntax

**SetRow**(_row_value_)

### [](#header-3)Description

Use this method to set the row value of the JSON Node.

### [](#header-3)Parameters

| Name            | Description                                                                    |
|:----------------|:-------------------------------------------------------------------------------|
| row_value       | Specifies the row value of the JSON Node as a Row object.                      |


### [](#header-3)Returns

None.

### [](#header-3)Example

```java
Local Rowset &rsOperDefn = CreateRowset(Record.PSOPRDEFN);
&rsOperDefn.Fill("WHERE OPRID = 'PS'");
   
Local Row &rOperDefn = &rsOperDefn.GetRow(1);
   
Local PSM_JSON:Node &oNode = create PSM_JSON:Node();
   
&oNode.SetRow(&rOperDefn);
```
