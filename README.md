# GUIMolEditor
Molecule Editor GUI using RDKit
![rdeditor, the RDKit molecule editor](./Screenshots/Main_window.png)

## Installation
* requirements

RDKIT and PySide2

* installation
```bash
python setup.py install

```

The install script Will also install PySide2, but not RDkit, so that should be installed manually or via your operating systems package manager. A launch script will also be added so that it can be started from the command line via the rdEditor command.

## Alternative install
Install PySide and RDKit yourself, save the content of rdeditor folder to somewhere you like and start it with 
`python rdEditor.py`

## Usage

Can be started with `rdEditor` or `rdEditor your_molecule.mol` to start edit an existing molecule.
Interactions with the molecule are done via clicking on the canvas, atoms or bonds. A choice of tools is available.

From left to right
* Open: Open a molfile
* Save: Save current molecule
* Save As: Save current molecule with a new name
* Arrow: Select tool. Click on an atom to select it, click on the canvas to deselect. Clicking on multiple atoms one after another will select them, but only the lastly clicked one will be highlighted in red and used for operations, such as bond creation to another existing atom.
* Add bond / Join atoms: Will add a single bond between a clicked atom (or a previously selected atom) and the next atom clicked.
* Increase/Decrease charge: Will increase or decrease the charge of the atom clicked
* Delete atom/bond: 
* Clear Canvas
* Undo.

