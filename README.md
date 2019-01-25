## Environment

```
[root@ip-172-31-21-135 ~]# cat /etc/os-release 
NAME="Amazon Linux AMI"
VERSION="2018.03"
ID="amzn"
ID_LIKE="rhel fedora"
VERSION_ID="2018.03"
PRETTY_NAME="Amazon Linux AMI 2018.03"
ANSI_COLOR="0;33"
CPE_NAME="cpe:/o:amazon:linux:2018.03:ga"
HOME_URL="http://aws.amazon.com/amazon-linux-ami/"
[root@ip-172-31-21-135 ~]# cat /etc/issue
Amazon Linux AMI release 2018.03
Kernel \r on an \m

[root@ip-172-31-21-135 ~]# 
```

## パッケージ更新
```
# yum check-update
# yum update -y
```

```
$ git clone https://github.com/spring-guides/gs-spring-boot.git
$ cd gs-spring-boot/complete/
```

# sdk install

```
$ curl -s "https://get.sdkman.io" | bash

                                -+syyyyyyys:
                            `/yho:`       -yd.
                         `/yh/`             +m.
                       .oho.                 hy                          .`
                     .sh/`                   :N`                `-/o`  `+dyyo:.
                   .yh:`                     `M-          `-/osysoym  :hs` `-+sys:      hhyssssssssy+
                 .sh:`                       `N:          ms/-``  yy.yh-      -hy.    `.N-````````+N.
               `od/`                         `N-       -/oM-      ddd+`     `sd:     hNNm        -N:
              :do`                           .M.       dMMM-     `ms.      /d+`     `NMMs       `do
            .yy-                             :N`    ```mMMM.      -      -hy.       /MMM:       yh
          `+d+`           `:/oo/`       `-/osyh/ossssssdNMM`           .sh:         yMMN`      /m.
         -dh-           :ymNMMMMy  `-/shmNm-`:N/-.``   `.sN            /N-         `NMMy      .m/
       `oNs`          -hysosmMMMMydmNmds+-.:ohm           :             sd`        :MMM/      yy
      .hN+           /d:    -MMMmhs/-.`   .MMMh   .ss+-                 `yy`       sMMN`     :N.
     :mN/           `N/     `o/-`         :MMMo   +MMMN-         .`      `ds       mMMh      do
    /NN/            `N+....--:/+oooosooo+:sMMM:   hMMMM:        `my       .m+     -MMM+     :N.
   /NMo              -+ooooo+/:-....`...:+hNMN.  `NMMMd`        .MM/       -m:    oMMN.     hs
  -NMd`                                    :mm   -MMMm- .s/     -MMm.       /m-   mMMd     -N.
 `mMM/                                      .-   /MMh. -dMo     -MMMy        od. .MMMs..---yh
 +MMM.                                           sNo`.sNMM+     :MMMM/        sh`+MMMNmNm+++-
 mMMM-                                           /--ohmMMM+     :MMMMm.       `hyymmmdddo
 MMMMh.                  ````                  `-+yy/`yMMM/     :MMMMMy       -sm:.``..-:-.`
 dMMMMmo-.``````..-:/osyhddddho.           `+shdh+.   hMMM:     :MmMMMM/   ./yy/` `:sys+/+sh/
 .dMMMMMMmdddddmmNMMMNNNNNMMMMMs           sNdo-      dMMM-  `-/yd/MMMMm-:sy+.   :hs-      /N`
  `/ymNNNNNNNmmdys+/::----/dMMm:          +m-         mMMM+ohmo/.` sMMMMdo-    .om:       `sh
     `.-----+/.`       `.-+hh/`         `od.          NMMNmds/     `mmy:`     +mMy      `:yy.
           /moyso+//+ossso:.           .yy`          `dy+:`         ..       :MMMN+---/oys:
         /+m:  `.-:::-`               /d+                                    +MMMMMMMNh:`
        +MN/                        -yh.                                     `+hddhy+.
       /MM+                       .sh:
      :NMo                      -sh/
     -NMs                    `/yy:
    .NMy                  `:sh+.
   `mMm`               ./yds-
  `dMMMmyo:-.````.-:oymNy:`
  +NMMMMMMMMMMMMMMMMms:`
    -+shmNMMMNmdy+:`


                                                                 Now attempting installation...


Looking for a previous installation of SDKMAN...
Looking for unzip...
Looking for zip...
Looking for curl...
Looking for sed...
Installing SDKMAN scripts...
Create distribution directories...
Getting available candidates...
Prime the config file...
Download script archive...
######################################################################## 100.0%
Extract script archive...
Install scripts...
Set version to 5.7.3+337 ...
Attempt update of interactive bash profile on regular UNIX...
Added sdkman init snippet to /home/ec2-user/.bashrc
Attempt update of zsh profile...
Updated existing /home/ec2-user/.zshrc



All done!


Please open a new terminal, or run the following in the existing one:

    source "/home/ec2-user/.sdkman/bin/sdkman-init.sh"

Then issue the following command:

    sdk help

Enjoy!!!
```

sdkコマンドの反映

```
$ source "/home/ec2-user/.sdkman/bin/sdkman-init.sh"
```

```
$ sdk version
==== BROADCAST =================================================================
* 23/01/19: Kotlin 1.3.20 released on SDKMAN! #kotlin
* 12/01/19: Springboot 2.1.2.RELEASE released on SDKMAN! #springboot
* 11/01/19: Springboot 2.0.8.RELEASE released on SDKMAN! #springboot
================================================================================

SDKMAN 5.7.3+337
```


gradleのリスト表示、最新版をインストールする

```
$ sdk list gradle
================================================================================
Available Gradle Versions
================================================================================
     5.1.1               4.3                 2.14                1.11           
     5.1                 4.2.1               2.13                1.10           
     5.0                 4.2                 2.12                1.9            
     4.10.3              4.1                 2.11                1.8            
     4.10.2              4.0.2               2.10                1.7            
     4.10.1              4.0.1               2.9                 1.6            
     4.10                4.0                 2.8                 1.5            
     4.9                 3.5.1               2.7                 1.4            
     4.8.1               3.5                 2.6                 1.3            
     4.8                 3.4.1               2.5                 1.2            
     4.7                 3.4                 2.4                 1.1            
     4.6                 3.3                 2.3                 1.0            
     4.5.1               3.2.1               2.2.1               0.9.2          
     4.5                 3.2                 2.2                 0.9.1          
     4.4.1               3.1                 2.1                 0.9            
     4.4                 3.0                 2.0                 0.8            
     4.3.1               2.14.1              1.12                0.7            

================================================================================
+ - local version
* - installed
> - currently in use
================================================================================
``` 


gradleのインストール

```
$ sdk install gradle 5.1.1

Downloading: gradle 5.1.1

In progress...

######################################################################## 100.0%

Installing: gradle 5.1.1
Done installing!


Setting gradle 5.1.1 as default.
```


```
$ sdk current

Using:

gradle: 5.1.1
```

元から入っているjavaを削除

```
[root@ip-172-31-21-135 ~]# yum remove java
Loaded plugins: priorities, update-motd, upgrade-helper
Resolving Dependencies
--> Running transaction check
---> Package java-1.7.0-openjdk.x86_64 1:1.7.0.201-2.6.16.0.78.amzn1 will be erased
--> Processing Dependency: java-1.7.0-openjdk = 1:1.7.0.201-2.6.16.0.78.amzn1 for package: 1:java-1.7.0-openjdk-devel-1.7.0.201-2.6.16.0.78.amzn1.x86_64
--> Processing Dependency: jre >= 1.6.0 for package: aws-apitools-mon-1.0.20.0-1.0.amzn1.noarch
--> Processing Dependency: jre >= 1.6.0 for package: aws-apitools-elb-1.0.35.0-1.0.amzn1.noarch
--> Processing Dependency: jre >= 1.6.0 for package: aws-apitools-common-1.1.0-1.9.amzn1.noarch
--> Processing Dependency: jre >= 1.6.0 for package: aws-apitools-ec2-1.7.3.0-1.0.amzn1.noarch
--> Processing Dependency: jre >= 1.6.0 for package: aws-apitools-as-1.0.61.6-1.0.amzn1.noarch
---> Package jdk-11.0.2.x86_64 2000:11.0.2-ga will be erased
--> Running transaction check
---> Package aws-apitools-as.noarch 0:1.0.61.6-1.0.amzn1 will be erased
---> Package aws-apitools-common.noarch 0:1.1.0-1.9.amzn1 will be erased
---> Package aws-apitools-ec2.noarch 0:1.7.3.0-1.0.amzn1 will be erased
---> Package aws-apitools-elb.noarch 0:1.0.35.0-1.0.amzn1 will be erased
---> Package aws-apitools-mon.noarch 0:1.0.20.0-1.0.amzn1 will be erased
---> Package java-1.7.0-openjdk-devel.x86_64 1:1.7.0.201-2.6.16.0.78.amzn1 will be erased
--> Finished Dependency Resolution

