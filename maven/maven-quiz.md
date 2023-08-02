## Maven

#### Q1. What element in the pom.xml file allows you to provide values that can be reused in other elements of the pom.xml?

- [ ] Plugins
- [ ] Build
- [ ] Properties
- [x] Parent

#### Q2. If you wish to build and package your artifact using the Maven package goal but don't want to execute the unit tests, which environment variable and value would you use?

- [ ] `maven.test.ignore=TRUE`
- [ ] `maven.test.run=FALSE`
- [x] `maven.test.skip=TRUE`
- [ ] `maven.verify.execute=FALSE`

#### Q3. When building a Maven EAR project and specifying the configuration of which projects to include, what is the element in the plugin configuration that contains Enterprise Java Bean projects?

- [ ] modules/webModule
- [x] modules/ejbModule
- [ ] modules/enterpriseModules
- [ ] modules/services

#### Q4. The goal that is executed to generate and deploy a documentation website is \_.

- [ ] deliver
- [x] site
- [ ] doc
- [ ] deploy

#### Q5. What does the `mvn -version` command do?

- [ ] It builds your Maven project.
- [ ] It installs Maven on your computer.
- [ ] It updates Maven to the latest version.
- [x] It print out your installed version of Maven.

#### Q6. There are several properties available for use in a pom.xml file that refer to details of the project, such as groupId and version. What do all of these properties start with?

- [ ] pom
- [ ] maven
- [ ] jar
- [x] project

#### Q7. What directory structure contains the source code of your artifact?

- [ ] src/code
- [ ] src/test/java
- [x] src/main/java
- [ ] src/main/resources

#### Q8. Which command is used to run the clean lifecycle followed by verify, install, and package with Maven?

- [ ] `mvn clean install package`
- [x] `mvn package`
- [ ] `mvn clean install`
- [ ] Option 4

```shell script
mvn clean
mvn package
mvn verify
mvn install
```

#### Q9. Which goal would you use with the Dependency plugin to determine which included dependencies are not used, as well as those you are using that you have not defined?

- [ ] `dependency:tree`
- [ ] `dependency:properties`
- [ ] `dependency:evaluate`
- [x] `dependency:analyze`

#### Q10. In a multimodule project, if you have a plugin bound to a phase in the parent, it will be bound to the same phase in the module. What strategy could you employ to prevent the plugin from executing in the module?

- [ ] In the excluded element of the build section of the POM, list the plugin you do not want to run.
- [ ] Set the phase in the module to none.
- [x] Set a value in the configuration of the plugin in the module to be excluded like this: TRUE.
- [ ] Do not specify the plugin in the module.

#### Q11. When building a web application with a WAR type project, which project directory should contain the style sheet, JavaScript, and other static file?

- [ ] src/main/static
- [ ] src/main/web
- [ ] src/main/resources
- [x] src/main/webapp

#### Q12. When performing a build, which Maven plugin will allow you to set the specific version of the artifact to be built without manual modifying the pom.xml file?

- [ ] Compiler
- [ ] Surefire
- [x] Versions
- [ ] Javadoc

#### Q13. When building a Maven Archetype, what is the filepath and file of the archetype descriptor that specifies how to lay out the prototype files?

- [ ] `src/main/template/descriptor.xml`
- [x] `src/main/resources/META-INF/maven/archetype-descriptor.xml`
- [ ] `src/main/archetype/descriptor.xml`
- [ ] `src/main/resources/META-INF/maven/maven-archetype.xml`

#### Q14. What is a valid packaging type for a Maven project?

- [ ] WAR
- [x] all of these answers
- [ ] POM
- [ ] EAR

#### Q15. When two dependencies of your Maven project introduce the same transitive dependency with different versions, which one(s) will be included in the dependency list for your project?

- [ ] the dependency with the higher version
- [ ] the transitive dependency that comes from the dependency listed first in the pom.xml file
- [ ] the transitive dependency that comes from the dependency listed last in the pom.xml file
- [x] the transitive dependency version of the artifact that is closest to your project

#### Q16. Many organizations set up local mirrors to the Maven central repository. In order to leverage your company's Maven repository as a proxy for the Maven central repository, which element should you put into the settings.xml file?

- [ ] Replacements
- [ ] Proxies
- [ ] Mirrors
- [x] LocalRepositories

