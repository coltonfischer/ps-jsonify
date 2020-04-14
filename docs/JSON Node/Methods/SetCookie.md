---
title: SetCookie
parent: JSON Node Methods
grand_parent: JSON Node
nav_order: 20
---

### [](#header-3)Syntax

**SetCookie**(_cookie_value_)

### [](#header-3)Description

Use this method to set the cookie value of the JSON Node.

### [](#header-3)Parameters

| Name           | Description                                                                    |
|:---------------|:-------------------------------------------------------------------------------|
| cookie_value   | Specifies the cookie value of the JSON Node as a Cookie object.                |


### [](#header-3)Returns

None.

### [](#header-3)Example

```java
Local Cookie &oCookie = %Response.CreateCookie("TheCookie");
&oCookie.Value = "TheCookieVal";
   
Local PSM_JSON:Node &oNode = create PSM_JSON:Node();
   
&oNode.SetCookie(&oCookie);
```
