# Mixtape
> [!CAUTION]
> **Mixtape is heavily work-in-progress, and not yet ready for production use.** It likely will not be ready for a very long time; this repository is meant to track the progress of implementation and to build up support for the project.

Mixtape is a modding framework for the game Cassette Beasts. It allows for mod authors to implement new features into the game with minimal headache and maximum interopability, all while _avoiding "coremodding"_ (i.e. directly editing the code of the base game) on the end of the user as much as possible.

## TODO
- [ ] **Utility and core modules**
  - [ ] **`Mashup`, used to manipulate internal Cassette Beasts code without _directly_ using `ResourceSaver`, `Resource.take_over_path()`, or the currently-prevalent class-patcher of Mod Utils.**
  - [ ] `MixtapeConfig`, used to add settings to mods through the main menu
  - [ ] `MixtapeLoader`, the modloader; mods registered through Mixtape are able to work together in a lot of respects
    - [ ] `MixtapeCache`, the capability for the modloader to preserve content from mods that have been uninstalled and remove content from saves that have had a mod uninstalled from them
  - [ ] `MixtapeLog`, used to directly report facets of the game's information to a file to give mod authors greater information in bug reports
  - [ ] `MixtapeMeshInjector`, the combination of an editor plugin and core module that works with the Godot editor to allow for generated `MeshLibrary` instances to be used when designing scenes with the `GridMap`, using the `SceneInjector` to automatically locate the respective meshes and load them into a given scene.
- [ ] **Modules for implementing features into the game**
  - [ ] Moves
  - [ ] Status effects
  - [ ] Implementation of complex, programmatic VFX
  - [ ] Custom types and type interactions
  - [ ] Consumable and "reference" (i.e. Ranger Handbook) items
    - [ ] Tapes associated with custom types
  - [ ] Player cosmetics
  - [ ] Partners, rangers, merchants, and other NPCs
  - [ ] Models (specifically `MeshLibraryFragment` and `SceneInjector`)
  - [ ] Worlds and associated maps for those worlds
  - [ ] Localization keys and values for mods
  - [ ] _Bespoke player movement abilities?_ (maybe a later update)