#### Q17. Which Maven plugin would you leverage to specify the version of the compiler to target as well as the source level of the language?

- [ ] Versions
- [ ] Surefire
- [ ] Target
- [x] Compiler

#### Q18. If your machine is behind a proxy, where should you specify the proxy server settings in order for Maven to access remote resources?

- [ ] `.m2/proxy.txt`
- [ ] `pom.xml`
- [ ] `proxy.xml`
- [x] `settings.xml`

#### Q19. What environment variable can you alter to increase the memory Maven uses?

- [x] MAVEN_OPTS
- [ ] M2_HOME
- [ ] MAVEN_MEMORY
- [ ] PATH

#### Q20. How can you use Maven to run unit tests in parallel?

- [ ] It is not possible to do this.
- [ ] Implement the JUnit dependency and add a configuration that sets the parallel element to true.
- [x] Specify the Maven Surefire Plugin and add a configuration that sets the parallel element to true.
- [ ] Move each test suite into a separate submodule.

#### Q21. What will the mvn dependency:tree command do?

- [ ] Verify the dependencies defined in the POM file.
- [x] Print out a report of your project's dependencies in a tree format.
- [ ] Download all the transitive dependencies.
- [ ] Prune unused dependencies from your dependency tree.

#### Q22. How do you run a single unit test in Maven?

- [ ] Maven runs only a single unit test by default.
- [x] Use the -Dtest= flag and pass in the name of the test.
- [ ] Use a plugin that can specify the test you want to run.
- [ ] It is not possible to do this.

#### Q23. How can Maven profiles be triggered?

- [ ] by explicitly calling the profiles using the -P flag
- [ ] based on environment variables
- [x] all of these answers
- [ ] through Maven settings

#### Q24. Why will an mvn install command not deploy any artifacts to a remote repository?

- [ ] The name of the artifact must also be specified in the command.
- [ ] The name of the remote repository must also be specified in the command.
- [ ] Deploying artifacts to a remote repository must be done manually.
- [x] The deploy phase of the default Maven lifecycle comes after the install phase.

#### Q25. Suppose you want to include a properties file in the JAR generated by your Maven build. What directory should you put it in?

- [x] `${basedir}/src/main/resources`
- [ ] `${basedir}/src/main/java/resources`
- [ ] `${basedir}/resources`
- [ ] `${basedir}/src/main/properties`

#### Q26. Which structure in a settings.xml file allows for flexing properties based on some value for the runtime of Maven?

- [ ] Environment
- [ ] Properties
- [ ] Switch
- [x] Profiles

#### Q27. What does it mean if the scope of a dependency is runtime?

- [x] The dependency is not required to compile the project, but is needed at runtime.
- [ ] The dependency is needed at compile time and at runtime, and must be packaged for distribution.
- [ ] The dependency is needed at compile time and at runtime, but does NOT need to be packaged for distribution.
- [ ] The dependency is required for compilation.

#### Q28. If you want to utilize a locally developed JAR file in another project and that JAR file has not been deployed to either the Maven central repository or your own locally sourced mirror repository, what Maven goal do you need to execute on the locally developed JAR project?

- [ ] package
- [x] install
- [ ] compile
- [ ] test

#### Q29. What is the default packaging type for a Maven project build artifact?

- [ ] WAR
- [x] JAR
- [ ] EAR
- [ ] POM

#### Q30. What does the following command do?

> mvn archetype:generate \
> -DgroupID=sample-maven-project \
> -DartifactID=com.palmer.bethan.sample \
> -Dversion=1.0.0 \
> -DinteractiveMode=false

- [ ] It does nothing since no archetype has been specified
- [ ] It generates a new Maven archetype
- [x] It generates a new Maven project using the default Maven archetype
- [ ] It cleans and installs the sample-maven-project project

#### Q31. When defining a dependency that is included with the runtime container, what scope do you use in the pom.xml?

- [x] provided
- [ ] compile
- [ ] execution
- [ ] runtime

#### Q32. What argument do you pass to Maven in order to update SNAPSHOT from the remote repository?

- [x] -U
- [ ] -J
- [ ] -X
- [ ] -S

#### Q33. When performing a release using the Maven release plugin, which environment variable for batch mode is used to define the stamp placed in SCM to indicate the state of the artifact for the actual release?

