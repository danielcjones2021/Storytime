Perfect! Here's the updated README and the commands:

# Storytime

**A fork of Storyboarder with AI-powered image generation built in.**

Storytime takes the fast, simple storyboarding of Wonderunit's Storyboarder and adds integrated AI image generation. Sketch your idea with stick figures, hit 'g', and generate a stylized image from your sketch. The fastest path from rough idea to polished animatic.

[![screenshot](https://user-images.githubusercontent.com/441117/27712058-4404e214-5cf3-11e7-8fa3-b88ae924d154.gif)](https://www.wonderunit.com/storyboarder)

## What's New in Storytime

**AI Generation Integration**
- Sketch rough ideas, generate reference images instantly
- Integrated ComfyUI support for local generation
- ControlNet-powered sketch-to-image workflow
- Hit `g` to generate, results import automatically
- Style prompts that carry across frames for consistency

**The Workflow:**
1. Rough sketch with stick figures
2. Press `g`, add a prompt ("cowboy on horseback in desert")
3. AI generates photorealistic reference from your sketch
4. Result imports as reference layer
5. Continue boarding with proper lighting/composition reference

No context switching. No export/import dance. Sketch → Generate → Polish.

## Download

This is a development fork. To use:
1. Clone this repo
2. `npm install` (requires Node 16)
3. `npm start`

For ComfyUI integration:
- Install [ComfyUI](https://github.com/comfyanonymous/ComfyUI)
- Run ComfyUI on port 8000
- Load the included workflow from `/ComfyUI-workflow/`

[Submit issues, bugs, ideas, suggestions here](https://github.com/danielcjones2021/storytime/issues)

## It's Still Easy...

1. Start a blank storyboard or open a Fountain screenplay
2. Draw boards with mouse, Wacom, or any pen tablet
3. Hit `g` to generate AI references from your sketches
4. Flip through boards, play it back, pitch it, iterate

The original Storyboarder philosophy: don't get slowed down by complexity. You're here to tell stories fast.

## Features:

**Original Storyboarder Features:**
* Simple, Smooth Drawing
* Super Simple Interface
* Printed Worksheets
* Works with Wacom
* Easy Organization
* Draw Straight Lines
* Works with Fountain
* Open in Photoshop
* Measure Line Mileage
* Guides to Help Drawing
* Reference Layer
* Onion Skin
* Track Changes
* Export to Various Formats

**New AI Features:**
* **Integrated AI Generation** - ComfyUI integration built in
* **Sketch-to-Image** - ControlNet converts rough sketches to references
* **Style Consistency** - Persistent style prompts across frames
* **Hotkey Generation** - Press `g` for instant generation
* **Local & Remote** - Supports both local ComfyUI and remote APIs
* **Async Generation** - Keep boarding while images generate

## Brushes (Same as Original):

* **Light pencil** for roughing
* **Pencil** for fast sketching
* **Pen** for inking strong lines
* **Brush** for filling and shading

No layers. No complexity. Board fast, generate references when needed, keep moving.

## Key Commands:

* Light Pencil: <kbd>1</kbd>
* Pencil: <kbd>2</kbd>
* Pen: <kbd>3</kbd>
* Brush: <kbd>4</kbd>
* Eraser: <kbd>5</kbd>
* **AI Generate: <kbd>g</kbd>** ← NEW
* Clear: <kbd>Delete</kbd> or <kbd>Backspace</kbd>
* Undo: <kbd>Cmd</kbd>+<kbd>z</kbd>
* Redo: <kbd>Cmd</kbd>+<kbd>y</kbd>
* Smaller Brush: <kbd>[</kbd>
* Bigger Brush: <kbd>]</kbd>
* Straight Lines: <kbd>Hold Shift</kbd>
* Move Contents: <kbd>Hold Cmd</kbd>
* Scale Contents: <kbd>Cmd</kbd>+<kbd>Option</kbd>

## Development Roadmap

**Current:** ComfyUI integration, basic sketch-to-image generation
**Next:**
- Additional AI backends (Replicate, Stability AI)
- Shot matching for style consistency
- Batch generation across multiple boards
- Improved pressure sensitivity (Wacom compatibility)

## About This Fork

Storytime is built on [Storyboarder by Wonderunit](https://github.com/wonderunit/storyboarder). The goal is to create the fastest possible workflow for modern storyboarding by integrating AI tools directly into the drawing interface. No switching apps, no manual import/export, no workflow interruption.

If you want stable, production-ready software, use the original Storyboarder. If you want cutting edge integration and don't mind experimental builds, this is for you.

## Credits

Original Storyboarder: [Wonderunit](https://wonderunit.com/storyboarder/)
AI Integration: Dan Jones

## License

See original Storyboarder license: https://wonderunit.com/thoughts-on-free-and-open-source/

---

**Commands to rename everything:**

```bash
# 1. First, rename on GitHub:
# Go to https://github.com/danielcjones2021/scribbler/settings
# Change "Repository name" to "storytime"
# Click "Rename"

# 2. Update local git remote (run this after GitHub rename):
git remote set-url origin https://github.com/danielcjones2021/storytime.git

# 3. Rename your local folder in File Explorer:
# Desktop\Scribbler → Desktop\Storytime

# 4. Update package.json - change the "name" field to:
"name": "storytime",
```

Start with step 1 on GitHub, then run the git command!
