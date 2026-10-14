# PlayblastXR v5

This update represents a major rewrite to the previous PlayblastVR v4 immersive previz toolset that supported 18 different image projections. Lightfielder PlayblastXR v5 is latest & greatest edition of PlayblastVR, with a planned release date of mid-November 2026.

You will be able to enjoy this refreshed software as free, LGPL licensed open-source tools, too! 🇨🇦

> Upcoming major feature additions for PlayblastXR include new DCC host application support for the [Rumba animation](https://rumba-animation.com) software with a [C++ plug-in integration](https://rumba-animation.com/doc/1.2/cpp/examples.html), and [SideFX Houdini Apprentice/Indie](https://www.sidefx.com/products/houdini-indie/) compatible PlayblastXR shelf tools, HDAs, and TOPs / COPs nodal workflows for neural inverse rendering, DLSS like video-to-video, and video-to-mesh stylization approaches. 

## What's New

PlayblastXR v5 ships with an interactive viewport that delivers AOVs (Arbitrary Output Variables) directly from the real-time hardware accelerated graphics framebuffer. The multi-channel / multi-layer image data can be bounced to disk, accessed via in-memory zero copy techniques, or pixel streamed as [OpenPBR](https://github.com/AcademySoftwareFoundation/OpenPBR) compatible render passes. 

When you render 2D/3D animation sequences as playblasts, they now include the option of delivering extra AOVs. This is super handy for interactive relighting in post, and for creative stylization purposes inside of a larger "hybrid" content creation pipeline that includes "Renderless Compositing" tools for multi-pass and light-select pass adjustments. 

You can take things even further, when the pixel streamed AOV data is used with ControlNet concepts, that rely on per-take [OpenPose](https://cmu-perceptual-computing-lab.github.io/openpose/web/html/doc/index.html) rig exports of humanoid-like or quadruped characters. 

To help the PlayblastXR technology work inside a colour-managed "film-quality" workflow, you can render to HDR output, and deliver image metadata or sidecar files with OpenCV compatible [Brown Conrady](https://en.wikipedia.org/wiki/Distortion_(optics)) lens model K1-K3 lens distortion profiles / [STMaps](https://docs.google.com/document/d/1lQ-wc9ucLJqj-HL7iKMNWA71klV5O1fk2-JicRB6gDY/edit?usp=sharing) warping templates, and more.

## Overview

PlayblastXR brings previz and techviz tools into the lightfield domain with hardware accelerated 6DoF image based rendering. PlayblastXR is built on-top of 16 years of prior-art development work to create a next-generation SOTA (State of the Art) solution.

This toolset is the direct sequel to [RocketComp](https://www.cgchannel.com/2015/07/andrew-hazelden-releases-rocketcomp-for-maya/), [PlayblastVR for Maya](https://www.cgchannel.com/2016/07/andrew-hazelden-releases-playblastvr-for-maya-v2-0/)/[Softimage](https://www.cgchannel.com/2015/11/andrew-hazelden-releases-playblastvr-for-softimage/), [Kartaverse/KartaVR](https://kartaverse.github.io/Kartaverse-Docs/), and the [Domemaster3D](https://github.com/zicher3d-org/domemaster-stereo-shader/releases) lens shaders.

## Immersive XR Output Formats

PlayblastXR allows you to work with multi-view camera rig presets sourced from SfM calibrated camera arrays. The recommended general purpose container format right now, is the Lightfielder [PBR-GS](https://github.com/Lightfielder/PBR-GS) and [OBJ-GS](https://github.com/Lightfielder/PBR-GS/blob/master/OBJ-GS.md) open formats. 

The upcoming PlayblastXR API will be available for user-defined input/output file format additions, and other forms of customization to the core capabilities of the software.

Detailed R&D work is going into the implementation of "direct to splat" based volume baking tools. This is targeted at [3DGS/4DGS](https://en.wikipedia.org/wiki/Gaussian_splatting) Gaussian Raytraced sequences, NVIDIA [InstantNGP](https://nvlabs.github.io/instant-ngp/) compatible [NeRF](https://en.wikipedia.org/wiki/Neural_radiance_field), and [DeepEXR](https://openexr.com/en/latest/InterpretingDeepPixels.html) image sequence output. 

Since 2024, Lightfielder development has operated as a licensed 3rd party [GoGhost Evotis](https://go-ghost.com/) solutions developer. This means PlayblastXR will support a larger ecosystem push to have GoGhost Evotis non-uniform .evol media format used broadly across creative workflows.

The Evotis technology is, in our professional view, the BAYER RAW media "final endgame" like image format for the media sector, that all other image container implementations will inevitably arrive/converge on for capabilities over the next 20 years+. 

Evotis represents the end of discreet RGB pixels as the smallest addressable sample, it allows non-uniform sub-pixel elements to be used with raytraced "stochastic composited" image sample data storage and retrieval. Evotis goes below the pixel grid, to render and store individual ray samples in a way few have even considered or pondered, yet. It's truly revolutionary technology.

## Multi-View and Multi-Pass Playblasts

A key advantage of adopting lightfield rendering techniques, is the way it provides free-view navigation of your pre-rendered character animation work. This is great for previz artists working on AAA level game cinematics, feature animation, virtual production VAD (art departments) delivering XR stage content, real-time immersive projects, or fulldome show production.

With full PlayblastXR renders you automatically get immersive playback options natively on [Apple Vision Pro](https://www.apple.com/apple-vision-pro/), as well as [OpenDisplayXR](https://opendisplayxr.github.io/OpenDisplayXR/) / [Monado OpenXR](https://gitlab.freedesktop.org/monado/monado) usage for [Meta Quest Horizon](https://horizon.meta.com/) HMDs, and Passive/Active Stereo 3D display systems. 

Lightfielders get to enjoy the powerful nature of a "frameless" media container format that allows cinematographers to dynamically reframe and modify their camera animation work. Also, [PBR-GS](https://github.com/Lightfielder/PBR-GS) licensed tools support interactive scene relighting capabilities, that happen "downstream" of the initial playblast output since the pipeline tools operate in the volumetric domain.