Dependencies Resolved

====================================================================================================================================================
 Package                                  Arch                   Version                                        Repository                     Size
====================================================================================================================================================
Removing:
 java-1.7.0-openjdk                       x86_64                 1:1.7.0.201-2.6.16.0.78.amzn1                  @amzn-updates                  91 M
 jdk-11.0.2                               x86_64                 2000:11.0.2-ga                                 installed                     288 M
Removing for dependencies:
 aws-apitools-as                          noarch                 1.0.61.6-1.0.amzn1                             installed                     7.1 M
 aws-apitools-common                      noarch                 1.1.0-1.9.amzn1                                installed                     915  
 aws-apitools-ec2                         noarch                 1.7.3.0-1.0.amzn1                              installed                      17 M
 aws-apitools-elb                         noarch                 1.0.35.0-1.0.amzn1                             installed                     7.8 M
 aws-apitools-mon                         noarch                 1.0.20.0-1.0.amzn1                             installed                     6.9 M
 java-1.7.0-openjdk-devel                 x86_64                 1:1.7.0.201-2.6.16.0.78.amzn1                  @amzn-updates                  36 M

Transaction Summary
====================================================================================================================================================
Remove  2 Packages (+6 Dependent packages)

Installed size: 454 M
Is this ok [y/N]: y
Downloading packages:
Running transaction check
Running transaction test
Transaction test succeeded
Running transaction
  Erasing    : aws-apitools-mon-1.0.20.0-1.0.amzn1.noarch                                                                                       1/8 
  Erasing    : aws-apitools-as-1.0.61.6-1.0.amzn1.noarch                                                                                        2/8 
  Erasing    : aws-apitools-elb-1.0.35.0-1.0.amzn1.noarch                                                                                       3/8 
  Erasing    : aws-apitools-ec2-1.7.3.0-1.0.amzn1.noarch                                                                                        4/8 
  Erasing    : aws-apitools-common-1.1.0-1.9.amzn1.noarch                                                                                       5/8 
  Erasing    : 2000:jdk-11.0.2-11.0.2-ga.x86_64                                                                                                 6/8 
  Erasing    : 1:java-1.7.0-openjdk-devel-1.7.0.201-2.6.16.0.78.amzn1.x86_64                                                                    7/8 
failed to read link /usr/bin/javac: No such file or directory
  Erasing    : 1:java-1.7.0-openjdk-1.7.0.201-2.6.16.0.78.amzn1.x86_64                                                                          8/8 
  Verifying  : 2000:jdk-11.0.2-11.0.2-ga.x86_64                                                                                                 1/8 
  Verifying  : 1:java-1.7.0-openjdk-devel-1.7.0.201-2.6.16.0.78.amzn1.x86_64                                                                    2/8 
  Verifying  : aws-apitools-common-1.1.0-1.9.amzn1.noarch                                                                                       3/8 
  Verifying  : aws-apitools-ec2-1.7.3.0-1.0.amzn1.noarch                                                                                        4/8 
  Verifying  : 1:java-1.7.0-openjdk-1.7.0.201-2.6.16.0.78.amzn1.x86_64                                                                          5/8 
  Verifying  : aws-apitools-elb-1.0.35.0-1.0.amzn1.noarch                                                                                       6/8 
  Verifying  : aws-apitools-as-1.0.61.6-1.0.amzn1.noarch                                                                                        7/8 
  Verifying  : aws-apitools-mon-1.0.20.0-1.0.amzn1.noarch                                                                                       8/8 

Removed:
  java-1.7.0-openjdk.x86_64 1:1.7.0.201-2.6.16.0.78.amzn1                              jdk-11.0.2.x86_64 2000:11.0.2-ga                             

Dependency Removed:
  aws-apitools-as.noarch 0:1.0.61.6-1.0.amzn1                      aws-apitools-common.noarch 0:1.1.0-1.9.amzn1                                     
  aws-apitools-ec2.noarch 0:1.7.3.0-1.0.amzn1                      aws-apitools-elb.noarch 0:1.0.35.0-1.0.amzn1                                     
  aws-apitools-mon.noarch 0:1.0.20.0-1.0.amzn1                     java-1.7.0-openjdk-devel.x86_64 1:1.7.0.201-2.6.16.0.78.amzn1                    

Complete!
[root@ip-172-31-21-135 ~]# 
```


```
# wget --no-check-certificate --no-cookies --header "Cookie: oraclelicense=accept-securebackup-cookie" http://download.oracle.com/otn-pub/java/jdk/11.0.2+9/f51449fcd52f4d52b93a989c5c56ed3c/jdk-11.0.2_linux-x64_bin.rpm

[root@ip-172-31-21-135 ~]# rpm -ivh jdk-11.0.2_linux-x64_bin.rpm 
warning: jdk-11.0.2_linux-x64_bin.rpm: Header V3 RSA/SHA256 Signature, key ID ec551f03: NOKEY
Preparing...                          ################################# [100%]
Updating / installing...
   1:jdk-11.0.2-2000:11.0.2-ga        ################################# [100%]
[root@ip-172-31-21-135 ~]# 
```

## jdk8のインストール

jdkダウンロード

```
# wget --no-check-certificate --no-cookies --header "Cookie: oraclelicense=accept-securebackup-cookie" https://download.oracle.com/otn-pub/java/jdk/8u202-b08/1961070e4c9b4e26a04e7f5a083f551e/jdk-8u202-linux-x64.rpm
```

jdkインストール

```
[root@ip-172-31-21-135 ~]# rpm -ivh jdk-8u202-linux-x64.rpm 
warning: jdk-8u202-linux-x64.rpm: Header V3 RSA/SHA256 Signature, key ID ec551f03: NOKEY
Preparing...                          ################################# [100%]
Updating / installing...
   1:jdk1.8-2000:1.8.0_202-fcs        ################################# [100%]
Unpacking JAR files...
        tools.jar...
        plugin.jar...
        javaws.jar...
        deploy.jar...
        rt.jar...
        jsse.jar...
        charsets.jar...
        localedata.jar...
[root@ip-172-31-21-135 ~]# 
```





下記コマンドのように出力されている場合成功

```
$ gradle -v

Welcome to Gradle 5.1.1!

Here are the highlights of this release:
 - Control which dependencies can be retrieved from which repositories
 - Production-ready configuration avoidance APIs

For more details see https://docs.gradle.org/5.1.1/release-notes.html


------------------------------------------------------------
Gradle 5.1.1
------------------------------------------------------------

Build time:   2019-01-10 23:05:02 UTC
Revision:     3c9abb645fb83932c44e8610642393ad62116807

Kotlin DSL:   1.1.1
Kotlin:       1.3.11
Groovy:       2.5.4
Ant:          Apache Ant(TM) version 1.9.13 compiled on July 10 2018
JVM:          11.0.2 (Oracle Corporation 11.0.2+9-LTS)
OS:           Linux 4.14.88-72.76.amzn1.x86_64 amd64

