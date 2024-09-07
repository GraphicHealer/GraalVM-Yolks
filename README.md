# GraalVM
GraalVM Based Java Yolks for Pterodactyl Panel, for running enhanced Java-Based Minecraft Servers.

Created because of this document: https://github.com/brucethemoose/Minecraft-Performance-Flags-Benchmarks#graalvm-enterprise-edition

# Installation
1. Select the correct Docker Image URL.
   Use the Following Format:
   ```
   ghcr.io/GraphicHealer/Pterodactyl-GraalVM-Yolks:java_<Version>
   ```
   For Example, if you need Java 17, use the `java_17` tag:
   ```
   ghcr.io/GraphicHealer/Pterodactyl-GraalVM-Yolks:java_17
   ```
3. On Pterodactyl Panel, go to `Admin > Servers > [YOUR SERVER] > Startup > Docker Image Configuration`
4. Enter the Docker Image URL into the Higlighted Box:
![image](https://github.com/user-attachments/assets/8cee1d08-a8ae-4336-89f2-94945ddb690a)
5. Click `Save Modifications` near the top on the right.
6. Done! Your Pterodactyl Server will Re-Install the Docker Image, and update you to GraalVM-EE Java!

# Available Images

* [`java`](https://github.com/GraphicHealer/Pterodactyl-GraalVM-Yolks/tree/master/java)
  * [`java17`](https://github.com/GraphicHealer/Pterodactyl-GraalVM-Yolks/tree/master/java/17)
    * `ghcr.io/GraphicHealer/Pterodactyl-GraalVM-Yolks:java_17`

# Contributing

When adding a new version to an existing image, such as `java v42`, you'd add it within a child folder of `java`, so
`java/42/Dockerfile` for example. Please also update the correct `.github/workflows` file to ensure that this new version
is tagged correctly.
