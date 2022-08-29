# Pre-Requisites
This section describes the pre-requisites setup to be done.
Please proceed with the below steps.

## Software List
1. [Github Desktop](#1-github-desktop)
2. [Java](#2-java)
3. [Apache Maven](#3-apache-maven)
4. [Spring Tool Suite](#4-spring-tool-suite)


## 1. Github Desktop
1. Create a new account in [https://github.com](https://github.com) and link it to your personal email account.
2. Goto [https://desktop.github.com/](https://desktop.github.com/) and download the version suitable for your Operating System.
3. Install the downloaded file and sign-in using your github account created in `step-1`


## 2. Java
Install Java 11 and setup the `JAVA_HOME` environment variable in system parameters using the below steps

### 2.1. Installation
1. Download JDK 11 from [https://download.java.net/openjdk/jdk11/ri/openjdk-11+28_windows-x64_bin.zip](https://download.java.net/openjdk/jdk11/ri/openjdk-11+28_windows-x64_bin.zip)
2. Extract this zip into a local folder like `c:\software\java`. After extracting this zip file, `jdk-11` folder is now available.

### 2.2. JAVA_HOME configuration
3. In windows, click on Settings icon in the Start menu, and search for `Environment Variable`. 
   - Select the link to `Edit the System Environment Variables`
   - Click on the `Environment Variables button` to open the `Environment Variables window`.
4. Inside the System Parameters, add `JAVA_HOME=<jdk-11 folder path>` eg., `c:\software\java\jdk-11`
5. Update the `Path` parameter and add `%JAVA_HOME%/bin` to the top of the list
6. Save and exit the system variables windows

### 2.3. Verify Installation
7. Open a new command line window and execute the command `java -version` to check the Java version installed



## 3. Apache Maven
Install Apache Maven 3.8.6 and setup the `MAVEN_HOME` environment variable in system parameters using the below steps

### 3.1. Installation
1. Make sure the Java installation is completed successfully, and JAVA_HOME is also configured correctly.
2. Go to the url [https://maven.apache.org/download.cgi](https://maven.apache.org/download.cgi)
   - Download the file `apache-maven-3.8.6-bin.zip` from the Binary Zip Archive section link column.
3. Extract this zip into a local folder like `c:\software\maven`.

### 3.2. MAVEN_HOME configuration
4. Inside the System Parameters, add `MAVEN_HOME=c:\software\maven`
5. Update the `Path` parameter and add `%MAVEN_HOME%/bin` as 2nd item in the list
6. Save and exit the system variables windows

### 3.3. Verify Installation
7. Open a new command line window and execute the command `mvn --version` to check the Maven version installed



## 4. Spring Tool Suite
### 4.1. Installation
1. Goto the website [https://spring.io/tools](https://spring.io/tools)
2. Select the software based on the OS version and download the `.jar` file to the location - `c:\software\sts`
   Sample filename  -`spring-tool-suite-4-4.15.3.RELEASE-e4.24.0-win32.win32.x86_64.self-extracting.jar`
4. Double click this file to begin extraction (if not extracting then goto `step 4`)
5. In command line goto the path - `c:\software\sts` and execute the command `java -jar <jar filename>`. 
   This will start the extraction and a progress bar will appear to show the progress.
6. Once the extraction is completed, the folder `sts-{4.x.x}.RELEASE` appears in this location.
   - Go into this folder and double click `SpringToolSuite4.exe` to start the STS editor.
   - When asked to create a workspace, create a new directory `c:\mywork\sts_workspace` and provide this path as workspace path. 
   - Select the checkbox - `Use this as default and do not ask again`.
   - Click `Launch` to complete the installation, and STS will open now.

### 4.2. Configuration
4. Goto `Windows menu -> Preferences -> Java`
5. Click on `Compiler`, set the `Compiler Compliance Level = 11`
6. Click on `Installed JRE`, verify if the JRE is available by default
7. Click on `Maven -> Installations`, click on the `Add` button
   - `Installation home: ` - Select the Maven home path and clink on `Finish` button
8. Select the checkbox for the `apache-maven-{3.x.x}` in the Installations list
9. Apply and Close to complete the configuration


