# Area Blocks

Area Blocks is a lightweight browser-based tool for quickly visualising programme areas as proportional 1 m² grid blocks.

![Area Blocks interface](assets/area-blocks-demo.jpg)

## Features

- Add, rename, recolour and remove programme areas
- Enter areas in m²
- Automatically generate proportional block shapes
- Shuffle layouts and colours
- Multiple built-in colour palettes
- Optional grid and room labels
- Light and dark modes
- Adjustable display scale and spacing
- Automatic local session saving
- Save and load projects as JSON
- Import programme data from CSV or pasted spreadsheet rows
- Export layouts and individual rooms as SVG or JPG

## Usage

Open `index.html` in a modern web browser. No installation or server is required.

Add rooms and enter their required areas. Use **Shuffle layout + shapes** to explore different arrangements and **Shuffle colours** or the palette selector to adjust the graphic appearance.

### Saving and Loading

The app automatically saves your current state using your browser's local storage.

This autosaved state is **local to your browser**. It is not uploaded to GitHub, shared with other users, or synchronised between browsers or devices. Each person opening the GitHub Pages site therefore has their own independent saved state.

Refreshing or reopening the page in the same browser will restore your previous session.

For project management:

- **Save State** — downloads the current project as a `.json` file
- **Load State** — restores a previously saved `.json` file
- **Clear** — removes all current programme entries

JSON state files can be transferred between browsers, devices, or users, making it easy to share programme configurations, colour schemes, layout settings, and other project options.

### Importing Data

Programme entries can also be imported using **Import CSV** or **Paste spreadsheet data**. Rows should contain the room name, area, and optionally a `#RRGGBB` colour value, with no header row.

If entries already exist, the app asks whether to replace them. Choose **OK** to replace the existing entries, or **Cancel** to keep them and append the imported entries.

### Exporting

The app provides four export options:

- **Export current layout SVG** — exports the complete arrangement as a single `.svg` file
- **Export separate SVGs** — exports every programme area as an individual `.svg` file, packaged together in a `.zip` archive
- **Export current layout JPG** — exports the complete arrangement as a single `.jpg` file
- **Export separate JPGs** — exports every programme area as an individual `.jpg` file, packaged together in a `.zip` archive

The **Include grid** and **Include text** options control whether the grid and room labels are included in exported files.

SVG provides editable vector output suitable for further graphic editing, while JPG provides a standard raster image suitable for presentations, documents, and quick sharing.

## Units

**1 grid cell = 1 m²**

The display cell size only changes the visual scale of the diagram; it does not change the represented areas.