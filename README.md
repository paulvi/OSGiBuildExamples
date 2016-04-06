
Collection of OSGi project build examples.

There is no Manifest first builds for OSGi with maven or gradle.

## For maven

- `maven-bundle-plugin`
aka [Apache Felix Maven Bundle Plugin (BND)](http://felix.apache.org/documentation/subprojects/apache-felix-maven-bundle-plugin-bnd.html)
is [“Maven first” approach](http://bnd.bndtools.org/tools/maven-felix.html) 
- `bnd-maven-plugin` [announce and 2 plugins comparison](http://njbartlett.name/2015/03/27/announcing-bnd-maven-plugin.html)

## For Gradle

- [Gradle OSGi Plugin]()
- [Gradle Bundle Plugin](https://github.com/TomDmitriev/gradle-bundle-plugin) allows you to create OSGI bundles. Its main difference from the Gradle OSGI Plugin is that it uses the bnd tool to generate not only a manifest but a whole jar.
-


### Repositories

- https://github.com/eclipse/packagedrone (from http://stackoverflow.com/questions/28698190/gradle-osgi-and-obr-or-other-repository)


### Links

1. [Gradle OSGi Plugin Example: BNDTools Bundle Integration on javacodegeeks.com](https://examples.javacodegeeks.com/core-java/gradle/gradle-osgi-plugin-example/)
1. [Tools bound to bnd](http://bnd.bndtools.org/chapters/700-tools.html)
2. https://github.com/bandesz/gradle-osgi-demo
3. [GRADLE-1107 "OSGi instruction `Include-Resource` not working"](https://issues.gradle.org/browse/GRADLE-1107) open issue since 2010 (also https://github.com/TomDmitriev/gradle-bundle-plugin/issues/54 )


Add entry at http://bnd.bndtools.org/chapters/700-tools.html :
- https://github.com/bndtools/bnd.manual/compare/gh-pages...paulvi:patch-3
- https://github.com/TomDmitriev/gradle-bundle-plugin/issues/55
- https://github.com/renatoathaydes/osgi-run/issues/30
- https://github.com/akhikhl/wuff/issues/108
