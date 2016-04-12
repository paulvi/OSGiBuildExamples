
Collection of OSGi project build examples.

There is no [Manifest first builds for OSGi](http://stackoverflow.com/questions/35629891/manifest-first-osgi-build-with-gradle-migrating-from-ant-to-gradle) with maven or gradle.

## For maven

- `maven-bundle-plugin`
aka [Apache Felix Maven Bundle Plugin (BND)](http://felix.apache.org/documentation/subprojects/apache-felix-maven-bundle-plugin-bnd.html)
is [“Maven first” approach](http://bnd.bndtools.org/tools/maven-felix.html) 
- `bnd-maven-plugin` [announce and 2 plugins comparison](http://njbartlett.name/2015/03/27/announcing-bnd-maven-plugin.html)
- [`maven-pax-plugin`](https://github.com/ops4j/org.ops4j.pax.construct) "Build, manage and deploy many types of OSGi bundles". It have not release for 5 years, than [got new version](http://mvnrepository.com/artifact/org.ops4j/maven-pax-plugin) in 2016.
- [Pax-Runner](https://ops4j1.jira.com/wiki/display/paxrunner/Pax+Runner) [on GitHub](https://github.com/ops4j/org.ops4j.pax.runner)

## For Gradle

- [Gradle OSGi Plugin](https://docs.gradle.org/current/userguide/osgi_plugin.html)
- [Gradle Bundle Plugin](https://github.com/TomDmitriev/gradle-bundle-plugin) allows you to create OSGI bundles. Its main difference from the Gradle OSGI Plugin is that it uses the bnd tool to generate not only a manifest but a whole jar.
- [`osgi-run`](https://github.com/renatoathaydes/osgi-run) "Osgi-Run - A Gradle plugin to make the development of modular applications using OSGi completely painless"
- [wuff](https://github.com/akhikhl/wuff) "Gradle plugin for automating assembly of OSGi/Eclipse bundles and applications" is suspiciously inactive for 7 months, but contrary to others has [nice to read wiki](https://github.com/akhikhl/wuff/wiki/).
For Eclipse plugins and apps only: Wuff as a gradle-based alternative to Eclipse Tycho.


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

Old bnd tools list from http://www.aqute.biz/Bnd/Download

<p>bnd is already used by several different projects.
</p>
<div class="vspace"></div><table width="100%"><tbody><tr><td><a class="urllink" href="http://njbartlett.name/bndtools.html" rel="nofollow">Bndtools</a></td><td>A plugin for Eclipse that is completely based on bnd. It is available in the Eclipse marketplace.</td></tr>
<tr><td><a class="urllink" href="http://felix.apache.org/site/apache-felix-maven-bundle-plugin-bnd.html" rel="nofollow">Apache Maven Bundle Plugin</a></td><td>The plugin is based on bnd. You can find more information and tips at <a class="wikilink" href="http://www.aqute.biz/Bnd/Maven">Maven</a>.</td></tr>
<tr><td><a class="urllink" href="http://felix.apache.org/site/sigil-key-features.html" rel="nofollow">Apache Felix Sigil</a></td><td>Ant/Eclipse plugin for <span class="wikiword">OSGi</span> development.</td></tr>
<tr><td><a class="urllink" href="http://jaxenter.com/bnd4sbt-bnd-plugin-for-sbt-0-4-14804.html" rel="nofollow">Bnd4sbt</a></td><td>A bundle tool for Scala applications.</td></tr>
<tr><td><a class="urllink" href="http://www.osmorc.org/" rel="nofollow">Osmorc</a></td><td>A plugin for IDEA's <span class="wikiword">IntelliJ</span>.</td></tr>
<tr><td><a class="urllink" href="http://oss.intalio.com/buildr4osgi/index.html" rel="nofollow">Build4OSGi</a></td><td>A plugin for the <span class="wikiword">JRuby</span> based build tool <a class="urllink" href="http://buildr.apache.org/index.html" rel="nofollow">buildr</a></td></tr>
<tr><td><a class="urllink" href="http://www.gradle.org/0.9-rc-1/docs/userguide/userguide_single.html#osgi_plugin" rel="nofollow">Gradle OSGi Plugin</a></td><td>A <a class="urllink" href="http://www.gradle.org" rel="nofollow">Gradle</a> based <span class="wikiword">OSGi</span> plugin. Gradle is a Groovy based builder.</td></tr>
<tr><td><a class="wikilink" href="http://www.aqute.biz/Bnd/Ant">Ant</a></td><td>bnd is already an ant task</td></tr>
<tr><td><a class="urllink" href="http://code.google.com/p/apache-felix-intellij-plugin/" rel="nofollow">Apache Felix IntelliJ Plugin</a></td><td align="left">provides native <span class="wikiword">IntelliJ</span> IDEA support for developing, running and debugging <span class="wikiword">OSGi</span> projects developed using Apache Felix and the Apache Felix Maven Bundle Plugin.</td></tr>
</tbody></table>
