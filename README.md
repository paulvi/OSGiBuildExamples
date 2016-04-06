
Collection of OSGi project build examples.

There is no Manifest first builds for OSGi with maven or gradle.

## For maven

- `maven-bundle-plugin`
aka [Apache Felix Maven Bundle Plugin (BND)](http://felix.apache.org/documentation/subprojects/apache-felix-maven-bundle-plugin-bnd.html)
is [“Maven first” approach](http://bnd.bndtools.org/tools/maven-felix.html) 
- `bnd-maven-plugin` [announce and 2 plugins comparison](http://njbartlett.name/2015/03/27/announcing-bnd-maven-plugin.html)

## For Gradle

- [Gradle OSGi Plugin](https://docs.gradle.org/current/userguide/osgi_plugin.html)
- [Gradle Bundle Plugin](https://github.com/TomDmitriev/gradle-bundle-plugin) allows you to create OSGI bundles. Its main difference from the Gradle OSGI Plugin is that it uses the bnd tool to generate not only a manifest but a whole jar.
- [`osgi-run`](https://github.com/renatoathaydes/osgi-run) "Osgi-Run - A Gradle plugin to make the development of modular applications using OSGi completely painless"
- [wuff](https://github.com/akhikhl/wuff) "Gradle plugin for automating assembly of OSGi/Eclipse bundles and applications" is suspiciously inactive for 7 months, but contrary to others has [nice to read wiki](https://github.com/akhikhl/wuff/wiki/)


### Repositories

- http://bndtools.org/repositories.html lists 

1. Index Repositories: Fixed and Local
2. File Repository
3. Aether (Maven) Repositories
4. Maven Repositories (Old Style): Maven Local and Maven Remote

- https://github.com/eclipse/packagedrone (from http://stackoverflow.com/questions/28698190/gradle-osgi-and-obr-or-other-repository)

### Links

1. [Gradle OSGi Plugin Example: BNDTools Bundle Integration on javacodegeeks.com](https://examples.javacodegeeks.com/core-java/gradle/gradle-osgi-plugin-example/)
1. [Tools bound to bnd](http://bnd.bndtools.org/chapters/700-tools.html)
2. https://github.com/bandesz/gradle-osgi-demo
3. https://github.com/paulvi/BndtoolsWorkspaceExample for an idea what to commit
3. [GRADLE-1107 "OSGi instruction `Include-Resource` not working"](https://issues.gradle.org/browse/GRADLE-1107)
 open issue since 2010 (also https://github.com/TomDmitriev/gradle-bundle-plugin/issues/54 )


Add entry at http://bnd.bndtools.org/chapters/700-tools.html :
- https://github.com/bndtools/bnd.manual/pull/30
- https://github.com/TomDmitriev/gradle-bundle-plugin/issues/55
- https://github.com/renatoathaydes/osgi-run/issues/30
- https://github.com/akhikhl/wuff/issues/108

#### Tutorials

- http://www.javaworld.com/article/2077837/java-se/hello--osgi--part-1--bundles-for-beginners.html?page=2 (from old http://stackoverflow.com/questions/4921542/using-osgi-to-develop-an-application)

#### Quotes

> Bnd is a command-line tool, developed by Peter Kriens, for building OSGi
bundles. Compared to PDE it may seem primitive, because it offers no GUI,
instead using plain text properties files and instructions issued on the command
line. However the core of the tool is very elegant and powerful, and it combines
well with standard and familiar build tools such as ANT.

http://njbartlett.name/files/osgibook_preview_20091217.pdf
