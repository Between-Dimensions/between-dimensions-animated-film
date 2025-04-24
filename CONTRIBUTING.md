# Contributing

## Constraints

- Animations should be capped to **30 FPS**???.
- Shot assembly. Each part of the shot will be a separate `.blend` file?????
- Everyone on the team should use the same blender version.

## Project Structure

```plaintext
│
├── .git
├── .gitignore
├── render # render frames (local, not tracked by git)
├── shared # Stores large files (shouldn't be tracked by git, google drive????)
└── blend
    │
    ├── assets
    │   ├── chars # Characters
    │   │   ├── dog
	|   │   │   └── tex
    │   │   ├── cat
    │   │   └── ..
    │   ├── env
    │   │   ├── barn
    │   │   ├── rocks
    │   │   ├── trees
    │   │   └── ...
    │   └── fx
    ├── scenes
    │   ├── 000_titles
    │   └── 001_intro
    │       ├── 010_0010
    │       │   ├── 010_0010-layout-anim.blend
    │       │   ├── 010_0010-lighting.blend
    │       │   ├── 010_0010-sim.blend
    |       │   └── 010_0010-comp.blend
    │       └── 010_0020
    │           ├── 010_0020-anim.blend
    │           └── ...
    ├── edit
    └── .blender_project
```

## Naming Conventions

Highly recommend reading [blender's naming conventions](https://studio.blender.org/tools/naming-conventions/datablock-names).

### Assets
```plaintext
bark_oak_normal.png
bark_oak_albedo.png
bark_birch_normal.png
```

### Shots
```plaintext
010_110-anim.blend
010_110-compositing.blend
```

## Collaboration Workflow

- `Not Ready` -> `Todo` -> `Work in Progress` -> `Waiting for Approval`
	-  -> `Done`
	- -> `Retake`
	-  -> `Could Be Better` 

### Task Statuses
- **Not Ready (NR):** Default status. Task is blocked.
- **Todo:** Ready to do work.
- **Work in Progress (WIP):** Work has started / ongoing.
- **Waiting for Approval (WFA):** Asking for feedback.
	- Should also attach a screenshot or an animation playblast
- **Done:** Approved / Task is finished.
- **Could Be Better (CBB):** In case we don't have time for **RTK**.
- **Retake (RTK):** Not approved + feedback.

### Asset Tasks
- **Concept:** Gather reference for the asset.
- **Modeling:** Model the asset in blender.
- **Texturing:** Create required textures in image editing software or find a suitable texture online.
- **Rigging (Characters only):**
- **Animation**

### Shots / Sequence Tasks
- **Storyboard:** Discuss how the scene / shot is going to be.
- **Layout:** Construct the scene. Merge created assets in one scene.
- **Animation:** Create shot specific animations that can't be created separately.
- **Lighting:** Light pass.
- **FX:** Create necessary visual effects.
- **Compositing:** Color correction / other effects.

## References

https://studio.blender.org/tools/naming-conventions/file-types
https://studio.blender.org/tools/naming-conventions/datablock-names
https://studio.blender.org/tools/naming-conventions/examples
https://docs.blender.org/manual/en/latest/files/linked_libraries/link_append.html
https://www.youtube.com/watch?v=aR3yNNGK_sc
