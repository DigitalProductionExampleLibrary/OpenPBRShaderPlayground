![OpenPBR Shader Playground](https://raw.githubusercontent.com/AcademySoftwareFoundation/OpenPBR/main/images/OpenPBR_title.jpg)

# OpenPBR Shader Playground Asset

> [!WARNING]
> The OpenPBR Shader Playground asset is currently in Beta and may not be usable or imageable out of the box.  See "Status" below.

Created to illustrate a modern look-development approach, OpenPBR Shader Playground uses the recently released [OpenPBR Surface](https://academysoftwarefoundation.github.io/OpenPBR/), a surface shading model developed by Adobe and Autodesk that can serve as an industry standard for computer graphics. Designed as an über-shader, OpenPBR Surface aims to provide a material representation capable of accurately modeling the vast majority of CG materials used in practical visual effects and feature animation productions. OpenPBR Shader Playground utilizes configurations that highlight novel aspects of OpenPBR, such as new fuzz, metal, emission, volume, and thin-wall behaviors. 

OpenPBR Shader Playground is expressed using [OpenUSD](https://aousd.org/blog/explainer-series-what-is-openusd), which references material networks composed of standard MaterialX and OpenPBR node definitions contained within [MaterialX](https://materialx.org/) documents. The scene was originally created by Adobe in Autodesk Maya and converted to USD and MaterialX in Omniverse by NVIDIA. Renders were produced using Arnold for Maya and NVIDIA Omniverse. 

## Status

***OpenPBR Shader Playground is currently in Beta and may not be usable or imageable out of the box***, as OpenPBR is not yet supported by OpenUSD.  

While support for [OpenPBR v1.1](https://github.com/AcademySoftwareFoundation/OpenPBR/releases/tag/v1.1) was officially released with [MaterialX v1.39.0](https://github.com/AcademySoftwareFoundation/MaterialX/releases/tag/v1.39.0), OpenUSD is currently limited to MaterialX v1.38.10 which does not support OpenPBR (as of [OpenUSD v0.24.08](https://github.com/PixarAnimationStudios/OpenUSD/blob/v24.08/VERSIONS.md)). Work to support MaterialX versioning in OpenUSD is currently in progress ([MaterialX Versioning in OpenUSD Proposal](https://github.com/PixarAnimationStudios/OpenUSD-proposals/tree/main/proposals/materialx-versioning)) and is the first step in enabling support for OpenPBR and this asset within OpenUSD.

**Using or imaging this asset short of that work requires patching and compiling OpenUSD**.

While the asset is in Beta and OpenPBR/OpenUSD integration work is in progress, this GitHub repository is being provded by DPEL to facilitate collaboration.

OpenPBR Shader Playground will be officially released and available on the DPEL site once this work is complete and the asset is out of Beta.