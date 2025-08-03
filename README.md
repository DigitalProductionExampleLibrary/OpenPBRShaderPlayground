![OpenPBR Shader Playground](https://raw.githubusercontent.com/AcademySoftwareFoundation/OpenPBR/main/images/OpenPBR_title.jpg)

# OpenPBR Shader Playground Asset

> [!IMPORTANT]
> While fully supported by the latest MaterialX and OpenUSD library versions, the OpenPBR Shader Playground asset may image differently from application to application as DCC and renderer adoption of OpenPBR is still a work in progress. See the “Status” section below.

Created to illustrate a modern look-development approach, OpenPBR Shader Playground uses the recently released [OpenPBR Surface](https://academysoftwarefoundation.github.io/OpenPBR/), a surface shading model developed by Adobe and Autodesk that can serve as an industry standard for computer graphics. Designed as an über-shader, OpenPBR Surface aims to provide a material representation capable of accurately modeling the vast majority of CG materials used in practical visual effects and feature animation productions. OpenPBR Shader Playground utilizes configurations that highlight novel aspects of OpenPBR, such as new fuzz, metal, emission, volume, and thin-wall behaviors. 

OpenPBR Shader Playground is expressed using [OpenUSD](https://aousd.org/blog/explainer-series-what-is-openusd), which references material networks composed of standard MaterialX and OpenPBR node definitions contained within [MaterialX](https://materialx.org/) documents. The scene was originally created by Adobe in Autodesk Maya and converted to USD and MaterialX in Omniverse by NVIDIA. Renders were produced using Arnold for Maya and NVIDIA Omniverse. 

## Status

***OpenPBR Shader Playground implements the latest [OpenPBR v1.1 specification](https://academysoftwarefoundation.github.io/OpenPBR/).*** It is supported in [MaterialX](https://github.com/AcademySoftwareFoundation/MaterialX) v1.39.3+ and [OpenUSD](https://github.com/PixarAnimationStudios/OpenUSD/) v0.25.05+.

As DCC and renderer integration of OpenPBR is still a work in progress, support may vary from application to application, and the asset may load or image differently depending on context. It has been tested in the following environments:
* Adobe Substance: Loads in latest version, fully supported rendering in an upcoming release
* Autodesk Maya: Loads and renders in Maya 2026 with [Arnold v7.4 and MtoA v5.5](https://help.autodesk.com/view/MAYAUL/2026/ENU/?guid=GUID-C9B5B872-A14A-4A73-9BEE-7668EC35AAD6), or Viewport 2.0

While the asset will render in these contexts, there are a number of [known issues](https://github.com/DigitalProductionExampleLibrary/OpenPBRShaderPlayground/issues) with the current material setup that may result in differences in appearance between renderers, or between the current version of the asset and prior renders from the original Maya-based asset. *The goal of this project is to refine the asset such that it can ultimately be a standard reference and validation for clients wishing to integrate with OpenPBR, as well as for the MaterialX and OpenUSD projects themselves.*

We welcome you to join the effort by filing issues for any identified gaps or inconsistencies with the specification, contribute updates to the asset, or help validate DCC and renderers with successful integrations.