- [ ] tag
- [ ] scmMark
- [ ] developmentVersion
- [x] releaseVersion

#### Q34. These are two general uses of plugins. The first is build and the second is \_

- [x] reporting
- [ ] servers
- [ ] dependencies
- [ ] distribution management

#### Q35. What does the mvn clean command do?

- [x] It removes the target directory
- [ ] It updates the version of the plugins defined in the POM file.
- [ ] It removes unused dependencies in your project
- [ ] It builds your project

#### Q36. Bellow is a definition of the Maven JAR Plugin, where the main class is set to com.palmer.bethan.App. What is the effect of this?

```
<configuration>
    <archive>
        <manifest>
            <addClasspath>true</addClasspath>
            <mainClass>com.palmer.bethan.App</mainClass>
        </manifest>
    </archive>
</configuration>
```

- [ ] Maven will generate javadocs for the App class.
- [x] Maven will generate an executable JAR, which can be used to run the App class.
- [ ] Maven will include only the App class when it compiles the source code.
- [ ] Maven will add an empty main method to the App class.

#### Q37. Suppose you are packaging a Maven project and see the following error: "[WARNING] Using platform encoding (Cp1252 actually) to copy filtered resources, i.e. build is platform dependent!" What do you add to your POM file to set the platform encoding to ensure your build is not platform dependent?

- [ ] <project.build.resources>
- [ ] <maven.compiler.source>
- [x] <project.build.sourceEncoding>
- [ ] <project.compiler.encoding>

#### Q38. Why might you not want to include groupId and version elements in child POM files?

- [ ] If you include these elements, an error will be thrown when you try to build the project.
- [x] These elements are inherited from the parent POM file, and do not need to be repeated.
- [ ] Child POM files should include definitions of only dependencies and plugins.
- [ ] The values in the parent POM will be overridden by what is defined in the child POM.

