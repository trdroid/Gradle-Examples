## Installation on Ubuntu

### Prerequisites
* Java JDK 1.5+

<b> Maintaining Multiple versions of Gradle </b>

Install sdkman to manage multiple versions of Gradle. (http://sdkman.io/)

> $ curl -s get.sdkman.io | bash

    Thanks for using...                                            		         
                                                                   		         
                                                                   		         
         SSSSSSSSSSSSSSS DDDDDDDDDDDDD       KKKKKKKKK    KKKKKKK                  
       SS:::::::::::::::SD::::::::::::DDD    K:::::::K    K:::::K                  
      S:::::SSSSSS::::::SD:::::::::::::::DD  K:::::::K    K:::::K                  
      S:::::S     SSSSSSSDDD:::::DDDDD:::::D K:::::::K   K::::::K                  
      S:::::S              D:::::D    D:::::DKK::::::K  K:::::KKK                  
      S:::::S              D:::::D     D:::::D K:::::K K:::::K                     
       S::::SSSS           D:::::D     D:::::D K::::::K:::::K                      
        SS::::::SSSSS      D:::::D     D:::::D K:::::::::::K                       
          SSS::::::::SS    D:::::D     D:::::D K:::::::::::K                       
             SSSSSS::::S   D:::::D     D:::::D K::::::K:::::K                      
                  S:::::S  D:::::D     D:::::D K:::::K K:::::K                     
                  S:::::S  D:::::D    D:::::DKK::::::K  K:::::KKK                  
      SSSSSSS     S:::::SDDD:::::DDDDD:::::D K:::::::K   K::::::K                  
      S::::::SSSSSS:::::SD:::::::::::::::DD  K:::::::K    K:::::K                  
      S:::::::::::::::SS D::::::::::::DDD    K:::::::K    K:::::K                  
       SSSSSSSSSSSSSSS   DDDDDDDDDDDDD       KKKKKKKKK    KKKKKKK                  
                                                                                   
                                                                                   
                          mmmmmmm    mmmmmmm     aaaaaaaaaaaaa  nnnn  nnnnnnnn     
                        mm:::::::m  m:::::::mm   a::::::::::::a n:::nn::::::::nn   
                       m::::::::::mm::::::::::m  aaaaaaaaa:::::an::::::::::::::nn  
                       m::::::::::::::::::::::m           a::::ann:::::::::::::::n 
                       m:::::mmm::::::mmm:::::m    aaaaaaa:::::a  n:::::nnnn:::::n 
                       m::::m   m::::m   m::::m  aa::::::::::::a  n::::n    n::::n 
                       m::::m   m::::m   m::::m a::::aaaa::::::a  n::::n    n::::n 
                       m::::m   m::::m   m::::ma::::a    a:::::a  n::::n    n::::n 
                       m::::m   m::::m   m::::ma::::a    a:::::a  n::::n    n::::n 
                       m::::m   m::::m   m::::ma:::::aaaa::::::a  n::::n    n::::n 
                       m::::m   m::::m   m::::m a::::::::::aa:::a n::::n    n::::n 
                       mmmmmm   mmmmmm   mmmmmm  aaaaaaaaaa  aaaa nnnnnn    nnnnnn 
                								                                     
                								                                     
                                                     Now attempting installation...
                                                                                   
    Looking for a previous installation of SDKMAN...
    Looking for unzip...
    Looking for curl...
    Looking for sed...
    Installing SDKMAN scripts...
    Create distribution directories...
    Getting available candidates...
    Prime the config file...
    Download script archive...
    Extract script archive...
    Install scripts...
    Set version to 3.3.2 ...
    Attempt update of bash profiles...
    Updated existing /home/droid/.bash_profile
    Updated existing /home/droid/.profile
    Updated existing /home/droid/.bashrc
    Attempt update of zsh profiles...
    Updated existing /home/droid/.zshrc
    
    
    
    All done!
    
    
    Please open a new terminal, or run the following in the existing one:
    
        source "/home/droid/.sdkman/bin/sdkman-init.sh"
    
    Then issue the following command:
    
        sdk help
    
    Enjoy!!!

> $ source "/home/droid/.sdkman/bin/sdkman-init.sh"

> $ sdk version

    ==== BROADCAST =================================================================
    * 08/02/16: Gradle 2.11 released on SDKMAN! #gradle
    * 06/02/16: Vertx 3.2.1 released on SDKMAN! #vertx
    * 04/02/16: Kotlin 1.0.0-rc-1036 released on SDKMAN! #kotlin
    ================================================================================
    SDKMAN 3.3.2

Check what versions of gradle are available:

> $ sdk list gradle

        ================================================================================
        Available Gradle Versions
        ================================================================================
             2.9                  2.0                  0.9.1                               
             2.8                  1.9                  0.9                                 
             2.7                  1.8                  0.8                                 
             2.6                  1.7                  0.7                                 
             2.5                  1.6                                                      
             2.4                  1.5                                                      
             2.3                  1.4                                                      
             2.2.1                1.3                                                      
             2.2                  1.2                                                      
             2.11-rc-3            1.12                                                     
             2.11-rc-2            1.11                                                     
             2.11-rc-1            1.10                                                     
             2.11                 1.1                                                      
             2.10                 1.0                                                      
             2.1                  0.9.2                                                    
        
        ================================================================================
        + - local version
        * - installed
        > - currently in use
        ================================================================================

<b>Install Gradle</b>

> $ sdk install gradle 2.11

        Downloading: gradle 2.11
        
          % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                         Dload  Upload   Total   Spent    Left  Speed
          0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0
          0     0    0   355    0     0    527      0 --:--:-- --:--:-- --:--:--  1119
        100 44.7M  100 44.7M    0     0   744k      0  0:01:01  0:01:01 --:--:-- 1703k
        
        Installing: gradle 2.11
        Done installing!
        
        Do you want gradle 2.11 to be set as default? (Y/n): Y
        
        Setting gradle 2.11 as default.

> $ which gradle

        /home/droid/.sdkman/candidates/gradle/current/bin/gradle

> droid@droidserver:~$ gradle --version

        ------------------------------------------------------------
        Gradle 2.11
        ------------------------------------------------------------
        
        Build time:   2016-02-08 07:59:16 UTC
        Build number: none
        Revision:     584db1c7c90bdd1de1d1c4c51271c665bfcba978
        
        Groovy:       2.4.4
        Ant:          Apache Ant(TM) version 1.9.3 compiled on December 23 2013
        JVM:          1.8.0_65 (Oracle Corporation 25.65-b01)
        OS:           Linux 3.16.0-60-generic amd64


$GRADLE_HOME is set for you.

> echo $GRADLE_HOME

        /home/droid/.sdkman/candidates/gradle/current

<b> Installation Directory </b>

<img src="_misc/Gradle%20installation%20directory.png"/>

<i>current/lib</i>

This directory contains all dependencies (plugins, jar files) that gradle needs. 

> ~/.sdkman/candidates/gradle/current$ ls lib

    ant-1.9.3.jar                  gradle-base-services-groovy-2.11.jar  gradle-native-2.11.jar       jansi-1.2.1.jar            kryo-2.20.jar                           native-platform-osx-amd64-0.10.jar
    ant-launcher-1.9.3.jar         gradle-cli-2.11.jar                   gradle-open-api-2.11.jar     jarjar-1.3.jar             log4j-over-slf4j-1.7.10.jar             native-platform-osx-i386-0.10.jar
    asm-all-5.0.3.jar              gradle-core-2.11.jar                  gradle-resources-2.11.jar    javax.inject-1.jar         minlog-1.2.jar                          native-platform-windows-amd64-0.10.jar
    commons-collections-3.2.1.jar  gradle-docs-2.11.jar                  gradle-tooling-api-2.11.jar  jaxen-1.1.jar              native-platform-0.10.jar                native-platform-windows-i386-0.10.jar
    commons-io-2.2.jar             gradle-launcher-2.11.jar              gradle-ui-2.11.jar           jcip-annotations-1.0.jar   native-platform-freebsd-amd64-0.10.jar  objenesis-1.2.jar
    commons-lang-2.6.jar           gradle-messaging-2.11.jar             gradle-wrapper-2.11.jar      jcl-over-slf4j-1.7.10.jar  native-platform-freebsd-i386-0.10.jar   plugins
    dom4j-1.6.1.jar                gradle-model-core-2.11.jar            groovy-all-2.4.4.jar         jna-3.2.7.jar              native-platform-linux-amd64-0.10.jar    reflectasm-1.07-shaded.jar
    gradle-base-services-2.11.jar  gradle-model-groovy-2.11.jar          guava-jdk5-17.0.jar          jul-to-slf4j-1.7.10.jar    native-platform-linux-i386-0.10.jar     slf4j-api-1.7.10.jar


> ~/.sdkman/candidates/gradle/current$ ls lib/plugins

    aether-api-1.13.1.jar                  gradle-ear-2.11.jar                 gradle-resources-http-2.11.jar        jetty-annotations-6.1.25.jar            plexus-container-default-1.5.5.jar
    aether-connector-wagon-1.13.1.jar      gradle-ide-2.11.jar                 gradle-resources-s3-2.11.jar          jetty-naming-6.1.25.jar                 plexus-interpolation-1.14.jar
    aether-impl-1.13.1.jar                 gradle-ide-native-2.11.jar          gradle-resources-sftp-2.11.jar        jetty-plus-6.1.25.jar                   plexus-sec-dispatcher-1.3.jar
    aether-spi-1.13.1.jar                  gradle-ivy-2.11.jar                 gradle-scala-2.11.jar                 jetty-util-6.1.25.jar                   plexus-utils-2.0.6.jar
    aether-util-1.13.1.jar                 gradle-jacoco-2.11.jar              gradle-signing-2.11.jar               joda-time-2.8.2.jar                     pmaven-common-0.8-20100325.jar
    aws-java-sdk-core-1.9.19.jar           gradle-javascript-2.11.jar          gradle-sonar-2.11.jar                 jsch-0.1.53.jar                         pmaven-groovy-0.8-20100325.jar
    aws-java-sdk-kms-1.9.19.jar            gradle-jetty-2.11.jar               gradle-testing-base-2.11.jar          jsp-2.1-6.1.14.jar                      rhino-1.7R3.jar
    aws-java-sdk-s3-1.9.19.jar             gradle-language-groovy-2.11.jar     gradle-testing-jvm-2.11.jar           jsp-api-2.1-6.1.14.jar                  servlet-api-2.5-20081211.jar
    bcpg-jdk15on-1.51.jar                  gradle-language-java-2.11.jar       gradle-testing-native-2.11.jar        junit-4.12.jar                          simple-4.1.21.jar
    bcprov-jdk15on-1.51.jar                gradle-language-jvm-2.11.jar        gradle-test-kit-2.11.jar              maven-aether-provider-3.0.4.jar         snakeyaml-1.6.jar
    bndlib-2.4.0.jar                       gradle-language-native-2.11.jar     gradle-tooling-api-builders-2.11.jar  maven-artifact-3.0.4.jar                sonar
    bsh-2.0b4.jar                          gradle-language-scala-2.11.jar      gson-2.2.4.jar                        maven-compat-3.0.4.jar                  sonar-batch-bootstrapper-2.9.jar
    commons-cli-1.2.jar                    gradle-maven-2.11.jar               hamcrest-core-1.3.jar                 maven-core-3.0.4.jar                    testng-6.3.1.jar
    commons-codec-1.6.jar                  gradle-osgi-2.11.jar                httpclient-4.4.1.jar                  maven-model-3.0.4.jar                   wagon-file-2.4.jar
    core-3.1.1.jar                         gradle-platform-base-2.11.jar       httpcore-4.4.4.jar                    maven-model-builder-3.0.4.jar           wagon-http-2.4.jar
    geronimo-annotation_1.0_spec-1.0.jar   gradle-platform-jvm-2.11.jar        ivy-2.2.0.jar                         maven-plugin-api-3.0.4.jar              wagon-http-shared4-2.4.jar
    gradle-announce-2.11.jar               gradle-platform-native-2.11.jar     jackson-annotations-2.3.2.jar         maven-repository-metadata-3.0.4.jar     wagon-provider-api-2.4.jar
    gradle-antlr-2.11.jar                  gradle-platform-play-2.11.jar       jackson-core-2.3.2.jar                maven-settings-3.0.4.jar                xbean-reflect-3.4.jar
    gradle-build-comparison-2.11.jar       gradle-plugin-development-2.11.jar  jackson-databind-2.3.2.jar            maven-settings-builder-3.0.4.jar        xercesImpl-2.9.1.jar
    gradle-build-init-2.11.jar             gradle-plugins-2.11.jar             jatl-0.2.2.jar                        nekohtml-1.9.14.jar                     xml-apis-1.3.04.jar
    gradle-code-quality-2.11.jar           gradle-plugin-use-2.11.jar          jcifs-1.3.17.jar                      plexus-cipher-1.7.jar
    gradle-dependency-management-2.11.jar  gradle-publish-2.11.jar             jcommander-1.12.jar                   plexus-classworlds-2.4.jar
    gradle-diagnostics-2.11.jar            gradle-reporting-2.11.jar           jetty-6.1.25.jar                      plexus-component-annotations-1.5.5.jar


<i>current/init.d/readme.txt</i>

```text
You can add .gradle init scripts to this directory. Each one is executed at the start of the build.
```

Add functionality that is needed for every gradle build here. Examples include gradle scripts to checkout source code before starting the build process, to start a process to clear out a database etc. 

### Manual Installation

http://gradle.org/gradle-download/

The gradle download is packaged with its own Groovy library so any existing groovy installation on the system is ignored.

<b> Gradle download Directory </b>

<img src="_misc/manual%20download%20project%20directory.png"/>

<i>gradle-2.11/samples</i>

> ~/software/gradle/gradle-2.11$ ls samples

    announce        clientModuleDependencies  customBuildLanguage  dependency-substitution  idea         javaGradlePlugin   maven-publish         osgi     signing      testing     webApplication
    antlr           codeQuality               customDistribution   ear                      ivypublish   javaLibraryPlugin  modelRules            play     sonar        testKit
    application     componentMetadataRules    customModel          eclipse                  ivy-publish  jvmComponents      multiProjectBuildSrc  plugins  sonarRunner  toolingApi
    buildDashboard  componentSelectionRules   customPlugin         groovy                   java         maven              native-binaries       scala    src          userguide

