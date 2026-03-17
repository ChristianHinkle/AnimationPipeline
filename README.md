# MediaProductionPipeline

Documentation and diagrams for creating a workflow to produce media such as 2D/3D video animations.

Note: Any tools we end up writing for this are planned to be developed in separate repositories. We will link to them in this documentation when they become available.

The original motivation for this pipeline was to produce 2D/3D animations, but since it's so cross-disciplinary, I plan to generalize these workflows for many purposes.

This workflow should be able to produce 2D animations (like anime), 3D animations (like pre-rendered video game cutscenes), and both at the same time (e.g., 3D backgrounds for anime, or 2D visual effects in the Spider-Verse movie). I think we could even combine this into being a general video-editing and CG/VFX workflow as well for live-action content.

The timesheet-based animation workflow is tailored to the Japanese anime industry's production pipeline. But I try to unify the terminology and give analogies for Western terms.

The 3D aspect of this is planned to be used for rendering animations of 3D characters. Namely, characters from our games, so we can post fun video animations of them as another form of content and branding/marketing. We also want this to be a common pipeline for producing actual in-game cutscenes.

Another possible use for this pipeline is to render still images as artwork and brand content. E.g., some video game covers are extremely complex (like Mario Kart World). Even though they are just single images, they use the 3D models, pose the models, add custom VFX (3D and 2D), overlay the game title, etc. Basically, they should be able to do anything to get a really good final artwork.

## Software

So far, all diagrams are completely generic to software choice, but here are the tools we plan to use.

All software of interest (not all are incorporated in the workflow):
- Blender
- Open 3D Engine (O3DE)
- Clip Studio
- `.xdts` file format
- `.tdts` file format
- Toei Animation Digital Exposure Sheet
- OpenToonz
- Krita
- Meddy
- Git
- A version control solution for large binary assets
- fSpy

### Storyboarding Software: TBD

### 2D Illustration (e.g., Background Art) Software: Anything

Any software is fine. 2D illustrations that are not used as animation cels have way more freedom as to how they are authored. It could even be hand-painted and scanned.

I decide to use Clip Studio.

### Layout, Keyframe, and Inbetween 2D Animation Software: Clip Studio

Although ideally not actually required. I feel we should be able to use any illustration software for this step and rely on the compositing step to achieve anything we want in there. At the end of the day, all that matters is that we have the finished cels to send to the compositing team. Clip Studio just happens to have really good animation previewing tools.

### Digital Timesheet File Format: `.tdts`

Toei's file format is not completely necessary. We could just use `.xdts` for the minimal timing data if desired.

### Digital Timesheet Syncing Tool: Toei Animation Digital Exposure Sheet

Or custom scripts for syncing timesheet files to non-Clip-Studio software.

We will need a way to sync timesheet information to the compositing software of choice. Toei's program has tools for After Effects.

### Animation Compositing Software: Blender

Blender's Video Sequence Editor for animating cels, implementing anime camera work, and VFX.

### Video Editing Software: Blender

Blender's Video Sequence Editor for combining all the cuts and audio, and rendering the final output artifact to go out for delivery.

### 3D Modeling: Blender

### 3D Hi-Res Sculpting: Blender

Maybe there's a better alternative, though.

### 3D Texture Painting: Blender

Maybe there's a better alternative, though.

### 3D Animation: Blender
