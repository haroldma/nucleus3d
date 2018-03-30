# nucleus3d (alpha)

A 3d framework for web devs. Powered by Babylon.JS. TypeScript first. Entity-Component architecture.

## Set Up

`npm install nucleus3d`

## Docs

Read the [Nucleus3D wiki](https://github.com/haroldma/nucleus3d/wiki) to go learn more in depth about the framework!

### The Basics

**Entities** are things in the 3D world. They're merely placeholders for components.

**Components** are modular chunks of data that can add appearance, behaviors and/or functionality to an entity.

**Systems** provide global scope, services, and management to classes of components.

## Quick Start

## The Baskeball Demo

[Make a simple bouncing basketball using Nucleus3D](https://stackblitz.com/edit/nucleus-basketball?embed=1&file=app.ts).

### The Model Loader

```
// Create a scene entity and mount it with an engine
const sceneEntity = new SceneEntity();
sceneEntity.mount(new BABYLON.Engine());

const entity = new Entity();
entity.addComponent(new ModelLoader('https://raw.githubusercontent.com/KhronosGroup/glTF-Sample-Models/master/2.0/BoomBox/glTF/BoomBox.gltf'));

// Mount the entity
sceneEntity.mountChild(entity);
```