[maven docs](https://maven.apache.org/guides/introduction/introduction-to-the-pom.html#the-solution)

#### Q39. The settings.xml file that provides the user-specific settings for Maven is contained in which directory by default?

- [ ] `${maven.home}/${user.name}/settings.xml`
- [x] `${user.home}/.m2/settings.xml`
- [ ] `${maven.home}/conf/settings.xml`
- [ ] `${user.home}/maven/settings.xml`

#### Q40. Suppose you are using Maven in a corporate environment and, to save bandwidth, you want to prevent the need for large numbers of developers to download the same dependency from the internet. What do you do to limit this?

- [x] Create an internal corporate repository to store copies of the necessary artifacts.
- [ ] It is not possible to do this.
- [ ] When defining the dependency, set the scope to provided.
- [ ] Each developer should define the dependency in the POM file in the local copy of the project.

#### Q41. In multimodule projects, what do child POMs inherit from the parent POM?

- [x] all of these answers
- [ ] dependencies
- [ ] groupId
- [ ] version

#### Q42. Below is a report generated for a multimodule project with the Checkstyle Plugin. Why might the highlighted links to the two child projects _not_ work?

![q43](q43.png?raw=png)

- [ ] The Checkstyle Plugin does not work on child modules.
- [ ] Each Checkstyle report is in the target/site folder of the respective module.
- [ ] All links in Checkstyle reports must be specified in the plugin definition.
- [ ] Checkstyle reports for child modules have to be behind a firewall.

#### Q43. Which build plugin allows you to create a "fat" JAR file that contains all of the dependencies in the final JAR file?

- [ ] Fatjar
- [x] Shade
- [ ] Dependency
- [ ] Package

#### Q44. What is the default scope for Maven dependencies?

- [ ] Test
- [x] Compile
- [ ] Runtime
- [ ] Build

#### Q45. How many times is compiler:compile called when executing mvn clean compile test package?

- [ ] one
- [ ] two
- [ ] none
- [ ] three

#### Q46. What is one of the advantages of using properties in Maven?

- [ ] Properties provide a template for you to build Maven projects with a certain structure.
- [ ] Properties allow you to inherit values from the parent POM in the child POM.
- [x] You can avoid hard-coding values in multiple places.
- [ ] Properties speed up your Maven build.

#### Q47. What are the phases of the clean lifecycle?

- [x] pre-clean, clean and post-clean
- [ ] Compile, clean and install
- [ ] clean and install
- [ ] validate, clean and deploy

#### Q48. A compile-time dependency of a dependency for your project is often called **a\_** dependency.

- [ ] Transitive
- [ ] runtime
- [ ] provided
- [ ] test

#### Q49. For what purpose can plugins use the validate phase in the default lifecycle?

- [ ] to check the parent POM file defines all of the child POM files
- [x] to carry out checks before building the project
- [ ] to ensure plugins defined in the POM file are in the correct order
- [ ] to check the project structure is correct after building a project

1. [stackoverflow](https://stackoverflow.com/a/40601037)
2. [maven docs](https://maven.apache.org/guides/introduction/introduction-to-the-lifecycle.html#a-build-lifecycle-is-made-up-of-phases)

#### Q50. How do you check for unused dependencies in your project?

- [ ] Run mvn clean and look at which plugins are not mentioned in the output.
- [ ] You will need to do this manually.
- [ ] Include the Maven dependency plugin in your POM file and run the unpack goal.
- [x] Run the analyze goal of the dependency plugin.

1. [baeldung](https://www.baeldung.com/maven-unused-dependencies)
2. [stackoverflow](https://stackoverflow.com/a/1518661)

#### Q51. Why is it best practice to avoid overriding the default directory structure?

- [ ] Keeping the default structure reduces onboarding time, because developers recognize it.
- [ ] Overriding the default structure is very complex.
- [ ] Overriding the default structure will cause Maven to take longer to compile your code.
- [x] all of these answers

[maven docs](https://maven.apache.org/guides/introduction/introduction-to-the-standard-directory-layout.html)

#### Q52. What is the main purpose of the install phase?

- [ ] to compile the source code of the project
- [ ] to install all of the remote dependencies
- [ ] to deploy the final project artifacts into a remote Maven repository
- [x] to copy the final project artifacts into the local Maven repository

[maven docs](https://maven.apache.org/guides/introduction/introduction-to-the-lifecycle.html#a-build-lifecycle-is-made-up-of-phases)

#### Q53. How do you skip the tests when running a mvn package command?

- [ ] Use -Dtest=skip
- [x] Use -DskipTests=true
- [ ] Use -Dtests=pass
- [ ] Use a plugin that can be configured to skip tests

#### Q54. Below is a section of a settings.xml file. How can you use the path to the app home in your POM file?

```
<profiles>
    <profile>
        <id>set=app-home</id>
        <properties>maven-people-plugin</artifactId>
            <application-home>/path/to/application</application-home>
        </properties>
    </profile>
</profiles>
<activeProfiles>
    <activeProfile>set-app-home</activeProfile>
</activeProfiles>
```

- [ ] ${activeProfile}
- [x] ${application-home}
- [ ] ${set-app-home}
- [ ] ${/path/to/application}

#### Q55. What is the default value of the warSourceDirectory configuration property of the Maven WAR Plugin?

- [ ] /src/main/webapp
- [ ] /src/main/war
- [x] /src/main/WEB-INF
- [ ] /src/web

#### Q56. When building a Maven Archetype, where do you put your prototype files?

- [ ] src/main/template
- [ ] src/main/archetype
- [x] src/main/resources/archetype-resources
- [ ] src/main/java

#### Q57. The primary purpose of Apache Maven is to provide uniform, easy, and standardized \_.

- [ ] versioning
- [ ] project structure
- [ ] source code style
- [x] builds

#### Q58. Below is the definition of a mirror in settings.xml. What does the element `<mirrorOf>\*</mirrorOf>` tell Maven to do?

```
<mirror>
    <id>internal-repo</id>
    <url>http://repo.mycompany.com/proxy</url>
    <mirrorOf>\*</mirrorOf>
</mirror>
```

- [ ] Use a single repository by having it mirror all repository requests.
- [x] Mirror all repositories except for http://repomycompany.com/proxy.
- [ ] Mirror any repositories with `\*` in the name.
- [ ] Use a mirror repository for every repository defined in the POM file.

#### Q59. How do you generate a site for a project with Maven?

- [x] Use the mvn site command.
- [ ] Use the mvn install command.
- [ ] This is not possible.
- [ ] Use the mvn package command.

#### Q60. What is the default location of the local Maven repository?

- [x] USER_HOME/.m2/repository
- [ ] USER_HOME/.m2/local
- [ ] USER_HOME/maven/repository
- [ ] /repo

#### Q61. A phase is a step in \_.

- [ ] the compile goal
- [ ] the development process
- [x] the build lifecycle
- [ ] the POM file

[maven docs](https://maven.apache.org/what-is-maven.html#:~:text=Maven's%20primary%20goal%20is%20to,Providing%20a%20uniform%20build%20system)

#### Q62. What is the Maven central repository?

- [ ] a local repository created by Maven in your local file system
- [ ] a repository in the middle of your Maven project
- [x] an online repository for open-source binaries
- [ ] a repository that you must download to build a Maven project

[!reference](https://www.javatpoint.com/maven-repository)

#### Q63. What are the artifacts that Apache Maven uses to perform its build operations?

- [ ] ant files
- [ ] properties
- [ ] dependencies
- [x] plugins

[!reference](https://maven.apache.org/guides/introduction/introduction-to-the-lifecycle.html)

#### Q64. Which plugin is used to copy, filter, include, and exclude non-Java files into your final project?

- [ ] Build
- [ ] Files
- [ ] Copy
- [x] Resources

[!reference](https://maven.apache.org/plugins/maven-resources-plugin/examples/include-exclude.html)

#### Q65. What is a module in a Maven project?

- [ ] a dependency
- [x] a subproject, or child project
- [ ] a Java package
- [ ] a plugin

[!reference](https://docs.jboss.org/tools/latest/en/maven_reference/html/creating_a_maven_application.html)

#### Q66. What does the mvn --version command do?

- [ ] It updates Maven to the latest version.
- [x] It prints out your installed version of Maven.
- [ ] It builds your Maven project.
- [ ] It installs Maven on your computer.

[!reference](https://jenkov.com/tutorials/maven/maven-commands.html)

#### Q67. When building a Maven project, where are Maven dependencies stored?

- [ ] in the target directory
- [x] in your local repository
- [ ] in the POM file
- [ ] online in the Maven central repository

[!reference](https://www.baeldung.com/maven-local-repository)

#### Q68. Why is it best practice not to release SNAPSHOT versions of Maven artifacts to production?

- [ ] A release marked with SNAPSHOT indicates that not all of the tests have passed.
- [x] A SNAPSHOT can be hard to reproduce, making it difficult to determine the cause of an issue.
- [ ] SNAPSHOT releases do not contain any dependencies.
- [ ] A release marked with SNAPSHOT may contain sensitive security information.

[!reference](https://maven.apache.org/guides/getting-started/index.html#What_is_a_SNAPSHOT_version)

#### Q69. Why do you use Maven Wrapper on a project shared with a large team of developers?

- [ ] all of these answers
- [x] All developers will be using the same Maven version, providing stability.
- [ ] The dependencies for the project will be downloaded only once for all developers, saving bandwidth.
- [ ] Maven Wrapper checks dependencies for vulnerabilities, increasing security.

#### Q70. This POM file contains an XML validation error. What is the cause of the error?

![q70](q70.png?raw=png)

- [ ] JUnit is not a valid dependency of a Maven project.
- [x] The `<dependency>` elements should be inside `<dependencies>` elements.
- [ ] The `<dependency>` element is not a valid in a POM file.
- [ ] The `<dependency>` elements should be at the bottom of the POM file.

#### Q71. Below is the configuration for a server on settings.xml. What does this configuration do?

![q71](q71.png?raw=png)

- [ ] It disables put requests to headers.
- [ ] It sets the headers for all GET requests.
- [ ] all of these answers
- [ ] It turns off the default behavior for headers and respecifies the Accept-Encoding header for the server with ID openssl.

#### Q72. Below is the build element of a parent POM file. Why might the resources not get copied when executing the plugin on a child project?

<img width="535" alt="5d697fe5498e21bcd2763c2a-1567198471328" src="https://user-images.githubusercontent.com/97866339/224229468-989d52e7-c3d3-4ff2-9514-a38e71d56b7d.png">

- [ ] Plugins defined in the pluginManagement element can never be executed.
- [ ] Plugins defined in the parent POM are not available in the child POM.
- [ ] The Build Helper Maven Plugin works only on parent projects.
- [ ] The plugin may not have been defined in the child POM.

[maven docs](https://maven.apache.org/guides/mini/guide-http-settings.html#taking-control-of-your-http-headers)
