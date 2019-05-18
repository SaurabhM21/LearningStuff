# Avro IDL

## What is Avro IDL?
A higher-level language for authoring Avro schemata. IDL = interface description languages.

An Avro IDL file consists of exactly one protocol definition. The minimal protocol is defined by the following code:

protocol MyProtocol {
}

This is equivalent to (and generates) the following JSON protocol definition:

{
"protocol" : "MyProtocol",
  "types" : [ ],
  "messages" : {
  }
}

The namespace of the protocol may be changed using the @namespace annotation:

@namespace("mynamespace")
protocol MyProtocol {
}


## References
https://avro.apache.org/docs/1.8.2/idl.html