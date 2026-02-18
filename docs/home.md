---
title: Text Decal
description: Text Decal lets you display dynamic text as decals directly on any surface in Unity
layout: libdoc_page.liquid
permalink: index.html
date: false
---

## Dependencies

## Quick Setup
### URP
1. Add [`Decal Renderer Feature`](https://docs.unity3d.com/Documentation/Manual/urp/renderer-feature-decal-reference.html) to your URP Renderer.
    {% alert 'Select `DBuffer` or `Screen Space` technique.', 'success', 'note' %}
2. Add `Text Decal Renderer Feature`.
3. Ensure the `TextMeshPro` package is installed and import `TextMeshPro Essentials`
    {% alert 'TextMesh Pro included in Unity UI package since Unity 6', 'success', 'note' %}
4. Create a custom `TMP_Font Asset` from a chosen font and apply the shader `Text Decal/Distance Field SSD [Unlit | URP Lit]` to it.
5. Add the `Rendering → Text Decal` component to a 3D TextMeshPro object and assign the custom font asset.
6. Configure the `Text Decal` component and text material, ensuring you set the `Projection Depth` properly.
7. PROFIT!

### HDRP
{% alert 'HDRP currently not supported', 'warning', 'Note' %}