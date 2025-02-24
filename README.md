# MHW-Loadouter

A small armor assembly tool for the game Monster Hunter World written to be statically served.

The project is available on my [Github Pages](https://www.statdk.com/MHW-Loadouter), but is able to be hosted locally (or anywhere else you can serve http requests).

# Features

- Searching for equipment by name, rank, and slot
- Saving and deleting custom equipment sets
- Display of individual equipment defensive stats and calculation of total stats
- Calculation of total required crafting materials

# How to use

## Using the tool

### Modifying an armor set

1. Select the armor slot you wish to modify on the left hand side (top for mobile users).
2. Optionally, enter the name and/or rarity of your desired replacement equipment in the search box located in the center of the screen (below the slots for mobile users).
3. Select a peice of equipment to replace the current slot.
4. The page will update to reflect your changes, with new stats on the right hand side of the screen.

### Save/Load/Delete a set

To save a set, simply enter a name for it at the top of the screen and click save.

To load or delete a set, select it from the drop down menu and click on your desired operation.

## Running Locally

Depending on your browser, you may be able to simply download the project source and open `index.html` with your file manager.

Many browsers, however, will deny the page access to the other javascript files in the project. To get around this, the project possesses a simple npm project to serve the page with the http-server package.

### Serving the page locally

#### Prerequisites

- npm
- git (optional)

#### CLI Commands

```bash
# Optionally, download the repository via git
git clone https://github.com/Statdk/MHW-Loadouter.git

# Navigate into the project root
cd MHW-Loader

# Install Dependancies
npm clean-install

# Run http-server on the current directory
npm run serve
```

Press Ctrl+C to terminate the server.

By default, the server is hosted on http://127.0.0.1:3000/, but the port can be customized to any of your choosing by editing the port argument in the `package.json` file.

## Current Limitations

- No selectable armor decorations
- No armor levels
- No inclusion of weapons as a slot
