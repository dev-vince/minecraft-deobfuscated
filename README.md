# minecraft-deobfuscated

This is a deobfuscated version of Minecraft 1.8.8. It is intended for use in libraries that need to access Minecraft's code, but do not want to depend on the obfuscated version of Minecraft.

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
        <url>https://repo.vince.dev/repository/maven-public/</url>
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