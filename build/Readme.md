# Build Directory

This directory contains a set of maven modules to handle the native build steps,
these are run independently of any deploy step so these modules do not get
published to Nexus or Maven Central.

The built natives are transferred to `wildfly-openssl-natives/target/lib`.

The modules under `wildfly-openssl-natives/package` are used to take the native
libraries from the `lib` directory and bundle into individual modules as well as
a single aggregated module of all available libraries.