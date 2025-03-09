# i18n support for Nvim

This plugins provides a simply way to go to definition for strings in your codebase, looking for definitions in various translation json files.

## Configuration

To set up the plugin, supply a list of language configurations (filePath, keymap) to the setup function like so:
```lua
require('i18n').setup({
  {
    filePath = 'path/to/your/translations.json',
    keymap = 'your-keymap'
  },
  {
    filePath = 'path/to/your/other-translations.json',
    keymap = 'your-other-keymap'
  }
})
```

With this setup, you can put your cursor at a string in your codebase, and press they keymap you've set up (per language) to jump to the definition of that string in that translation file. 