$ 
```






```
$ ./gradlew build && java -jar build/libs/gs-spring-boot-0.1.0.jar
Download https://repo.maven.apache.org/maven2/org/springframework/boot/spring-boot-gradle-plugin/2.0.5.RELEASE/spring-boot-gradle-plugin-2.0.5.RELEASE.pom
Download https://repo.maven.apache.org/maven2/org/springframework/boot/spring-boot-tools/2.0.5.RELEASE/spring-boot-tools-2.0.5.RELEASE.pom
Download https://repo.maven.apache.org/maven2/org/springframework/boot/spring-boot-parent/2.0.5.RELEASE/spring-boot-parent-2.0.5.RELEASE.pom
Download https://repo.maven.apache.org/maven2/org/springframework/boot/spring-boot-dependencies/2.0.5.RELEASE/spring-boot-dependencies-2.0.5.RELEASE.pom
Download https://repo.maven.apache.org/maven2/com/fasterxml/jackson/jackson-bom/2.9.6/jackson-bom-2.9.6.pom
Download https://repo.maven.apache.org/maven2/com/fasterxml/jackson/jackson-parent/2.9.1.1/jackson-parent-2.9.1.1.pom
Download https://repo.maven.apache.org/maven2/com/fasterxml/oss-parent/33/oss-parent-33.pom
Download https://repo.maven.apache.org/maven2/io/netty/netty-bom/4.1.29.Final/netty-bom-4.1.29.Final.pom
Download https://repo.maven.apache.org/maven2/org/sonatype/oss/oss-parent/7/oss-parent-7.pom
Download https://repo.maven.apache.org/maven2/io/projectreactor/reactor-bom/Bismuth-SR11/reactor-bom-Bismuth-SR11.pom
Download https://repo.maven.apache.org/maven2/org/apache/logging/log4j/log4j-bom/2.10.0/log4j-bom-2.10.0.pom
Download https://repo.maven.apache.org/maven2/org/apache/logging/logging-parent/1/logging-parent-1.pom
Download https://repo.maven.apache.org/maven2/org/apache/apache/18/apache-18.pom
Download https://repo.maven.apache.org/maven2/org/eclipse/jetty/jetty-bom/9.4.12.v20180830/jetty-bom-9.4.12.v20180830.pom
Download https://repo.maven.apache.org/maven2/org/springframework/spring-framework-bom/5.0.9.RELEASE/spring-framework-bom-5.0.9.RELEASE.pom
Download https://repo.maven.apache.org/maven2/org/springframework/data/spring-data-releasetrain/Kay-SR10/spring-data-releasetrain-Kay-SR10.pom
Download https://repo.maven.apache.org/maven2/org/springframework/data/build/spring-data-build/2.0.10.RELEASE/spring-data-build-2.0.10.RELEASE.pom
Download https://repo.maven.apache.org/maven2/org/springframework/integration/spring-integration-bom/5.0.8.RELEASE/spring-integration-bom-5.0.8.RELEASE.pom
Download https://repo.maven.apache.org/maven2/org/springframework/security/spring-security-bom/5.0.8.RELEASE/spring-security-bom-5.0.8.RELEASE.pom
Download https://repo.maven.apache.org/maven2/org/springframework/session/spring-session-bom/Apple-SR5/spring-session-bom-Apple-SR5.pom
Download https://repo.maven.apache.org/maven2/org/springframework/boot/spring-boot-loader-tools/2.0.5.RELEASE/spring-boot-loader-tools-2.0.5.RELEASE.pom
Download https://repo.maven.apache.org/maven2/org/apache/commons/commons-compress/1.14/commons-compress-1.14.pom
Download https://repo.maven.apache.org/maven2/org/apache/commons/commons-parent/42/commons-parent-42.pom
Download https://repo.maven.apache.org/maven2/io/spring/gradle/dependency-management-plugin/1.0.6.RELEASE/dependency-management-plugin-1.0.6.RELEASE.pom
Download https://repo.maven.apache.org/maven2/org/springframework/spring-core/5.0.9.RELEASE/spring-core-5.0.9.RELEASE.pom
Download https://repo.maven.apache.org/maven2/org/springframework/spring-jcl/5.0.9.RELEASE/spring-jcl-5.0.9.RELEASE.pom
Download https://repo.maven.apache.org/maven2/org/springframework/boot/spring-boot-gradle-plugin/2.0.5.RELEASE/spring-boot-gradle-plugin-2.0.5.RELEASE.jar
Download https://repo.maven.apache.org/maven2/io/spring/gradle/dependency-management-plugin/1.0.6.RELEASE/dependency-management-plugin-1.0.6.RELEASE.jar
Download https://repo.maven.apache.org/maven2/org/apache/commons/commons-compress/1.14/commons-compress-1.14.jar
Download https://repo.maven.apache.org/maven2/org/springframework/spring-core/5.0.9.RELEASE/spring-core-5.0.9.RELEASE.jar
Download https://repo.maven.apache.org/maven2/org/springframework/spring-jcl/5.0.9.RELEASE/spring-jcl-5.0.9.RELEASE.jar
Download https://repo.maven.apache.org/maven2/org/springframework/boot/spring-boot-loader-tools/2.0.5.RELEASE/spring-boot-loader-tools-2.0.5.RELEASE.jar
Download https://repo.maven.apache.org/maven2/org/springframework/boot/spring-boot-starter-web/2.0.5.RELEASE/spring-boot-starter-web-2.0.5.RELEASE.pom
Download https://repo.maven.apache.org/maven2/org/springframework/boot/spring-boot-starters/2.0.5.RELEASE/spring-boot-starters-2.0.5.RELEASE.pom
Download https://repo.maven.apache.org/maven2/org/springframework/boot/spring-boot-starter-actuator/2.0.5.RELEASE/spring-boot-starter-actuator-2.0.5.RELEASE.pom
Download https://repo.maven.apache.org/maven2/org/springframework/boot/spring-boot-starter/2.0.5.RELEASE/spring-boot-starter-2.0.5.RELEASE.pom
Download https://repo.maven.apache.org/maven2/org/springframework/boot/spring-boot-starter-tomcat/2.0.5.RELEASE/spring-boot-starter-tomcat-2.0.5.RELEASE.pom
Download https://repo.maven.apache.org/maven2/org/hibernate/validator/hibernate-validator/6.0.12.Final/hibernate-validator-6.0.12.Final.pom
Download https://repo.maven.apache.org/maven2/org/hibernate/validator/hibernate-validator-parent/6.0.12.Final/hibernate-validator-parent-6.0.12.Final.pom
Download https://repo.maven.apache.org/maven2/org/springframework/spring-web/5.0.9.RELEASE/spring-web-5.0.9.RELEASE.pom
Download https://repo.maven.apache.org/maven2/org/springframework/spring-webmvc/5.0.9.RELEASE/spring-webmvc-5.0.9.RELEASE.pom
Download https://repo.maven.apache.org/maven2/org/springframework/boot/spring-boot-starter-json/2.0.5.RELEASE/spring-boot-starter-json-2.0.5.RELEASE.pom
Download https://repo.maven.apache.org/maven2/org/springframework/boot/spring-boot-actuator-autoconfigure/2.0.5.RELEASE/spring-boot-actuator-autoconfigure-2.0.5.RELEASE.pom
Download https://repo.maven.apache.org/maven2/io/micrometer/micrometer-core/1.0.6/micrometer-core-1.0.6.pom
Download https://repo.maven.apache.org/maven2/org/springframework/boot/spring-boot/2.0.5.RELEASE/spring-boot-2.0.5.RELEASE.pom
Download https://repo.maven.apache.org/maven2/org/springframework/boot/spring-boot-starter-logging/2.0.5.RELEASE/spring-boot-starter-logging-2.0.5.RELEASE.pom
Download https://repo.maven.apache.org/maven2/javax/annotation/javax.annotation-api/1.3.2/javax.annotation-api-1.3.2.pom
Download https://repo.maven.apache.org/maven2/org/yaml/snakeyaml/1.19/snakeyaml-1.19.pom
Download https://repo.maven.apache.org/maven2/org/springframework/boot/spring-boot-autoconfigure/2.0.5.RELEASE/spring-boot-autoconfigure-2.0.5.RELEASE.pom
Download https://repo.maven.apache.org/maven2/com/fasterxml/jackson/core/jackson-databind/2.9.6/jackson-databind-2.9.6.pom
Download https://repo.maven.apache.org/maven2/com/fasterxml/jackson/jackson-base/2.9.6/jackson-base-2.9.6.pom
Download https://repo.maven.apache.org/maven2/com/fasterxml/jackson/datatype/jackson-datatype-jsr310/2.9.6/jackson-datatype-jsr310-2.9.6.pom
Download https://repo.maven.apache.org/maven2/com/fasterxml/jackson/module/jackson-modules-java8/2.9.6/jackson-modules-java8-2.9.6.pom
Download https://repo.maven.apache.org/maven2/com/fasterxml/jackson/module/jackson-module-parameter-names/2.9.6/jackson-module-parameter-names-2.9.6.pom
Download https://repo.maven.apache.org/maven2/com/fasterxml/jackson/datatype/jackson-datatype-jdk8/2.9.6/jackson-datatype-jdk8-2.9.6.pom
Download https://repo.maven.apache.org/maven2/org/apache/tomcat/embed/tomcat-embed-core/8.5.34/tomcat-embed-core-8.5.34.pom
Download https://repo.maven.apache.org/maven2/org/apache/tomcat/embed/tomcat-embed-websocket/8.5.34/tomcat-embed-websocket-8.5.34.pom
Download https://repo.maven.apache.org/maven2/org/apache/tomcat/embed/tomcat-embed-el/8.5.34/tomcat-embed-el-8.5.34.pom
Download https://repo.maven.apache.org/maven2/javax/validation/validation-api/2.0.1.Final/validation-api-2.0.1.Final.pom
Download https://repo.maven.apache.org/maven2/com/fasterxml/classmate/1.3.4/classmate-1.3.4.pom
Download https://repo.maven.apache.org/maven2/org/jboss/logging/jboss-logging/3.3.2.Final/jboss-logging-3.3.2.Final.pom
Download https://repo.maven.apache.org/maven2/org/springframework/spring-beans/5.0.9.RELEASE/spring-beans-5.0.9.RELEASE.pom
Download https://repo.maven.apache.org/maven2/org/springframework/spring-aop/5.0.9.RELEASE/spring-aop-5.0.9.RELEASE.pom
Download https://repo.maven.apache.org/maven2/org/springframework/spring-expression/5.0.9.RELEASE/spring-expression-5.0.9.RELEASE.pom
Download https://repo.maven.apache.org/maven2/org/springframework/spring-context/5.0.9.RELEASE/spring-context-5.0.9.RELEASE.pom
Download https://repo.maven.apache.org/maven2/org/springframework/boot/spring-boot-actuator/2.0.5.RELEASE/spring-boot-actuator-2.0.5.RELEASE.pom
Download https://repo.maven.apache.org/maven2/org/hdrhistogram/HdrHistogram/2.1.10/HdrHistogram-2.1.10.pom
Download https://repo.maven.apache.org/maven2/org/latencyutils/LatencyUtils/2.0.3/LatencyUtils-2.0.3.pom
Download https://repo.maven.apache.org/maven2/ch/qos/logback/logback-classic/1.2.3/logback-classic-1.2.3.pom
Download https://repo.maven.apache.org/maven2/ch/qos/logback/logback-parent/1.2.3/logback-parent-1.2.3.pom
Download https://repo.maven.apache.org/maven2/org/apache/logging/log4j/log4j-to-slf4j/2.10.0/log4j-to-slf4j-2.10.0.pom
Download https://repo.maven.apache.org/maven2/org/apache/logging/log4j/log4j/2.10.0/log4j-2.10.0.pom
Download https://repo.maven.apache.org/maven2/com/fasterxml/jackson/core/jackson-annotations/2.9.0/jackson-annotations-2.9.0.pom
Download https://repo.maven.apache.org/maven2/com/fasterxml/jackson/jackson-parent/2.9.0/jackson-parent-2.9.0.pom
Download https://repo.maven.apache.org/maven2/com/fasterxml/oss-parent/28/oss-parent-28.pom
Download https://repo.maven.apache.org/maven2/com/fasterxml/jackson/core/jackson-core/2.9.6/jackson-core-2.9.6.pom
Download https://repo.maven.apache.org/maven2/ch/qos/logback/logback-core/1.2.3/logback-core-1.2.3.pom
Download https://repo.maven.apache.org/maven2/org/apache/logging/log4j/log4j-api/2.10.0/log4j-api-2.10.0.pom
Download https://repo.maven.apache.org/maven2/org/apache/tomcat/tomcat-annotations-api/8.5.34/tomcat-annotations-api-8.5.34.pom
Download https://repo.maven.apache.org/maven2/org/springframework/boot/spring-boot-starter-web/2.0.5.RELEASE/spring-boot-starter-web-2.0.5.RELEASE.jar
Download https://repo.maven.apache.org/maven2/org/springframework/boot/spring-boot-starter-json/2.0.5.RELEASE/spring-boot-starter-json-2.0.5.RELEASE.jar
Download https://repo.maven.apache.org/maven2/org/springframework/boot/spring-boot-starter/2.0.5.RELEASE/spring-boot-starter-2.0.5.RELEASE.jar
Download https://repo.maven.apache.org/maven2/org/springframework/boot/spring-boot-starter-tomcat/2.0.5.RELEASE/spring-boot-starter-tomcat-2.0.5.RELEASE.jar
Download https://repo.maven.apache.org/maven2/org/hibernate/validator/hibernate-validator/6.0.12.Final/hibernate-validator-6.0.12.Final.jar
Download https://repo.maven.apache.org/maven2/org/springframework/spring-webmvc/5.0.9.RELEASE/spring-webmvc-5.0.9.RELEASE.jar
Download https://repo.maven.apache.org/maven2/org/springframework/spring-web/5.0.9.RELEASE/spring-web-5.0.9.RELEASE.jar
Download https://repo.maven.apache.org/maven2/org/springframework/boot/spring-boot-actuator-autoconfigure/2.0.5.RELEASE/spring-boot-actuator-autoconfigure-2.0.5.RELEASE.jar
Download https://repo.maven.apache.org/maven2/io/micrometer/micrometer-core/1.0.6/micrometer-core-1.0.6.jar
Download https://repo.maven.apache.org/maven2/org/springframework/boot/spring-boot-autoconfigure/2.0.5.RELEASE/spring-boot-autoconfigure-2.0.5.RELEASE.jar
Download https://repo.maven.apache.org/maven2/org/springframework/boot/spring-boot-actuator/2.0.5.RELEASE/spring-boot-actuator-2.0.5.RELEASE.jar
Download https://repo.maven.apache.org/maven2/org/springframework/boot/spring-boot/2.0.5.RELEASE/spring-boot-2.0.5.RELEASE.jar
Download https://repo.maven.apache.org/maven2/org/springframework/boot/spring-boot-starter-logging/2.0.5.RELEASE/spring-boot-starter-logging-2.0.5.RELEASE.jar
Download https://repo.maven.apache.org/maven2/javax/annotation/javax.annotation-api/1.3.2/javax.annotation-api-1.3.2.jar
Download https://repo.maven.apache.org/maven2/org/springframework/spring-context/5.0.9.RELEASE/spring-context-5.0.9.RELEASE.jar
Download https://repo.maven.apache.org/maven2/org/springframework/spring-aop/5.0.9.RELEASE/spring-aop-5.0.9.RELEASE.jar
Download https://repo.maven.apache.org/maven2/org/springframework/spring-beans/5.0.9.RELEASE/spring-beans-5.0.9.RELEASE.jar
Download https://repo.maven.apache.org/maven2/org/springframework/spring-expression/5.0.9.RELEASE/spring-expression-5.0.9.RELEASE.jar
Download https://repo.maven.apache.org/maven2/org/yaml/snakeyaml/1.19/snakeyaml-1.19.jar
Download https://repo.maven.apache.org/maven2/com/fasterxml/jackson/datatype/jackson-datatype-jdk8/2.9.6/jackson-datatype-jdk8-2.9.6.jar
Download https://repo.maven.apache.org/maven2/com/fasterxml/jackson/datatype/jackson-datatype-jsr310/2.9.6/jackson-datatype-jsr310-2.9.6.jar
Download https://repo.maven.apache.org/maven2/com/fasterxml/jackson/module/jackson-module-parameter-names/2.9.6/jackson-module-parameter-names-2.9.6.jar
Download https://repo.maven.apache.org/maven2/com/fasterxml/jackson/core/jackson-databind/2.9.6/jackson-databind-2.9.6.jar
Download https://repo.maven.apache.org/maven2/org/apache/tomcat/embed/tomcat-embed-websocket/8.5.34/tomcat-embed-websocket-8.5.34.jar
Download https://repo.maven.apache.org/maven2/org/apache/tomcat/embed/tomcat-embed-core/8.5.34/tomcat-embed-core-8.5.34.jar
Download https://repo.maven.apache.org/maven2/org/apache/tomcat/embed/tomcat-embed-el/8.5.34/tomcat-embed-el-8.5.34.jar
Download https://repo.maven.apache.org/maven2/javax/validation/validation-api/2.0.1.Final/validation-api-2.0.1.Final.jar
Download https://repo.maven.apache.org/maven2/org/jboss/logging/jboss-logging/3.3.2.Final/jboss-logging-3.3.2.Final.jar
Download https://repo.maven.apache.org/maven2/com/fasterxml/classmate/1.3.4/classmate-1.3.4.jar
Download https://repo.maven.apache.org/maven2/org/hdrhistogram/HdrHistogram/2.1.10/HdrHistogram-2.1.10.jar
Download https://repo.maven.apache.org/maven2/org/latencyutils/LatencyUtils/2.0.3/LatencyUtils-2.0.3.jar
Download https://repo.maven.apache.org/maven2/ch/qos/logback/logback-classic/1.2.3/logback-classic-1.2.3.jar
Download https://repo.maven.apache.org/maven2/org/apache/logging/log4j/log4j-to-slf4j/2.10.0/log4j-to-slf4j-2.10.0.jar
Download https://repo.maven.apache.org/maven2/com/fasterxml/jackson/core/jackson-annotations/2.9.0/jackson-annotations-2.9.0.jar
Download https://repo.maven.apache.org/maven2/com/fasterxml/jackson/core/jackson-core/2.9.6/jackson-core-2.9.6.jar
Download https://repo.maven.apache.org/maven2/ch/qos/logback/logback-core/1.2.3/logback-core-1.2.3.jar
Download https://repo.maven.apache.org/maven2/org/apache/logging/log4j/log4j-api/2.10.0/log4j-api-2.10.0.jar
Download https://repo.maven.apache.org/maven2/org/springframework/boot/spring-boot-starter-actuator/2.0.5.RELEASE/spring-boot-starter-actuator-2.0.5.RELEASE.jar
Download https://repo.maven.apache.org/maven2/org/springframework/boot/spring-boot-starter-test/2.0.5.RELEASE/spring-boot-starter-test-2.0.5.RELEASE.pom
Download https://repo.maven.apache.org/maven2/org/springframework/boot/spring-boot-test/2.0.5.RELEASE/spring-boot-test-2.0.5.RELEASE.pom
Download https://repo.maven.apache.org/maven2/com/jayway/jsonpath/json-path/2.4.0/json-path-2.4.0.pom
Download https://repo.maven.apache.org/maven2/junit/junit/4.12/junit-4.12.pom
Download https://repo.maven.apache.org/maven2/org/assertj/assertj-core/3.9.1/assertj-core-3.9.1.pom
Download https://repo.maven.apache.org/maven2/org/assertj/assertj-parent-pom/2.1.9/assertj-parent-pom-2.1.9.pom
Download https://repo.maven.apache.org/maven2/org/mockito/mockito-core/2.15.0/mockito-core-2.15.0.pom
Download https://repo.maven.apache.org/maven2/org/hamcrest/hamcrest-core/1.3/hamcrest-core-1.3.pom
Download https://repo.maven.apache.org/maven2/org/hamcrest/hamcrest-parent/1.3/hamcrest-parent-1.3.pom
Download https://repo.maven.apache.org/maven2/org/hamcrest/hamcrest-library/1.3/hamcrest-library-1.3.pom
Download https://repo.maven.apache.org/maven2/org/skyscreamer/jsonassert/1.5.0/jsonassert-1.5.0.pom
Download https://repo.maven.apache.org/maven2/org/springframework/spring-test/5.0.9.RELEASE/spring-test-5.0.9.RELEASE.pom
Download https://repo.maven.apache.org/maven2/org/xmlunit/xmlunit-core/2.5.1/xmlunit-core-2.5.1.pom
Download https://repo.maven.apache.org/maven2/org/xmlunit/xmlunit-parent/2.5.1/xmlunit-parent-2.5.1.pom
Download https://repo.maven.apache.org/maven2/org/springframework/boot/spring-boot-test-autoconfigure/2.0.5.RELEASE/spring-boot-test-autoconfigure-2.0.5.RELEASE.pom
Download https://repo.maven.apache.org/maven2/net/minidev/json-smart/2.3/json-smart-2.3.pom
Download https://repo.maven.apache.org/maven2/net/minidev/minidev-parent/2.3/minidev-parent-2.3.pom
Download https://repo.maven.apache.org/maven2/net/bytebuddy/byte-buddy/1.7.11/byte-buddy-1.7.11.pom
Download https://repo.maven.apache.org/maven2/net/bytebuddy/byte-buddy-parent/1.7.11/byte-buddy-parent-1.7.11.pom
Download https://repo.maven.apache.org/maven2/org/objenesis/objenesis/2.6/objenesis-2.6.pom
Download https://repo.maven.apache.org/maven2/org/objenesis/objenesis-parent/2.6/objenesis-parent-2.6.pom
Download https://repo.maven.apache.org/maven2/net/bytebuddy/byte-buddy-agent/1.7.11/byte-buddy-agent-1.7.11.pom
Download https://repo.maven.apache.org/maven2/com/vaadin/external/google/android-json/0.0.20131108.vaadin1/android-json-0.0.20131108.vaadin1.pom
Download https://repo.maven.apache.org/maven2/net/minidev/accessors-smart/1.2/accessors-smart-1.2.pom
Download https://repo.maven.apache.org/maven2/org/ow2/asm/asm/5.0.4/asm-5.0.4.pom
Download https://repo.maven.apache.org/maven2/org/ow2/asm/asm-parent/5.0.4/asm-parent-5.0.4.pom
Download https://repo.maven.apache.org/maven2/org/springframework/boot/spring-boot-starter-test/2.0.5.RELEASE/spring-boot-starter-test-2.0.5.RELEASE.jar
Download https://repo.maven.apache.org/maven2/org/springframework/boot/spring-boot-test/2.0.5.RELEASE/spring-boot-test-2.0.5.RELEASE.jar
Download https://repo.maven.apache.org/maven2/com/jayway/jsonpath/json-path/2.4.0/json-path-2.4.0.jar
Download https://repo.maven.apache.org/maven2/junit/junit/4.12/junit-4.12.jar
Download https://repo.maven.apache.org/maven2/org/assertj/assertj-core/3.9.1/assertj-core-3.9.1.jar
Download https://repo.maven.apache.org/maven2/org/mockito/mockito-core/2.15.0/mockito-core-2.15.0.jar
Download https://repo.maven.apache.org/maven2/org/hamcrest/hamcrest-library/1.3/hamcrest-library-1.3.jar
Download https://repo.maven.apache.org/maven2/org/hamcrest/hamcrest-core/1.3/hamcrest-core-1.3.jar
Download https://repo.maven.apache.org/maven2/org/skyscreamer/jsonassert/1.5.0/jsonassert-1.5.0.jar
Download https://repo.maven.apache.org/maven2/org/springframework/spring-test/5.0.9.RELEASE/spring-test-5.0.9.RELEASE.jar
Download https://repo.maven.apache.org/maven2/org/xmlunit/xmlunit-core/2.5.1/xmlunit-core-2.5.1.jar
Download https://repo.maven.apache.org/maven2/net/minidev/json-smart/2.3/json-smart-2.3.jar
Download https://repo.maven.apache.org/maven2/net/bytebuddy/byte-buddy/1.7.11/byte-buddy-1.7.11.jar
Download https://repo.maven.apache.org/maven2/net/bytebuddy/byte-buddy-agent/1.7.11/byte-buddy-agent-1.7.11.jar
Download https://repo.maven.apache.org/maven2/org/objenesis/objenesis/2.6/objenesis-2.6.jar
Download https://repo.maven.apache.org/maven2/com/vaadin/external/google/android-json/0.0.20131108.vaadin1/android-json-0.0.20131108.vaadin1.jar
Download https://repo.maven.apache.org/maven2/net/minidev/accessors-smart/1.2/accessors-smart-1.2.jar
Download https://repo.maven.apache.org/maven2/org/ow2/asm/asm/5.0.4/asm-5.0.4.jar
Download https://repo.maven.apache.org/maven2/org/springframework/boot/spring-boot-test-autoconfigure/2.0.5.RELEASE/spring-boot-test-autoconfigure-2.0.5.RELEASE.jar

