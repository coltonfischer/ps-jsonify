---
title: AddCookie
parent: JSON Object Methods
grand_parent: JSON Object
nav_order: 30
---

### [](#header-3)Syntax

**AddCookie**(_name_, _cookie_)

### [](#header-3)Description

Use this method to add a Cookie object to the JSON Object.

### [](#header-3)Parameters

| Name           | Description                                                                      |
|:---------------|:---------------------------------------------------------------------------------|
| name           | Specifies the name of the cookie that needs to be added as a string.             |
| cookie         | Specifies the cookie to add to the JSON Object as a Cookie object.               |


### [](#header-3)Returns

None.

### [](#header-3)Example

```java
Local Cookie &oCookie = %Response.CreateCookie("TheCookie");
&oCookie.Value = "TheCookieVal";
   
Local PSM_JSON:Object &oObject = create PSM_JSON:Object();
   
&oObject.AddCookie("MyCookie", &oCookie);
```
