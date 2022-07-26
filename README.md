# rkon-core

> :warning: **This repository is archived and thus not maintained anymore.**

This is a library for the [Source RCON Protocol](https://developer.valvesoftware.com/wiki/Source_RCON_Protocol), it is intended for raw use; there are no presets or built-in commands.

## Usage
```java
// Connects to 127.0.0.1 on port 27015
Rcon rcon = new Rcon("127.0.0.1", 27015, "mypassword".getBytes());

// Example: On a minecraft server this will list the connected players
String result = rcon.command("list");

// Display the result in the console
System.out.println(result);
```
When connecting to the rcon server, an `AuthenticationException` will be thrown if the password is incorrect.

## Download
The latest packed .jar, ready to use as a library, is available [here](https://github.com/Kronos666/rkon-core/releases/latest).

### Maven 
[![](https://www.jitpack.io/v/Sunshine-wzy/rkon-core.svg)](https://www.jitpack.io/#Sunshine-wzy/rkon-core)
```xml
<repository>
    <id>jitpack.io</id>
    <url>https://jitpack.io</url>
</repository>

<dependency>
    <groupId>com.github.Sunshine-wzy</groupId>
    <artifactId>rkon-core</artifactId>
    <version>1.2.2</version>
</dependency>
```
