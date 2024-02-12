---
title: "Development Note #0001"
summary: "Tips/Notes for Unreal Engine from January 2024."
date: 2024-02-11
tags:
   - dev note
   - unreal engine
author: "a_nightails"
---
## Introduction 👋
Welcome to my first development note. This is a series of posts about documenting tips/notes that I gathered during
a personal project's development.

For this week, I have some notes relate to the `UActorComponent` and `UMaterialInstanceDynamic` from Unreal Engine.

## Note 📝
 - To set `CastShadow` value at runtime, use `SetCastShadow()` function from the `UActorComponent` class. This function will
force the component to update in the next frame. Set variable directly will only work during construction.
 - To create a `UMaterialInstanceDynamic` use the static function `UMaterialInstanceDynamic::Create(Material, UObject);`
   - Parameter: Material -> the parent material that need to be converted to instance dynamic.
   - Parameter: UObject -> the world object in the game, use `this` keyword is sufficient.
 - To have `UPROPERTY` be placed in a specific spot in the detail panel, use `DisplayPriority` or `DisplayAfter` in `meta` specifier.
 - To initialize an empty array of given type and given size, use `Array.Init({}, size);`
   - `{}` also work for passing an empty parameter, not pointer.