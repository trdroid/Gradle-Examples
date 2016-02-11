http://gradle.org/gradle-download/

The gradle download is packaged with its own Groovy library so any existing groovy installation on the system is ignored.

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

### Installation Directory

<img src="_misc/Gradle%20installation%20directory.png"/>

<i>gradle/init.d/readme.txt</i>

```text
You can add .gradle init scripts to this directory. Each one is executed at the start of the build.
```

Add functionality that is needed for every gradle build here. Examples include gradle scripts to checkout source code before starting the build process, to start a process to clear out a database etc. 
