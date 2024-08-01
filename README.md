# Let's Play with Java

## Abstract

I would like to finally become a bit proficient writing implementation of API (endpoints) in Java. I will of course (re-)start from the "Hello, World!" program written in Java, and then we will see...

## Setting up a Java Development Kit

There is a one-stop page that always refers to the latest version of the JDK: <https://jdk.java.net/>. Selecting the latest "Ready for use" JDK version takes you to a page where you can download the version of the JDK you need.

### Setting up a JDK for Windows/x64

1\. Go to <https://jdk.java.net/>.

2\. Click on the "JDK 22" link, <https://jdk.java.net/22/>.

3\. Then, click on "zip" link next to "Windows/x64 ", <https://download.java.net/java/GA/jdk22.0.2/c9ecb94cd31b495da20a27d4581645e8/9/GPL/openjdk-22.0.2_windows-x64_bin.zip>.

4\. Unzip the file `openjdk-22.0.2_windows-x64_bin.zip` into the folder `C:\Users\{Username}\AppData\Local\Programs`, it will create the sub-folder `jdk-22.0.2` in it.

> ***Note:*** You may have to create the sub-folder `Programs` within the folder `C:\Users\{Username}\AppData\Local`.

5\. Open a _Command Prompt_ and type the following command:

```text
setx JAVA_HOME "%PATH%;C:\Users\{Username}\AppData\Local\Programs\jdk-22.0.2`
```

```text
setx PATH %JAVA_HOME%\bin;%PATH%
```

6\. To verify the installtion, close the _Command Prompt_, open a new one, and type the following commands:

```text
java -version
```

```text
javac --version
```

## Setting up a JDK for Linux/x64

We will use the _Ubuntu Playground_ from [Killercoda](https://killercoda.com/about) on which I will install the **Linux/x64** build. Many thanks again to the Killercoda team to provide such environment for free!

1\. Go to <https://killercoda.com/playgrounds/scenario/ubuntu> and register if necessary.

... to be continued ...

## References

* (n.d.). _Java Tutorial_. W3Schools. Retrieved October 18, 2023, from <https://www.w3schools.com/java/default.asp>

* (n.d.). _JDK Installation Guide. Oracle_. Retrieved October 18, 2023, from <https://docs.oracle.com/en/java/javase/21/install/installation-jdk-linux-platforms.html#GUID-CF001E7F-7E0D-49D4-A158-9CF3ED4C247C>

* (n.d.). _Getting Started with Java_. Retrieved August 1, 2024, from <https://dev.java/learn/getting-started/>
