# WavesFX (Signalyze Edition)


WavesFX (Signalyze Edition) is an open-source [Waves](https://wavesplatform.com) wallet for Windows, macOS and Linux.

Releases can be found on the [release](https://github.com/wavesfx/wavesfx/releases) list.


# How to build WavesFX

## 1. Prerequisites

### Install Java Development Kit (JDK) 14

[OpenJDK](https://jdk.java.net/14/) and [AdoptOpenJDK](https://adoptopenjdk.net/archive.html) are excellent choices. 

## Install JDK 14 Ubuntu 18

Ubuntu, Linux Mint, Pop!_OS and other Linux distributions based on Ubuntu: open a terminal and use the commands below to add the Linux Uprising Oracle Java PPA and install Oracle Java 14 (Oracle JDK 14) for 64bit:

```
sudo add-apt-repository ppa:linuxuprising/java
sudo apt update
sudo apt install oracle-java14-installer
sudo apt update
sudo apt-get install oracle-java14-installer
```

After install check your version of Java in terminal with 

```
java --version
```

You should see output that matches the following

```
java 14.0.1 2020-04-14
Java(TM) SE Runtime Environment (build 14.0.1+7)
Java HotSpot(TM) 64-Bit Server VM (build 14.0.1+7, mixed mode, sharing)
```

## 2. Obtain Source Code

```
git clone github.com/Signalyze/Signalyze.git
cd Signalyze
```
## 3. Compilation and packaging
### Build binary package
```
./gradlew jpackageImage 
```
Package will be located in `build/jpackage`   

### Build installer
**Note:** Wix, a third-party tool, is required to generate an installer for Windows.
```
./gradlew jpackage
```
### How to run

after the above has finsihed navigate to  

```
wavesfx/install/wavesfx/bin

```

and launch with 

```
./wavesfx
````

# Bug Reports
Please use the issue tracker provided by GitHub to send bug reports or feature requests.
