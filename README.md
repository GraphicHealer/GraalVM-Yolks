# GraalVM
GraalVM Based Java Yolks for Pterodactyl Panel, for running enhanced Java-Based Minecraft Servers.

Created because of this document: https://github.com/brucethemoose/Minecraft-Performance-Flags-Benchmarks#graalvm-enterprise-edition

# Available Images

* [`java`](/java)
  * [`java17`](/java/17)
    * `ghcr.io/graphichealer/graalvm-yolks:java_17`

# Installation
1. Select a Docker Image URL from above.
2. On Pterodactyl Panel, go to `Admin > Servers > [YOUR SERVER] > Startup > Docker Image Configuration`
3. Enter the Docker Image URL into the Higlighted Box:
![image](https://github.com/user-attachments/assets/8cee1d08-a8ae-4336-89f2-94945ddb690a)
4. Click `Save Modifications` near the top on the right.
5. Done! Your Pterodactyl Server will Re-Install the Docker Image, and update you to GraalVM-EE Java!

# Contributing

When adding a new version to an existing image, such as `java v42`, you'd add it within a child folder of `java`, so
`java/42/Dockerfile` for example. Please also update the correct `.github/workflows` file to ensure that this new version
is tagged correctly.
