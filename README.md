# Gradle

### Build Scripts

To build a project using Gradle, a build script has to be set up. By convention, the build script is called *build.gradle*. 

**Project, Tasks, & Actions**

A *build.gradle* file represents a **project** and contains **task** definitions. Each **task** definition contains a list of **actions**. An **action** is a block of code analagous to a Java method.

**Language**

Gradle build scripts are written in a DSL (Domain Specific Language) based on Groovy. 

**In-memory Representation**

Gradle creates a *Project* object and the *Task* objects based on the build file. A *Task* object consists of a list of *Action* objects. 
The order of the *Action* objects represent the order in which they have to be executed. 

### Convention over Configuration

Gradle favors convention over configuration by providing sensible default values for properties and settings. 

Conventions can be overridden if required.

*Benefits*

As sensible default values are provided, it is much easier to get started with less configuration required.


