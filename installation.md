http://gradle.org/gradle-download/

The gradle download is packaged with its own Groovy library so any existing groovy installation on the system is ignored.

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

