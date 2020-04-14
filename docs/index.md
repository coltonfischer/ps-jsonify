---
layout: default
title: Home
nav_order: 1
description: "PS-Jsonify is a library for converting PeopleCode objects to JSON."
permalink: /
---

# Convert PeopleCode Objects to JSON
{: .fs-9 }

PS-Jsonify provides an easy to use API to build complex and dynamic JSON from PeopleCode objects.  PS-Jsonify is implemented via Application Class PeopleCode and requires no external dependencies.
{: .fs-6 .fw-300 }

[Get started now](#getting-started){: .btn .btn-primary .fs-5 .mb-4 .mb-md-0 .mr-2 } [View it on GitHub](https://github.com/coltonfischer/ps-jsonify){: .btn .fs-5 .mb-4 .mb-md-0 }

---

## Getting Started

### Dependencies

You must be on PeopleTools `8.55` or later.

### Installing

Download and import the [PeopleSoft project](https://github.com/coltonfischer/ps-jsonify/raw/master/PSM_JSON.zip) into App Designer

## How to Use

The PS-Jsonify library offers three consumer Application Classes: `PSM_JSON:Object`, `PSM_JSON:Array`, and `PSM_JSON:Node`.  These three classes extend the functionality of the PeopleCode `JsonObject`, `JsonArray`, and `JsonNode` types respectively.

### Building JSON Objects

Use the `PSM_JSON:Object` Class to build dynamic JSON Objects.  

```
Local PSM_JSON:Object &oJson = create PSM_JSON:Object();
```

The various `AddXxx` methods allow you to add PeopleCode native object types to the JSON Object.

```
/* AddRecord and AddRequest Examples */
Local Record &rPsOptions = CreateRecord(Record.PSOPTIONS);
&rPsOptions.SelectByKey();
   
&oJson.AddRecord("MyRecord", &rPsOptions);
&oJson.AddRequest("MyRequest", %Request);
```

Use the `AddProperty` method if you are unsure of the data or object type.
```
/* AddProperty Example */
Local Any &aAny = &oVar;
&oJson.AddProperty("data", &aAny);
```

Invoke the `ToJsonString` method when you are ready to get the JSON String output. 

```
Local String &sOutput = &oJson.ToJsonString();
```

You can always access the underlying `JsonObject` object by calling the `ToJsonObject` method.

```
Local JsonObject &joMyJsonObject = &oJson.ToJsonObject();
```

### Building JSON Arrays

Use the `PSM_JSON:Array` Class to build dynamic JSON Arrays

```
Local PSM_JSON:Array &oArray = create PSM_JSON:Array();
```

The various `AddXxx` methods allow you to add PeopleCode native object types to the JSON Array.

```
/* Adding Array Elements Example */
&oArray.AddString("Hello");
&oArray.AddBoolean( True);
&oArray.AddNumber(2);
```

Use the `AddElement` method if you are unsure of the data or object type.
```
/* AddElement Example */
Local any &aAny = &oVar;
&oArray.AddElement(&aAny);
```

Invoke the `ToJsonString` method when you are ready to get the JSON String output. 

```
Local String &sOutput = &oArray.ToJsonString();
```

You can always access the underlying `JsonArray` object by calling the `ToJsonArray` method.

```
Local JsonArray &jaMyJsonArray = &oArray.ToJsonArray();
```
### Any to JSON String

Convert an `Any` object type to a JSON String with the `PSM_JSON:Node` Class.

```
Local PTPP_COLLECTIONS:Shortcut &Cref;
&Cref = create PTPP_COLLECTIONS:Shortcut(%Portal, "PT_CHANGE_PASSWORD_GBL");

Local PSM_JSON:Node &jnJson = create PSM_JSON:Node(&Cref);
%Response.Write(&jnJson.ToJsonString());
```
_Note: Not all object types are supported at this time.  `ToJsonString()` will return the object type name as a String  if you use an unsupported type._

---

### Contributing

When contributing to this repository, please first discuss the change you wish to make via issue,
email, or any other method with the owners of this repository before making a change.

#### Thank you to the contributors of PS-Jsonify!

<ul class="list-style-none">
{% for contributor in site.github.contributors %}
  <li class="d-inline-block mr-1">
     <a href="{{ contributor.html_url }}"><img src="{{ contributor.avatar_url }}" width="32" height="32" alt="{{ contributor.login }}"/></a>
  </li>
{% endfor %}
</ul>
