
<div id="top"></div>

<!-- PROJECT SHIELDS -->
<!--
*** I'm using markdown "reference style" links for readability.
*** Reference links are enclosed in brackets [ ] instead of parentheses ( ).
*** See the bottom of this document for the declaration of the reference variables
*** for contributors-url, forks-url, etc. This is an optional, concise syntax you may use.
*** https://www.markdownguide.org/basic-syntax/#reference-style-links
-->
[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]
[![APACHE-2.0 License][license-shield]][license-url]

<!-- PROJECT LOGO -->
<br />
<div align="center">
  <a href="https://github.com/WorldSeedMMO/WorldSeedEntityEngine">
    <img src=".github/icon.png" alt="Logo" width="180" height="180">
  </a>

  <h3 align="center">WSEE</h3>

  <p align="center">
    WorldSeed Entity Engine
    <br />
    <br />
    <br />
    <a href="https://github.com/WorldSeedMMO/WorldSeedEntityEngine/issues">Report Bug</a>
    ·
    <a href="https://github.com/WorldSeedMMO/WorldSeedEntityEngine/issues">Request Feature</a>
  </p>
</div>

<!-- ABOUT THE PROJECT -->
## About The Project
<div align="center">
  <a href="https://github.com/WorldSeedMMO/WorldSeedEntityEngine">
    <img src=".github/demo.gif" alt="Logo" width="320" height="240">
  </a>
  </div>

This is a library that allows users to add bedrock models from blockbench in to **Vanilla Minecraft**!

WSEE lets you create multipart entities with Armor Stands, as well as Zombies for much smoother animations.
The framework provided allows users to easily create multipart entities, define animations, and write AI that fully utilises the entity's animations.

Currently WSEE only supports [Minestom](https://github.com/Minestom/Minestom)

<!-- GETTING STARTED -->
## Getting Started

A full, runnable example server can be found in [here](https://github.com/WorldSeedMMO/WorldSeedEntityEngine/tree/master/src/test/java)

### Adding as a dependency

Add the following to your `build.gradle.kts` file:

```
repositories {
    maven("https://reposilite.worldseed.online/public")
}
```

Add the library as a dependency
```
dependencies {
    implementation("net.worldseed.multipart:WorldSeedEntityEngine:<version>")
}
```

The lastest version number can be found [here](https://reposilite.worldseed.online/#/public/net/worldseed/multipart/WorldSeedEntityEngine)

## Restrictions

Some restrictions are imposed by Minecraft
- Cubes can only be rotated on one axis, and can only have rotation values of 0, -22.5, 22.5, 45 or -45. This does not effect bones (these show up as folders in blockbench)
- Bones can only be 64 blocks in size

## [Wiki](https://github.com/WorldSeedGames/WorldSeedEntityEngine/wiki)
Learn what this project is, how it works and how you can use it on your server

## FAQ

Q: Why are my bones positioned incorrectly in minecraft?\
A: Entities used for bones will be placed at the pivot point of the bone in blockbench. To fix this, move the pivot point closer to the bone


Q: Why are my hitboxes in the wrong place?\
A: Slime entities for hitboxes are placed at the bone pivot point, not the block location.

<p align="right">(<a href="#top">back to top</a>)</p>

<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[contributors-shield]: https://img.shields.io/github/contributors/WorldSeedMMO/WorldSeedEntityEngine.svg?style=for-the-badge
[contributors-url]: https://github.com/WorldSeedMMO/WorldSeedEntityEngine/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/WorldSeedMMO/WorldSeedEntityEngine.svg?style=for-the-badge
[forks-url]: https://github.com/othneildrew/Best-README-Template/network/members
[stars-shield]: https://img.shields.io/github/stars/WorldSeedMMO/WorldSeedEntityEngine.svg?style=for-the-badge
[stars-url]: https://github.com/WorldSeedMMO/WorldSeedEntityEngine/stargazers
[issues-shield]: https://img.shields.io/github/issues/WorldSeedMMO/WorldSeedEntityEngine.svg?style=for-the-badge
[issues-url]: https://github.com/WorldSeedMMO/WorldSeedEntityEngine/issues
[license-shield]: https://img.shields.io/github/license/WorldSeedMMO/WorldSeedEntityEngine?style=for-the-badge
[license-url]: https://github.com/WorldSeedMMO/WorldSeedEntityEngine/blob/master/LICENSE
