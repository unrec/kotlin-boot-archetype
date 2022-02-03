# kotlin-boot-archetype
1. Clone the repository to local machine. 
2. Enter the repository folder and run `mvn clean install` to put the archetype in your local repository.
3. Enter the root folder where you want to create new project.
4. Run command `mvn archetype: generate` with next parameters:
   * -DarchetypeGroupId=com.unrec
   * -DarchetypeArtifactId=kotlin-boot-archetype
   * -DarchetypeVersion=1.0-SNAPSHOT
   * -DgroupId=com.unrec - **enter desired project base package**
   * -DartifactId=rest-test-project - **enter desired project name**
   * -DarchetypeCatalog=local - flag to use local repository for archetype look-up.
    
Example: `mvn archetype:generate -DarchetypeGroupId=com.unrec -DarchetypeArtifactId=kotlin-boot-archetype -DarchetypeVersion=1.0-SNAPSHOT -DgroupId=com.unrec -DartifactId=rest-test-project -DarchetypeCatalog=local
`.

Put parameters in double-quotes while using PowerShell: `mvn archetype:generate "-DarchetypeGroupId=com.unrec" "-DarchetypeArtifactId=kotlin-boot-archetype" "-DarchetypeVersion=1.0-SNAPSHOT" "-DgroupId=com.unrec" "-DartifactId=rest-test-project" "-DarchetypeCatalog=local"`.

5. Follow Maven instructions and provide non-default values if required.