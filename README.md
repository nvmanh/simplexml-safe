# SimpleXML

`simple-xml` is an XML serialization and deserialization framework for Java. 

# About this fork

This is a somewhat cleaned up and modernized fork of the original 
[simple-xml](https://github.com/ngallagher/simplexml) library by Niall Gallagher.

# Changes

## 2.7.1

* Initial version forked from the original repository's commit 01d47a656. This 
  corresponds roughly to simple-xml 2.7.1 with stable order on several 
  associative containers.
* Gradle is used as the build system.
* Java 1.8 or older is required.
* Any cruft not related to the core XML serialization/ parsing library
  has been removed.
* Removed pull parser support and dependency.
* Removed an explicit Stax dependency.
* Corrected a few tests for compatibility with new Java versions.
* Opened up the Provider infrastructure so that StreamProvider and DocumentProvider
  can be configured with custom underlying XML parser factory.
* Changed the defaults on existing providers to use web-safe settings (no entity 
  expansion, no external entity resolution).
