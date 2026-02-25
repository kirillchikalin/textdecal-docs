---
title: Text Decal
description: Create dynamic, surface-aligned text decals with realistic shading at runtime in Unity
layout: libdoc_page.liquid
permalink: index.html
date: false
---
![Text Decal on the Unity Asset Store](https://textdecal.chikalin.space/assets/og-image.png)
## Getting started
1. **Add** [`Decal Renderer Feature`](https://docs.unity3d.com/Documentation/Manual/urp/renderer-feature-decal-reference.html) and `Text Decal Renderer Feature` to your URP Renderer.
2. **Create** a custom `TMP_Font Asset` and apply the shader `Text Decal/Distance Field SSD [Unlit | URP Lit]` to it.
3. **Attach** the `Rendering → Text Decal` component to a 3D TextMeshPro object, **assign the custom font you created**, and configure it.