> Task :test 
2019-01-25 03:14:58.142  INFO 10709 --- [      Thread-13] o.s.w.c.s.GenericWebApplicationContext   : Closing org.springframework.web.context.support.GenericWebApplicationContext@77e24dfb: startup date [Fri Jan 25 03:14:55 UTC 2019]; root of context hierarchy
2019-01-25 03:14:58.150  INFO 10709 --- [       Thread-8] ConfigServletWebServerApplicationContext : Closing org.springframework.boot.web.servlet.context.AnnotationConfigServletWebServerApplicationContext@3ae93e8e: startup date [Fri Jan 25 03:14:48 UTC 2019]; root of context hierarchy


BUILD SUCCESSFUL in 40s
4 actionable tasks: 4 executed

  .   ____          _            __ _ _
 /\\ / ___'_ __ _ _(_)_ __  __ _ \ \ \ \
( ( )\___ | '_ | '_| | '_ \/ _` | \ \ \ \
 \\/  ___)| |_)| | | | | || (_| |  ) ) ) )
  '  |____| .__|_| |_|_| |_\__, | / / / /
 =========|_|==============|___/=/_/_/_/
 :: Spring Boot ::        (v2.0.5.RELEASE)

2019-01-25 03:15:01.426  INFO 10771 --- [           main] hello.Application                        : Starting Application on ip-172-31-21-135 with PID 10771 (/home/ec2-user/environment/gs-spring-boot/complete/build/libs/gs-spring-boot-0.1.0.jar started by ec2-user in /home/ec2-user/environment/gs-spring-boot/complete)
2019-01-25 03:15:01.440  INFO 10771 --- [           main] hello.Application                        : No active profile set, falling back to default profiles: default
2019-01-25 03:15:01.653  INFO 10771 --- [           main] ConfigServletWebServerApplicationContext : Refreshing org.springframework.boot.web.servlet.context.AnnotationConfigServletWebServerApplicationContext@47089e5f: startup date [Fri Jan 25 03:15:01 UTC 2019]; root of context hierarchy
2019-01-25 03:15:05.746  INFO 10771 --- [           main] o.s.b.w.embedded.tomcat.TomcatWebServer  : Tomcat initialized with port(s): 8080 (http)
2019-01-25 03:15:05.827  INFO 10771 --- [           main] o.apache.catalina.core.StandardService   : Starting service [Tomcat]
2019-01-25 03:15:05.828  INFO 10771 --- [           main] org.apache.catalina.core.StandardEngine  : Starting Servlet Engine: Apache Tomcat/8.5.34
2019-01-25 03:15:05.862  INFO 10771 --- [ost-startStop-1] o.a.catalina.core.AprLifecycleListener   : The APR based Apache Tomcat Native library which allows optimal performance in production environments was not found on the java.library.path: [/usr/java/packages/lib/amd64:/usr/lib64:/lib64:/lib:/usr/lib]
2019-01-25 03:15:06.054  INFO 10771 --- [ost-startStop-1] o.a.c.c.C.[Tomcat].[localhost].[/]       : Initializing Spring embedded WebApplicationContext
2019-01-25 03:15:06.054  INFO 10771 --- [ost-startStop-1] o.s.web.context.ContextLoader            : Root WebApplicationContext: initialization completed in 4408 ms
2019-01-25 03:15:07.387  INFO 10771 --- [ost-startStop-1] o.s.b.w.servlet.FilterRegistrationBean   : Mapping filter: 'characterEncodingFilter' to: [/*]
2019-01-25 03:15:07.390  INFO 10771 --- [ost-startStop-1] o.s.b.w.servlet.FilterRegistrationBean   : Mapping filter: 'webMvcMetricsFilter' to: [/*]
2019-01-25 03:15:07.390  INFO 10771 --- [ost-startStop-1] o.s.b.w.servlet.FilterRegistrationBean   : Mapping filter: 'hiddenHttpMethodFilter' to: [/*]
2019-01-25 03:15:07.391  INFO 10771 --- [ost-startStop-1] o.s.b.w.servlet.FilterRegistrationBean   : Mapping filter: 'httpPutFormContentFilter' to: [/*]
2019-01-25 03:15:07.391  INFO 10771 --- [ost-startStop-1] o.s.b.w.servlet.FilterRegistrationBean   : Mapping filter: 'requestContextFilter' to: [/*]
2019-01-25 03:15:07.391  INFO 10771 --- [ost-startStop-1] o.s.b.w.servlet.FilterRegistrationBean   : Mapping filter: 'httpTraceFilter' to: [/*]
2019-01-25 03:15:07.392  INFO 10771 --- [ost-startStop-1] o.s.b.w.servlet.ServletRegistrationBean  : Servlet dispatcherServlet mapped to [/]
2019-01-25 03:15:07.660  INFO 10771 --- [           main] o.s.w.s.handler.SimpleUrlHandlerMapping  : Mapped URL path [/**/favicon.ico] onto handler of type [class org.springframework.web.servlet.resource.ResourceHttpRequestHandler]
2019-01-25 03:15:08.039  INFO 10771 --- [           main] s.w.s.m.m.a.RequestMappingHandlerAdapter : Looking for @ControllerAdvice: org.springframework.boot.web.servlet.context.AnnotationConfigServletWebServerApplicationContext@47089e5f: startup date [Fri Jan 25 03:15:01 UTC 2019]; root of context hierarchy
2019-01-25 03:15:08.208  INFO 10771 --- [           main] s.w.s.m.m.a.RequestMappingHandlerMapping : Mapped "{[/]}" onto public java.lang.String hello.HelloController.index()
2019-01-25 03:15:08.222  INFO 10771 --- [           main] s.w.s.m.m.a.RequestMappingHandlerMapping : Mapped "{[/error],produces=[text/html]}" onto public org.springframework.web.servlet.ModelAndView org.springframework.boot.autoconfigure.web.servlet.error.BasicErrorController.errorHtml(javax.servlet.http.HttpServletRequest,javax.servlet.http.HttpServletResponse)
2019-01-25 03:15:08.230  INFO 10771 --- [           main] s.w.s.m.m.a.RequestMappingHandlerMapping : Mapped "{[/error]}" onto public org.springframework.http.ResponseEntity<java.util.Map<java.lang.String, java.lang.Object>> org.springframework.boot.autoconfigure.web.servlet.error.BasicErrorController.error(javax.servlet.http.HttpServletRequest)
2019-01-25 03:15:08.300  INFO 10771 --- [           main] o.s.w.s.handler.SimpleUrlHandlerMapping  : Mapped URL path [/webjars/**] onto handler of type [class org.springframework.web.servlet.resource.ResourceHttpRequestHandler]
2019-01-25 03:15:08.301  INFO 10771 --- [           main] o.s.w.s.handler.SimpleUrlHandlerMapping  : Mapped URL path [/**] onto handler of type [class org.springframework.web.servlet.resource.ResourceHttpRequestHandler]
2019-01-25 03:15:08.913  INFO 10771 --- [           main] o.s.b.a.e.web.EndpointLinksResolver      : Exposing 2 endpoint(s) beneath base path '/actuator'
2019-01-25 03:15:08.933  INFO 10771 --- [           main] s.b.a.e.w.s.WebMvcEndpointHandlerMapping : Mapped "{[/actuator/health],methods=[GET],produces=[application/vnd.spring-boot.actuator.v2+json || application/json]}" onto public java.lang.Object org.springframework.boot.actuate.endpoint.web.servlet.AbstractWebMvcEndpointHandlerMapping$OperationHandler.handle(javax.servlet.http.HttpServletRequest,java.util.Map<java.lang.String, java.lang.String>)
2019-01-25 03:15:08.943  INFO 10771 --- [           main] s.b.a.e.w.s.WebMvcEndpointHandlerMapping : Mapped "{[/actuator/info],methods=[GET],produces=[application/vnd.spring-boot.actuator.v2+json || application/json]}" onto public java.lang.Object org.springframework.boot.actuate.endpoint.web.servlet.AbstractWebMvcEndpointHandlerMapping$OperationHandler.handle(javax.servlet.http.HttpServletRequest,java.util.Map<java.lang.String, java.lang.String>)
2019-01-25 03:15:08.944  INFO 10771 --- [           main] s.b.a.e.w.s.WebMvcEndpointHandlerMapping : Mapped "{[/actuator],methods=[GET],produces=[application/vnd.spring-boot.actuator.v2+json || application/json]}" onto protected java.util.Map<java.lang.String, java.util.Map<java.lang.String, org.springframework.boot.actuate.endpoint.web.Link>> org.springframework.boot.actuate.endpoint.web.servlet.WebMvcEndpointHandlerMapping.links(javax.servlet.http.HttpServletRequest,javax.servlet.http.HttpServletResponse)
2019-01-25 03:15:09.060  INFO 10771 --- [           main] o.s.j.e.a.AnnotationMBeanExporter        : Registering beans for JMX exposure on startup
2019-01-25 03:15:09.170  INFO 10771 --- [           main] o.s.b.w.embedded.tomcat.TomcatWebServer  : Tomcat started on port(s): 8080 (http) with context path ''
2019-01-25 03:15:09.180  INFO 10771 --- [           main] hello.Application                        : Started Application in 8.946 seconds (JVM running for 10.331)
Let's inspect the beans provided by Spring Boot:
application
auditEventRepository
auditEventsEndpoint
auditListener
basicErrorController
beanNameHandlerMapping
beanNameViewResolver
beansEndpoint
characterEncodingFilter
classLoaderMetrics
commandLineRunner
conditionsReportEndpoint
configurationPropertiesReportEndpoint
contextCapturingServletTomcatCustomizer
controllerEndpointDiscoverer
controllerEndpointHandlerMapping
controllerExposeExcludePropertyEndpointFilter
conventionErrorViewResolver
createHealthStatusHttpMapper
defaultServletHandlerMapping
defaultValidator
defaultViewResolver
diskSpaceHealthIndicator
diskSpaceHealthIndicatorProperties
dispatcherServlet
dispatcherServletMappingDescriptionProvider
dispatcherServletRegistration
dumpEndpoint
endpointCachingOperationInvokerAdvisor
endpointMediaTypes
endpointOperationParameterMapper
envInfoContributor
environmentEndpoint
environmentEndpointWebExtension
error
errorAttributes
errorPageCustomizer
errorPageRegistrarBeanPostProcessor
faviconHandlerMapping
faviconRequestHandler
fileDescriptorMetrics
filterMappingDescriptionProvider
handlerExceptionResolver
healthAggregator
healthEndpoint
healthEndpointWebExtension
healthWebEndpointResponseMapper
heapDumpWebEndpoint
helloController
hiddenHttpMethodFilter
httpExchangeTracer
httpPutFormContentFilter
httpRequestHandlerAdapter
httpTraceEndpoint
httpTraceFilter
infoEndpoint
jacksonCodecCustomizer
jacksonObjectMapper
jacksonObjectMapperBuilder
jmxAnnotationEndpointDiscoverer
jmxIncludeExcludePropertyEndpointFilter
jmxMBeanExporter
jsonComponentModule
jvmGcMetrics
jvmMemoryMetrics
jvmThreadMetrics
localeCharsetMappingsCustomizer
logbackMetrics
loggersEndpoint
management.endpoint.configprops-org.springframework.boot.actuate.autoconfigure.context.properties.ConfigurationPropertiesReportEndpointProperties
management.endpoint.env-org.springframework.boot.actuate.autoconfigure.env.EnvironmentEndpointProperties
management.endpoint.health-org.springframework.boot.actuate.autoconfigure.health.HealthEndpointProperties
management.endpoint.logfile-org.springframework.boot.actuate.autoconfigure.logging.LogFileWebEndpointProperties
management.endpoints.jmx-org.springframework.boot.actuate.autoconfigure.endpoint.jmx.JmxEndpointProperties
management.endpoints.web-org.springframework.boot.actuate.autoconfigure.endpoint.web.WebEndpointProperties
management.endpoints.web.cors-org.springframework.boot.actuate.autoconfigure.endpoint.web.CorsEndpointProperties
management.health.status-org.springframework.boot.actuate.autoconfigure.health.HealthIndicatorProperties
management.info-org.springframework.boot.actuate.autoconfigure.info.InfoContributorProperties
management.metrics-org.springframework.boot.actuate.autoconfigure.metrics.MetricsProperties
management.metrics.export.simple-org.springframework.boot.actuate.autoconfigure.metrics.export.simple.SimpleProperties
management.server-org.springframework.boot.actuate.autoconfigure.web.server.ManagementServerProperties
management.trace.http-org.springframework.boot.actuate.autoconfigure.trace.http.HttpTraceProperties
managementServletContext
mappingJackson2HttpMessageConverter
mappingsEndpoint
mbeanExporter
mbeanServer
messageConverters
meterRegistryPostProcessor
methodValidationPostProcessor
metricsEndpoint
metricsHttpServerUriTagFilter
metricsRestTemplateCustomizer
metricsWebClientUriTagFilter
micrometerClock
multipartConfigElement
multipartResolver
mvcContentNegotiationManager
mvcConversionService
mvcHandlerMappingIntrospector
mvcPathMatcher
mvcResourceUrlProvider
mvcUriComponentsContributor
mvcUrlPathHelper
mvcValidator
mvcViewResolver
objectNamingStrategy
org.springframework.boot.actuate.autoconfigure.audit.AuditAutoConfiguration
org.springframework.boot.actuate.autoconfigure.audit.AuditAutoConfiguration$AuditEventRepositoryConfiguration
org.springframework.boot.actuate.autoconfigure.audit.AuditEventsEndpointAutoConfiguration
org.springframework.boot.actuate.autoconfigure.beans.BeansEndpointAutoConfiguration
org.springframework.boot.actuate.autoconfigure.condition.ConditionsReportEndpointAutoConfiguration
org.springframework.boot.actuate.autoconfigure.context.ShutdownEndpointAutoConfiguration
org.springframework.boot.actuate.autoconfigure.context.properties.ConfigurationPropertiesReportEndpointAutoConfiguration
org.springframework.boot.actuate.autoconfigure.elasticsearch.ElasticsearchHealthIndicatorAutoConfiguration
org.springframework.boot.actuate.autoconfigure.endpoint.EndpointAutoConfiguration
org.springframework.boot.actuate.autoconfigure.endpoint.jmx.JmxEndpointAutoConfiguration
org.springframework.boot.actuate.autoconfigure.endpoint.web.ServletEndpointManagementContextConfiguration
org.springframework.boot.actuate.autoconfigure.endpoint.web.ServletEndpointManagementContextConfiguration$WebMvcServletEndpointManagementContextConfiguration
org.springframework.boot.actuate.autoconfigure.endpoint.web.WebEndpointAutoConfiguration
org.springframework.boot.actuate.autoconfigure.endpoint.web.WebEndpointAutoConfiguration$WebEndpointServletConfiguration
org.springframework.boot.actuate.autoconfigure.endpoint.web.servlet.WebMvcEndpointManagementContextConfiguration
org.springframework.boot.actuate.autoconfigure.env.EnvironmentEndpointAutoConfiguration
org.springframework.boot.actuate.autoconfigure.health.HealthEndpointAutoConfiguration
org.springframework.boot.actuate.autoconfigure.health.HealthEndpointConfiguration
org.springframework.boot.actuate.autoconfigure.health.HealthEndpointWebExtensionConfiguration
org.springframework.boot.actuate.autoconfigure.health.HealthEndpointWebExtensionConfiguration$ServletWebHealthConfiguration
org.springframework.boot.actuate.autoconfigure.health.HealthIndicatorAutoConfiguration
org.springframework.boot.actuate.autoconfigure.info.InfoContributorAutoConfiguration
org.springframework.boot.actuate.autoconfigure.info.InfoEndpointAutoConfiguration
org.springframework.boot.actuate.autoconfigure.logging.LogFileWebEndpointAutoConfiguration
org.springframework.boot.actuate.autoconfigure.logging.LoggersEndpointAutoConfiguration
org.springframework.boot.actuate.autoconfigure.management.HeapDumpWebEndpointAutoConfiguration
org.springframework.boot.actuate.autoconfigure.management.ThreadDumpEndpointAutoConfiguration
org.springframework.boot.actuate.autoconfigure.metrics.CompositeMeterRegistryAutoConfiguration
org.springframework.boot.actuate.autoconfigure.metrics.MetricsAutoConfiguration
org.springframework.boot.actuate.autoconfigure.metrics.MetricsAutoConfiguration$JvmMeterBindersConfiguration
org.springframework.boot.actuate.autoconfigure.metrics.MetricsAutoConfiguration$MeterBindersConfiguration
org.springframework.boot.actuate.autoconfigure.metrics.MetricsEndpointAutoConfiguration
org.springframework.boot.actuate.autoconfigure.metrics.export.simple.SimpleMetricsExportAutoConfiguration
org.springframework.boot.actuate.autoconfigure.metrics.web.client.RestTemplateMetricsAutoConfiguration
org.springframework.boot.actuate.autoconfigure.metrics.web.servlet.WebMvcMetricsAutoConfiguration
org.springframework.boot.actuate.autoconfigure.metrics.web.tomcat.TomcatMetricsAutoConfiguration
org.springframework.boot.actuate.autoconfigure.mongo.MongoHealthIndicatorAutoConfiguration
org.springframework.boot.actuate.autoconfigure.redis.RedisHealthIndicatorAutoConfiguration
org.springframework.boot.actuate.autoconfigure.scheduling.ScheduledTasksEndpointAutoConfiguration
org.springframework.boot.actuate.autoconfigure.system.DiskSpaceHealthIndicatorAutoConfiguration
org.springframework.boot.actuate.autoconfigure.trace.http.HttpTraceAutoConfiguration
org.springframework.boot.actuate.autoconfigure.trace.http.HttpTraceAutoConfiguration$ServletTraceFilterConfiguration
org.springframework.boot.actuate.autoconfigure.trace.http.HttpTraceEndpointAutoConfiguration
org.springframework.boot.actuate.autoconfigure.web.mappings.MappingsEndpointAutoConfiguration
org.springframework.boot.actuate.autoconfigure.web.mappings.MappingsEndpointAutoConfiguration$ServletWebConfiguration
org.springframework.boot.actuate.autoconfigure.web.mappings.MappingsEndpointAutoConfiguration$ServletWebConfiguration$SpringMvcConfiguration
org.springframework.boot.actuate.autoconfigure.web.server.ManagementContextAutoConfiguration
org.springframework.boot.actuate.autoconfigure.web.server.ManagementContextAutoConfiguration$SameManagementContextConfiguration
org.springframework.boot.actuate.autoconfigure.web.server.ManagementContextAutoConfiguration$SameManagementContextConfiguration$EnableSameManagementContextConfiguration
org.springframework.boot.actuate.autoconfigure.web.servlet.ServletManagementContextAutoConfiguration
org.springframework.boot.autoconfigure.AutoConfigurationPackages
org.springframework.boot.autoconfigure.condition.BeanTypeRegistry
org.springframework.boot.autoconfigure.context.ConfigurationPropertiesAutoConfiguration
org.springframework.boot.autoconfigure.context.PropertyPlaceholderAutoConfiguration
org.springframework.boot.autoconfigure.http.HttpMessageConvertersAutoConfiguration
org.springframework.boot.autoconfigure.http.HttpMessageConvertersAutoConfiguration$StringHttpMessageConverterConfiguration
org.springframework.boot.autoconfigure.http.JacksonHttpMessageConvertersConfiguration
org.springframework.boot.autoconfigure.http.JacksonHttpMessageConvertersConfiguration$MappingJackson2HttpMessageConverterConfiguration
org.springframework.boot.autoconfigure.http.codec.CodecsAutoConfiguration
org.springframework.boot.autoconfigure.http.codec.CodecsAutoConfiguration$JacksonCodecConfiguration
org.springframework.boot.autoconfigure.info.ProjectInfoAutoConfiguration
org.springframework.boot.autoconfigure.internalCachingMetadataReaderFactory
org.springframework.boot.autoconfigure.jackson.JacksonAutoConfiguration
org.springframework.boot.autoconfigure.jackson.JacksonAutoConfiguration$Jackson2ObjectMapperBuilderCustomizerConfiguration
org.springframework.boot.autoconfigure.jackson.JacksonAutoConfiguration$JacksonObjectMapperBuilderConfiguration
org.springframework.boot.autoconfigure.jackson.JacksonAutoConfiguration$JacksonObjectMapperConfiguration
org.springframework.boot.autoconfigure.jackson.JacksonAutoConfiguration$ParameterNamesModuleConfiguration
org.springframework.boot.autoconfigure.jmx.JmxAutoConfiguration
org.springframework.boot.autoconfigure.validation.ValidationAutoConfiguration
org.springframework.boot.autoconfigure.web.client.RestTemplateAutoConfiguration
org.springframework.boot.autoconfigure.web.embedded.EmbeddedWebServerFactoryCustomizerAutoConfiguration
org.springframework.boot.autoconfigure.web.embedded.EmbeddedWebServerFactoryCustomizerAutoConfiguration$TomcatWebServerFactoryCustomizerConfiguration
org.springframework.boot.autoconfigure.web.servlet.DispatcherServletAutoConfiguration
org.springframework.boot.autoconfigure.web.servlet.DispatcherServletAutoConfiguration$DispatcherServletConfiguration
org.springframework.boot.autoconfigure.web.servlet.DispatcherServletAutoConfiguration$DispatcherServletRegistrationConfiguration
org.springframework.boot.autoconfigure.web.servlet.HttpEncodingAutoConfiguration
org.springframework.boot.autoconfigure.web.servlet.MultipartAutoConfiguration
org.springframework.boot.autoconfigure.web.servlet.ServletWebServerFactoryAutoConfiguration
org.springframework.boot.autoconfigure.web.servlet.ServletWebServerFactoryConfiguration$EmbeddedTomcat
org.springframework.boot.autoconfigure.web.servlet.WebMvcAutoConfiguration
org.springframework.boot.autoconfigure.web.servlet.WebMvcAutoConfiguration$EnableWebMvcConfiguration
org.springframework.boot.autoconfigure.web.servlet.WebMvcAutoConfiguration$WebMvcAutoConfigurationAdapter
org.springframework.boot.autoconfigure.web.servlet.WebMvcAutoConfiguration$WebMvcAutoConfigurationAdapter$FaviconConfiguration
org.springframework.boot.autoconfigure.web.servlet.error.ErrorMvcAutoConfiguration
org.springframework.boot.autoconfigure.web.servlet.error.ErrorMvcAutoConfiguration$DefaultErrorViewResolverConfiguration
org.springframework.boot.autoconfigure.web.servlet.error.ErrorMvcAutoConfiguration$WhitelabelErrorViewConfiguration
org.springframework.boot.autoconfigure.websocket.servlet.WebSocketServletAutoConfiguration
org.springframework.boot.autoconfigure.websocket.servlet.WebSocketServletAutoConfiguration$TomcatWebSocketConfiguration
org.springframework.boot.context.properties.ConfigurationBeanFactoryMetadata
org.springframework.boot.context.properties.ConfigurationPropertiesBindingPostProcessor
org.springframework.context.annotation.internalAutowiredAnnotationProcessor
org.springframework.context.annotation.internalCommonAnnotationProcessor
org.springframework.context.annotation.internalConfigurationAnnotationProcessor
org.springframework.context.annotation.internalRequiredAnnotationProcessor
org.springframework.context.event.internalEventListenerFactory
org.springframework.context.event.internalEventListenerProcessor
parameterNamesModule
pathMappedEndpoints
preserveErrorControllerTargetClassPostProcessor
processorMetrics
propertiesMeterFilter
propertySourcesPlaceholderConfigurer
requestContextFilter
requestMappingHandlerAdapter
requestMappingHandlerMapping
resourceHandlerMapping
restTemplateBuilder
restTemplateTagConfigurer
scheduledTasksEndpoint
server-org.springframework.boot.autoconfigure.web.ServerProperties
servletEndpointDiscoverer
servletEndpointRegistrar
servletExposeExcludePropertyEndpointFilter
servletMappingDescriptionProvider
servletWebChildContextFactory
servletWebServerFactoryCustomizer
simpleConfig
simpleControllerHandlerAdapter
simpleMeterRegistry
spring.http.encoding-org.springframework.boot.autoconfigure.http.HttpEncodingProperties
spring.info-org.springframework.boot.autoconfigure.info.ProjectInfoProperties
spring.jackson-org.springframework.boot.autoconfigure.jackson.JacksonProperties
spring.mvc-org.springframework.boot.autoconfigure.web.servlet.WebMvcProperties
spring.resources-org.springframework.boot.autoconfigure.web.ResourceProperties
spring.servlet.multipart-org.springframework.boot.autoconfigure.web.servlet.MultipartProperties
standardJacksonObjectMapperBuilderCustomizer
stringHttpMessageConverter
tomcatMetrics
tomcatServletWebServerFactory
tomcatServletWebServerFactoryCustomizer
tomcatWebServerFactoryCustomizer
traceRepository
uptimeMetrics
viewControllerHandlerMapping
viewResolver
webEndpointDiscoverer
webEndpointPathMapper
webEndpointServletHandlerMapping
webExposeExcludePropertyEndpointFilter
webMvcMetricsFilter
webMvcTagsProvider
webServerFactoryCustomizerBeanPostProcessor
websocketContainerCustomizer
welcomePageHandlerMapping
2019-01-25 03:15:57.173  INFO 10771 --- [nio-8080-exec-1] o.a.c.c.C.[Tomcat].[localhost].[/]       : Initializing Spring FrameworkServlet 'dispatcherServlet'
2019-01-25 03:15:57.179  INFO 10771 --- [nio-8080-exec-1] o.s.web.servlet.DispatcherServlet        : FrameworkServlet 'dispatcherServlet': initialization started
2019-01-25 03:15:57.218  INFO 10771 --- [nio-8080-exec-1] o.s.web.servlet.DispatcherServlet        : FrameworkServlet 'dispatcherServlet': initialization completed in 38 ms
^C2019-01-25 03:17:59.580  INFO 10771 --- [       Thread-5] ConfigServletWebServerApplicationContext : Closing org.springframework.boot.web.servlet.context.AnnotationConfigServletWebServerApplicationContext@47089e5f: startup date [Fri Jan 25 03:15:01 UTC 2019]; root of context hierarchy
2019-01-25 03:17:59.586  INFO 10771 --- [       Thread-5] o.s.j.e.a.AnnotationMBeanExporter        : Unregistering JMX-exposed beans on shutdown
$ 
```
