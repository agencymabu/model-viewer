
# 3D Model-Viewer
Web Component to easily embed 3D files to HTML pages using BabylonJS.

Forked from https://github.com/RussoFaccin/model-viewer. This fork has been modified for specific applications and is not meant for general use. You should probably use the original repo for your own project.

### Demo

Setup
1. Clone this repo
2. `$ yarn` in repo root dir ([don't have yarn?](https://classic.yarnpkg.com/lang/en/docs/install/#windows-stable))
3. `$ yarn run build` in repo root dir

Run
1. `$ yarn http-server .` in root dir
2. Visit [localhost:8080/examples/iframe.html](http://localhost:8080/examples/iframe.html) to view

### Usage
Include BabylonJS engine script. [Get here](https://doc.babylonjs.com/babylon101/how_to_get)

    <script  src="https://cdn.babylonjs.com/babylon.js"></script>
---
Include BabylonJS file loader

    <script src="https://cdn.babylonjs.com/loaders/xxx"></script>
where **xxx** can be any file from [https://github.com/BabylonJS/Babylon.js/tree/master/dist/loaders](https://github.com/BabylonJS/Babylon.js/tree/master/dist/loaders)

---
Include model-viewer script

	<script src="dist/model-viewer.min.js"></script>
***
Include model-viewer tag in HTM

    <model-viewer src="https://googlewebcomponents.github.io/model-viewer/examples/assets/DamagedHelmet/DamagedHelmet.gltf" camradius="3" yoffset="-0.15" bgcolor="#dbdbdb"></model-viewer>

### Attributes
|**Attribute**|**Value**|**Description**|
|--|--|--|
|src|(required)<br/>url: string|Specifies the URL of the 3D model|
|camradius|(optional)<br/>number|The radius distance from camera to target|
|yoffset|(optional)<br/>number|The Y axis offset distance the camera look from target origin|
|bgcolor|(optional)<br/>hex color number|Defines the Skybox texture color