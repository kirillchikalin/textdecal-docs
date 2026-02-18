---
title: Rendering layers
description: Rendering Layers determine which objects the decal will project onto
layout: libdoc_page.liquid
permalink: features/layers/index.html
eleventyNavigation:
    key: Rendering layers
---

1. **Enable Rendering Layers in URP Settings:**
    - Go to `Universal Renderer Data` asset.
    - Ensure that `Use Rendering Layers` are enabled in the `Renderer Features → Decal` settings.

2. **Set Rendering Layers on Decal Object:**
    - Select the 3D TextMeshPro object with the `Text Decal` script attached.
    - In the **Inspector**, locate the material settings, in the `Rendering Layers` dropdown assign the desired rendering layer(s) for the decal.

3. **Assign Rendering Layers to Target Surfaces:**
    - Select the objects in your scene that you want the decal to project onto.
    - In the **Inspector**, locate the `Mesh Renderer → Additional Settings → Rendering Layer Mask` dropdown.
    - Ensure these objects are assigned to the same rendering layer(s) as the decal.

> **Tip:** Use unique layers to isolate specific decals to certain surfaces, making it easier to manage complex scenes.