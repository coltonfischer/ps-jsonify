# PS-Jsonify

View the [Documentation Site](http://www.coltonfischer.com/ps-jsonify/) for complete API details.

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

See the [JSON Object section](http://www.coltonfischer.com/ps-jsonify/JSON%20Object/) to view all of the available methods and properties.

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

See the [JSON Array section](http://www.coltonfischer.com/ps-jsonify/JSON%20Array/) to view all of the available methods and properties.

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

See the [JSON Node section](http://www.coltonfischer.com/ps-jsonify/JSON%20Node/) to view all of the available methods and properties.

_Note: Not all PeopleCode object types are supported. `ToJsonString` will return the object type name as a String if you use an unsupported type._
