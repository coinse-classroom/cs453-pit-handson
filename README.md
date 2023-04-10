## Mutation Testing with PIT Hands-on

### [PIT](https://pitest.org)

PIT is a mutation testing tool developed by Henry Coles, a professional softeware developer. It is unique because it is NOT an academic prototype.

Please refer to its documentation, especially its integration to build tools such as [Maven](https://pitest.org/quickstart/maven/) and [Gradle](http://gradle-pitest-plugin.solidsoft.info). Download and install PIT from the URL above.

### Instructions

We will use two Apache Commons projects, [Math](https://commons.apache.org/proper/commons-math/) and [Lang](https://commons.apache.org/proper/commons-lang/). Download the latest source code for each of these projects.

1. Build the target projects using Maven.
2. Using the Maven plugin, integrate PIT into the build. It is recommended that you narrow down the scope of PIT using the `targetClasses` parameter.
3. Execute PITest, and generate the report.
4. Consult the report, and find a mutant that is not killed.
5. Improve the test suite, so that you kill the mutant from Step 4.