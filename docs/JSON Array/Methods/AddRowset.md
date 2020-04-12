---
title: AddRowset
parent: JSON Array Methods
grand_parent: JSON Array
nav_order: 120
---

### [](#header-3)Syntax

**AddRowset**(_rowset_)

### [](#header-3)Description

Use this method to add a Rowset object to the JSON Array.

### [](#header-3)Parameters

| Name           | Description                                                                    |
|:---------------|:-------------------------------------------------------------------------------|
| rowset         | Specifies the rowset to add to the JSON Array as a Rowset object.              |


### [](#header-3)Returns

None.

### [](#header-3)Example

```java
Local Rowset &rsOperDefn = CreateRowset(Record.PSOPRDEFN);
&rsOperDefn.Fill("WHERE OPRID = 'PS'");
   
Local PSM_JSON:Array &oArray = create PSM_JSON:Array();
   
&oArray.AddRowset(&rsOperDefn);
```
