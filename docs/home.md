---
title: Text Decal
description: Text Decal lets you display dynamic text as decals directly on any surface in Unity
layout: libdoc_page.liquid
permalink: index.html
date: false
---

## Quick Setup
### URP
1. Add [`Decal Renderer Feature`](https://docs.unity3d.com/Documentation/Manual/urp/renderer-feature-decal-reference.html) and `Text Decal Renderer Feature` to your URP Renderer  with `DBuffer` or `Screen Space` technique.
2. Ensure the `TextMeshPro` package is installed and import `TextMeshPro Essentials`
3. Create a custom `TMP_Font Asset` from a chosen font and apply the shader `Text Decal/Distance Field SSD [Unlit | URP Lit]` to it.
4. Add the `Rendering → Text Decal` component to a 3D TextMeshPro object and assign the custom font asset.
5. Configure the `Text Decal` component and text material, ensuring you set the `Projection Depth` properly.

### HDRP
{% alert 'HDRP is currently not supported', 'warning', 'Note' %}