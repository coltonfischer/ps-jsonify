---
layout: default
title: Home
nav_order: 1
description: "PS-Jsonify is a library for converting PeopleCode objects to JSON."
permalink: /
---

# Convert PeopleCode Objects to JSON
{: .fs-9 }

PS-Jsonify provides an easy to use API to build dynamic JSON from PeopleCode objects.  PS-Jsonify is implemented via Application Class PeopleCode and requires no external dependencies.
{: .fs-6 .fw-300 }

[Get started now](#getting-started){: .btn .btn-primary .fs-5 .mb-4 .mb-md-0 .mr-2 } [View it on GitHub](https://github.com/coltonfischer/ps-jsonify){: .btn .fs-5 .mb-4 .mb-md-0 }

---

## Getting Started

### Dependencies

You must be on PeopleTools `8.55` or later.

### Installing

Download and import the [PeopleSoft project](https://github.com/coltonfischer/ps-jsonify/raw/master/PSM_JSON.zip) into App Designer

## How to Use

The PS-Jsonify library offers three consumer App Classes: `PSM_JSON:Object`, `PSM_JSON:Array`, and `PSM_JSON:Node`.  These three classes can be used to build and parse JSON Objects, Arrays, and Nodes respectively.

### Building JSON Objects

Use the `PSM_JSON:Object` Class to build JSON Objects.

```
Local PSM_JSON:Object &oJson = create PSM_JSON:Object();
```

The various `AddXxx` methods allow you to add PeopleCode object types to the JSON Object.

```
Local Rowset &rsOperDefn = CreateRowset(Record.PSOPRDEFN);
&rsOperDefn.Fill("WHERE OPRID = 'PS'");
   
&oJson.AddRowset("MyRowset", &rsOperDefn);
```

Use the `AddProperty` method if you are unsure of the data or object type.

```
Local any &aValue = CreateArrayAny("test", True, 6, Null);
   
If Int(Rand() * 10) > 5 Then
   &aValue = Null;
End-If;
   
&oJson.AddProperty("MyProperty", &aValue);
```

Invoke the `ToJsonString` method to get the JSON String output. 

```
Local String &sOutput = &oJson.ToJsonString();
```

See the [JSON Object section](/ps-jsonify/JSON%20Object/) to view all of the available methods and properties.

### Building JSON Arrays

Use the `PSM_JSON:Array` Class to build JSON Arrays.

```
Local PSM_JSON:Array &oJson = create PSM_JSON:Array();
```

The various `AddXxx` methods allow you to add PeopleCode object types to the JSON Array.

```
Local Record &rPsOptions = CreateRecord(Record.PSOPTIONS);
&rPsOptions.SelectByKey();
   
&oJson.AddRecord(&rPsOptions);
```

Use the `AddElement` method if you are unsure of the data or object type.
```
Local any &aValue = %Request;
   
If Int(Rand() * 10) > 5 Then
   &aValue = %Response;
End-If;
   
&oJson.AddElement(&aValue);
```

Invoke the `ToJsonString` method to get the JSON String output. 

```
Local String &sOutput = &oJson.ToJsonString();
```

See the [JSON Array section](/ps-jsonify/JSON%20Array/) to view all of the available methods and properties.

### Building JSON Nodes

Use the `PSM_JSON:Node` Class to build JSON Nodes.

```
Local PSM_JSON:Node &oJson = create PSM_JSON:Node();
```

The various `SetXxx` methods allow you convert PeopleCode object types to a JSON Node.

```
Local PTPP_COLLECTIONS:Shortcut &oCref;
&oCref = create PTPP_COLLECTIONS:Shortcut(%Portal, "PT_CHANGE_PASSWORD_GBL");
   
&oJson.SetClass(&oCref);
```

Invoke the `ToJsonString` method to get the JSON String output. 

```
Local String &sOutput = &oJson.ToJsonString();
```

See the [JSON Node section](/ps-jsonify/JSON%20Node/) to view all of the available methods and properties.

_Note: Not all PeopleCode object types are supported. `ToJsonString` will return the object type name as a String if you use an unsupported type._

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
