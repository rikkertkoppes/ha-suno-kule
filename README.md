# Suno Kule Home Assistant Add-on

Suno Kule is a visual shader-style editor for animated LED setups.

It lets you:

- define one or more LED fixtures (for example WLED devices)
- build animation logic as a node graph (the shader graph)
- run those animations live from Home Assistant

## Quick Install Button

Use this button to open the App Repository dialog in Home Assistant with the Suno Kule repository URL prefilled:

[![Open your Home Assistant instance and add this repository.](https://my.home-assistant.io/badges/supervisor_add_addon_repository.svg)](https://my.home-assistant.io/redirect/supervisor_add_addon_repository/?repository_url=https%3A%2F%2Fgithub.com%2Frikkertkoppes%2Fha-suno-kule)

If this does not work in your setup, follow the manual steps below.

## Install In Home Assistant

### 1. Add this repository

1. In Home Assistant, open **Settings** -> **Add-ons**.
2. Open the **Add-on Store**.
3. Open the menu (top-right) and choose **Repositories**.
4. Add this repository URL:

    `https://github.com/rikkertkoppes/ha-suno-kule`

5. Confirm and close the repository dialog.

### 2. Install the Suno Kule add-on

1. Search for **Suno Kule** in the Add-on Store.
2. Open it and click **Install**.
3. (Optional) Configure add-on options.
4. Click **Start**.
5. If you want quick access, enable **Show in sidebar**.

## First Run Setup

After installation:

1. Open Suno Kule from the sidebar.
2. Add at least one fixture (your LED output target).
3. Create or open a shader graph.
4. Press run/start in the app to stream output.

## Core Concepts

### Fixtures

A fixture is an LED output target that Suno Kule can render to.

In practice, a fixture usually maps to a physical device (for example a WLED controller/strip), plus its layout information such as pixel count and arrangement.

Think of fixtures as the "where" of your visuals.

### Shader Graph

The shader graph is the node-based program that generates your animation.

- Nodes create and transform values over time.
- You connect nodes to build behavior.
- The final output drives color/brightness for the selected fixtures.

Think of the shader graph as the "how" of your visuals.

## Tips

- Start with one fixture and a simple graph before scaling up.
- Save working graphs often.
- Add complexity in small steps: timing, color, then modulation/effects.

## Support

Project repository:

`https://github.com/rikkertkoppes/ha-suno-kule`
