[![Apache 2.0](https://img.shields.io/github/license/nebula-plugins/nebula-publishing-plugin.svg)](http://www.apache.org/licenses/LICENSE-2.0)

# Awesome OSGi [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)

[<img src="http://www.rebaze.com/assets/Rebaze_icon_colors_tbg.png" align="right" width="100">](http://rebaze.com)

[<img src="https://avatars0.githubusercontent.com/u/1123352?v=3&s=400" align="right" width="100">](http://osgi.org/)

> Useful resources for working with [OSGi](https://osgi.org)

*Inspired by the [awesome](https://github.com/sindresorhus/awesome) list thing.*

## Framework Implementations
OSGi framework implementations are the kernel of your OSGi runtime. While you compile against APIs specified by the [OSGi Alliance](http://osgi.org) you always need a concrete framework implementation.
### Major Open Source implementations
* [Apache Felix](https://felix.apache.org) - OSGi Core 6 compliant Implementation from Apache Community.
* [Eclipse Equinox](http://www.eclipse.org/equinox/) - OSGi Core 6 Reference Implementation from the Eclipse Community.

## OSGi based Containers

### Apache Karaf
[Apache Karaf](http://karaf.apache.org) is an opinionated OSGi distributions that comes with read-made solutions for common operation topics such as:
* Hot deployment
* Complete Console
* Dynamic Configuration* Advanced Logging System
* Provisioning
* Management
* Security
* Cloud deployment

As such, Karaf might be your first choice when selecting OSGi as a runtime and you _do not want_ to create all of the above yourself.

Karaf works on small devices (perfect for IoT) as well as part of a cloud container deployment.  


## First class bundles
Bundles are regular jars with extra Metadata.
This list contains libraries that provide first level OSGi citizens. So not just wrapped java libraries but implementations of OSGi standards (e.g. from the OSGi Compendium Specification).

### High quality bundle distributors
* [OSGi enRoute](http://enroute.osgi.org) - Set of APIs and Implementations for getting started with OSGi quickly.
* [Apache Felix](http://felix.apache.org) - Felix is not just an OSGi framework implementation (read above) but also host of many super useful OSGi bundles for parts of the OSGi specification such as Logging, Web Servers, Configuration and Shell bundles. Most notably:
  * [Felix ConfigAdmin](http://felix.apache.org/documentation/subprojects/apache-felix-config-admin.html) - Implementation of the OSGi Compendium Configuration Admin Service.
  * [Felix SCR](http://felix.apache.org/documentation/subprojects/apache-felix-service-component-runtime.html) - Implementation of the OSGi Declarative Services Specification.
  * [Felix GOGO Shell](http://felix.apache.org/documentation/subprojects/apache-felix-gogo.html) - Implementation of OSGi RFC 147, the standard shell for OSGi-based environments.

* [Apache Aries](http://aries.apache.org) - OSGi Enterprise Bundle Implementations (e.g. JPA, JTA etc.)
* [Amdatu](http://amdatu.org) - Amdatu is a set of open source components and tools to build modular applications in Java. E.g. Components for multi tenancy, blobstores, MongoDB integration and RESTful web services.
* [OPS4J](https://ops4j1.jira.com/wiki/display/ops4j/Pax) - Pax is the umbrella project for all OSGi bundles and tools at the OPS4J Community.

## Web related bundles
* [Pax Web](https://github.com/ops4j/org.ops4j.pax.web) - OSGi R4 Http Service and Web Applications (OSGi Enterprise Release chapter 128) implementation using Jetty 9 and Tomcat 7.
* [JAX-RS Connector](https://github.com/hstaudacher/osgi-jax-rs-connector) - An OSGi - JAX-RS 2.0 Connector

## IDE Support
Without any doubt, the ultimate tooling is the one that is deeply integrated with your IDE.
As of now (June 2016) only Eclipse has a production ready IDE integration. And its not PDE (the Eclipse Plugin Development Tooling) but Bndtools.
* [Bndtools](http://bndtools.org) - Lipstick for BND in Eclipse (quote: Neil Bartlett)

## Testing
* [Pax Exam](https://ops4j1.jira.com/wiki/display/PAXEXAM4/Pax+Exam) - IDE independent OSGi and JEE integration testing framework.

## Guides
* [Where to Find Stuff](http://enroute.osgi.org/book/700-links.html) - The enRoute directory of OSGi related resources.
* [enRoute Appnotes](http://enroute.osgi.org/book/680-appnotes.html) - A directory of discussions to OSGi related topics. A very worthy read!

## Blogs to follow
* [Official OSGi Blog](http://blog.osgi.org/) - Official OSGi Blog. Mostly articles by Peter Kriens.
* [Neil Bartlett](http://njbartlett.name/) - Neil Bartlett, creator of Bndtools.
* [Know How Lab](http://blog.knowhowlab.org) - Dmytro Pishchukhin writing about OSGi tooling, libraries and AWS.

## Build Tools
How do you create OSGi components? How do you work with external, non bundle dependencies?
There are quite many tools out there that let you work with your tools of choice (Maven, Gradle, any other scriptable environment) to work on OSGi projects.
* [BND](http://bnd.bndtools.org) - BND is the engine behind a number of popular software development tools that support OSGi.
* [Maven Bundle Plugin](http://felix.apache.org/documentation/subprojects/apache-felix-maven-bundle-plugin-bnd.html) - The classic maven plugin for creating OSGi metadata.
* [bnd Maven Plugin](https://github.com/bndtools/bnd/tree/master/maven/bnd-maven-plugin) - A new (introduced in 2015) take on bnd library integration as a maven plugin. Neil Bartlett [introducing the new maven plugin](http://njbartlett.name/2015/03/27/announcing-bnd-maven-plugin.html) in his blog.
* [BND Indexer Maven Plugin](https://github.com/bndtools/bnd/tree/master/maven/bnd-indexer-maven-plugin) - Create OSGi R5 Repository indexes from Maven Dependency/pom.

## License

Apache License 2.0
