---
title: URP Setup
description: Detailed setup for URP
layout: libdoc_page.liquid
permalink: setup/urp/index.html
eleventyNavigation:
    key: URP
    parent: Setup
---

## Configure Universal Render Pipeline

1. Open your `Universal Renderer Data` asset
    - _you can find the location through_ `Universal Renderer Pipeline Asset → Renderer List`.
2. In the `Renderer Features` section:
    - click `Add Renderer Feature → Decal`.
    - click `Add Renderer Feature → Text Decal`.
3. Set `Decal Technique` to either `DBuffer` or `Screen Space`.
    {% alert 'To use the `DBuffer` mode with `Text Decal Renderer`, enable it in the `Decal Renderer` and configure the settings accordingly. `Automatic` mode is not supported.', 'success', 'Note' %}

## Set Up TextMesh Pro with Decal Shader

1. **Create TMP_Font Asset:**
    - Select the font you want to use in the Project window.
    - Right-click the font and choose `Create → TextMeshPro → Font Asset → SDF`.
    - This will generate a `TMP_Font Asset`.

2. **Assign Decal Shader:**
    - Select the created `TMP_Font Asset`.
    - In the **Inspector**, locate the `Atlas & Material`, double click to the `Font Material` field value.
    - Click the shader dropdown and choose one of the following:
        - `Text Decal/Distance Field SSD Unlit` – Use for unlit rendering.
        - `Text Decal/Distance Field SSD URP Lit` – Use for lit rendering.

## Using the Decal in the Scene

1. Add a 3D TextMeshPro object to your scene
   - `Game Object → 3D Object → Text - TextMeshPro`.
2. Attach the `Text Decal` script to the object by clicking `Add Component` in the **Inspector**:
    - You can find the script at: `Packages/Text Decal/Runtime/TextDecal.cs`.
3. Assign the `TMP_Font Asset` you created in _Step 2_ with the shader applied
   - by selecting it in the `Font Asset` property of the `TextMeshPro - Text` component.
4. Adjust `Projection Depth` and `Rendering Layers` in the **Inspector**:
    - `Projection Depth` controls how far the decal projection extends.
    - `Rendering Layers` allows you to control where the decal appears.