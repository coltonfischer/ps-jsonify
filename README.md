# PS-Jsonify


_This is still a work in progress..._

PeopleCode library for converting native object types to JSON.  Built on top of JsonObject, JsonArray, and JsonNode PeopleCode objects.  Aims to provide an easy to use API to build complex and dynamic JSON.  

The following object types are currently supported:
```
Array
App Class
Cookie
Exception
Hash
Record
Request
Response
Row
Rowset
```


## Getting Started

PS-Jsonify is implemented via Application Class PeopleCode and requires no external dependencies.  The only prerequisite is to be on PeopleTools `8.55` or later.


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

Invoke the `ToString` method when you are ready to get the JSON String output. 

```
Local String &sOutput = &oJson.ToString();
```

You can always access the underlying `JsonObject` native object by referencing the `Value` property.

```
Local JsonObject &joMyJsonObject = &oJson.Value;
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

Invoke the `ToString` method when you are ready to get the JSON String output. 

```
Local String &sOutput = &oArray.ToString();
```

You can always access the underlying `JsonArray` native object by referencing the `Value` property.

```
Local JsonArray &jaMyJsonArray = &oArray.Value;
```
### Any to JSON String

Convert an `Any` object type to a JSON String with the `PSM_JSON:Node` Class.

```
Local PTPP_COLLECTIONS:Shortcut &Cref;
&Cref = create PTPP_COLLECTIONS:Shortcut(%Portal, "PT_CHANGE_PASSWORD_GBL");

Local PSM_JSON:Node &jnJson = create PSM_JSON:Node(&Cref);
%Response.Write(&jnJson.ToString());
```
_Note: Not all object types are supported at this time.  `ToString()` will return the object type name as a String  if you use an unsupported type._
