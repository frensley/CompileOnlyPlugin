CompileOnlyPlugin
=================

Adds a _compileOnly_ configuration to a Java based gradle build.

The plugin will also take care of registering the _compilyOnly_ dependencies to the matching scopes of IntelliJ Idea and Eclipse

Usage
-----
Add the following lines to your gradle build script

    buildscript {
      repositories {
        mavenCentral()
      }
      dependencies {
        classpath 'com.coders-kitchen:compileonlyplugin:1.0.0'
      }
    }

    apply plugin: 'compileOnly'

    dependencies {
      compileOnly <dependencies>
    }
