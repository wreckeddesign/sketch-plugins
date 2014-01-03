# Sketch Symbols

Sketch Symbols is a plug-in for Sketch (http://bohemiancoding.com/sketch/) that lets you mimic basic Smart Objects / Symbols functionality by automatically syncing changes between layer groups named in a particular way. As an added bonus, you can mark certain text layers in your symbols as dynamic and have their styles replicated, but not their content.

## Installation

1. Download the plugin.
2. Double-click the `.sketchplugin` file. Sketch should open
   automatically and tell you that a new plugin was installed.

## Usage

1. Create a layer group for your symbol. (`Cmd + G`)
2. Add ": symbol-name" to its name to mark it as a symbol. E.g.: "signup
   button : button-default".
3. Use a copy of the same symbol in other parts of your document. You
   can change the name before the colon to whatever you like.
E.g.: "signin button : button-default".
4. Make changes to any of the copies of the symbol you've created. Press
   `Cmd + E` to sync these changes with other instances of the same
symbol.

## Dynamic Text Layers

Put a `$` in front of the name of any text layer inside a symbol to mark
it as dynamic. When you sync changes between symbols, dynamic text layers will
not be replaced. Their styles, including font size, family and line height will be updated, but their content will remain
intact. This lets you define a single symbol for a button, for example, but use
different copy for each instance of that button.

## Changing the Default Keyboard Shortcut

1. Open Sketch's plugins folder. You can do that easily by choosing
   Custom Script from the Plugins menu, then click the gear icon and
choose "Open Plugins Folder".
2. Open the file "Sync Symbols.sketchplugin" in your favorite text
   editor.
3. The shortcut is on the first line:

  // Syncs all instances of a symbol tagged with ": symbol-name" **(cmd e)**

  Change it to whatever you like (ctrl shift s, for example), and you
should be good to go. The following modifiers are all valid: `control ctrl alt option cmd command shift`.

## Thanks

Bohemian Coding for creating Sketch in the first place and @bomberstudios for their wonderful sketch-commands bundle (https://github.com/bomberstudios/sketch-commands), which proved a wonderful source for learning and inspiration.

## License

The MIT License (MIT)

Copyright (c) 2013 Tisho Georgiev

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.