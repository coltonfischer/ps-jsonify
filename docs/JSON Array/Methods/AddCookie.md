---
title: AddCookie
parent: JSON Array Methods
grand_parent: JSON Array
nav_order: 30
---

### [](#header-3)Syntax

**AddCookie**(_cookie_)

### [](#header-3)Description

Use this method to add a Cookie object to the JSON Array.

### [](#header-3)Parameters

| Name           | Description                                                                    |
|:---------------|:-------------------------------------------------------------------------------|
| cookie         | Specifies the cookie to add to the JSON Array as a Cookie object.              |


### [](#header-3)Returns

None.

### [](#header-3)Example

```java
Local Cookie &oCookie = %Response.CreateCookie("MyCookie");
&oCookie.Value = "MyCookeVal";
   
Local PSM_JSON:Array &oArray = create PSM_JSON:Array();
   
&oArray.AddCookie(&oCookie);
```
