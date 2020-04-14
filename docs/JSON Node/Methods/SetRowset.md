---
title: SetRowset
parent: JSON Node Methods
grand_parent: JSON Node
nav_order: 50
---

### [](#header-3)Syntax

**SetRowset**(_rowset_value_)

### [](#header-3)Description

Use this method to set the rowset value of the JSON Node.

### [](#header-3)Parameters

| Name            | Description                                                                    |
|:----------------|:-------------------------------------------------------------------------------|
| rowset_value    | Specifies the rowset value of the JSON Node as a Rowset object.                |


### [](#header-3)Returns

None.

### [](#header-3)Example

```java
Local Rowset &rsOperDefn = CreateRowset(Record.PSOPRDEFN);
&rsOperDefn.Fill("WHERE OPRID = 'PS'");

Local PSM_JSON:Node &oNode = create PSM_JSON:Node();
   
&oNode.SetRowset(&rsOperDefn);
```
