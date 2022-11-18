# minecraft-deobfuscated

This is a deobfuscated version of Minecraft 1.8.8. It is intended for use in libraries that need to access Minecraft's code, but do not want to depend on the obfuscated version of Minecraft.

<!-- TOC -->
* [minecraft-deobfuscated](#minecraft-deobfuscated)
    * [Examples](#examples)
  * [Versions](#versions)
  * [Usage](#usage)
<!-- TOC -->

## Examples 
### [client-commons](https://github.com/dev-vince/client-commons)

```java
package dev.vince.commons;

import net.minecraft.client.Minecraft;

/**
 * The MinecraftInterface is a class that allows you to access multiple Minecraft variables/methods without having to use the Minecraft class.
 * It is recommended to use this class instead of the Minecraft class.
 * It is also recommended to use this class instead of creating instance fields extending Minecraft.
 *
 * @author dev-vince
 */
public interface MinecraftInterface {
    Minecraft mc = Minecraft.getMinecraft();
}
```



## Versions

| Supported Versions | Package                                |
|--------------------|----------------------------------------|
| 1.8.8              | dev.vince.minecraft-deobfuscated:1.8.8 |

## Usage
To import the library using maven, add the following to your `pom.xml`:

```xml
<repositories>
    <repository>
        <id>github</id>
        <url>https://maven.pkg.github.com/dev-vince/minecraft-deobfuscated</url>
    </repository>
</repositories>

<dependencys>
    <dependency>
        <groupId>dev.vince</groupId>
        <artifactId>minecraft-deobfuscated</artifactId>
        <version>1.8.8</version>
    </dependency>
</dependencys>
```
otherwise, you can download the jar from the [package](https://github.com/dev-vince/minecraft-deobfuscated/packages) page.
