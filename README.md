
[[_introduction]]
= Introduction

== Welcome to Json-lib

JSON-lib is a java library for transforming beans, maps, collections, arrays and XML to JSON
and back again to beans and DynaBeans. It is based on the work by Douglas Crockford in
http://www.json.org/java[http://www.json.org/java, window="_blank"].

The following table summarizes the types conversion between Java and JavaScript:

[cols="40,10,60"]
|===
|JSON | |Java

|string|&#8660;
|java.lang.String, java.lang.Character, char

|number | &#8660;
|java.lang.Number, byte, short, int, long, float, double

|true/false|&#8660;
|java.lang.Boolean, boolean

|null |&#8660;
|null

|function |&#8660;
|org.kordamp.json.JSONFunction

|array|&#8660;
|org.kordamp.json.JSONArray (object, string, number, boolean, function)

|object |&#8660;
|org.kordamp.json.JSONObject

|===

The `function` type from JavaScript is not part of the JSON
format "officially" (please refer to http://www.json.org[http://www.json.org])
but it is supported as well.

Json-lib requires (at least) the following dependencies in your classpath:

* Apache commons-lang3 3.9
* Apache commons-beanutils 1.9.3
* Apache commons-collections4 4.4
* slf4j 1.7.28
* ezmorph 1.0.6

Other dependencies are needed if working with XML and Groovy.

* xom 1.3.2
* groovy 2.5.8

== What is JSON

JSON (JavaScript Object Notation) is a lightweight
data-interchange format. It is easy for humans to read
and write. It is easy for machines to parse and
generate. It is based on a subset of the JavaScript
Programming Language, Standard ECMA-262 3rd Edition -
December 1999. JSON is a text format that is completely
language independent but uses conventions that are
familiar to programmers of the C-family of languages,
including C, C++, C#, Java, JavaScript, Perl, Python,
and many others.

These properties make JSON an ideal data-interchange
language.

NOTE: Documentation for older releases can be found at link:json-lib.sourceforge.net/[]