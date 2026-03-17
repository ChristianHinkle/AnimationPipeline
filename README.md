# MediaProductionPipeline

Documentation, diagrams, and potentially even tools (although, those tools would likely call for separate repositories) to creating a workflow for making 2D/3D video animations.

This was originally designed for animation pipelines but the workflows will end up becoming generalized for many purposes.

This workflow should be able to produce 2D animations (like anime), 3D animations (like pre-rendered video game cutscenes), and both at the same time (e.g., 3D backgrounds for anime, or 2D visual effects in the Spider-Verse movie). I think we could even combine this into being a general video-editing and CG/VFX workflow as well for live-action content.

The 2D aspect of this is planned to be tailored to the Japanese anime industry's production pipeline. E.g., making use of timesheets.

The 3D aspect of this is planned to used for rendering animations of 3D characters. Namely, characters from our games so we can post fun video animations of them as another form of content and branding/marketing.

This could also be useful for rendering still images as artwork and brand content.

## Software

Here are the software tools we plan to use.

All software of interest:
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

Any software is fine. 2D illustrations not used as animation cels have way more freedom on how they are authored. It could even be hand-painted and scanned.

I decide to use Clip Studio.

### Layout, Keyframe, and Inbetween 2D Animation Software: Clip Studio

Although, ideally not actually required. I feel we should be able to use any illustration software for this step and rely on the compositing step to achieve anything we want in there. At the end of the day, all that matters is that we have the finished cels to send to the compositing team. Clip Studio just happens to have really good animation previewing tools.

### Digital Timesheet File Format: `.tdts`

Toei's file format is not completely necessary, we could just use `.xdts` for the minimal timing data if desired.

### Digital Timesheet Syncing Tool: Toei Animation Digital Exposure Sheet

Or custom scripts for syncing timesheet files to non-Clip-Studio software.

We will need a way to sync timesheet information to the compositing software of choice. Toei's program has tools for After Effects.

### 2D Animation Compositing Software: Blender

Blender's Video Sequence Editor for animating cels, implementing anime camera work, and VFX.

### Video Editing Software: Blender

Blender's Video Sequence Editor for combining all the cuts and audio, and rendering the final output artifact to go out for delivery.
