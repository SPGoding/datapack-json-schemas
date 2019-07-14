# datapack-json-schemas

[![CircleCI](https://img.shields.io/circleci/build/github/SPGoding/datapack-json-schemas.svg?logo=circleci&style=flat-square)](https://circleci.com/gh/SPGoding/datapack-json-schemas)
[![npm](https://img.shields.io/npm/v/datapack-json-schemas.svg?logo=npm&style=flat-square)](https://npmjs.com/package/datapack-json-schemas)
[![License](https://img.shields.io/badge/License-CC%20BY%204.0-blue.svg?style=flat-square)](https://creativecommons.org/licenses/by/4.0/)
[![semantic-release](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--release-e10079.svg?style=flat-square)](https://github.com/semantic-release/semantic-release)
[![Gitmoji](https://img.shields.io/badge/gitmoji-%20😜%20😍-FFDD67.svg?style=flat-square)](https://gitmoji.carloscuesta.me/)

Update to: Minecraft Java Edition 1.14.4-pre5

JSON schemas for Minecraft: Java Edition datapack JSON files. Information about json schemas can be found at [json-schema.org](http://json-schema.org/).

You can see [vscode-datapack-helper-plus-json](https://github.com/SPGoding/vscode-datapack-helper-plus-json) for a use if you are using [VSCode](https://code.visualstudio.com/).

## Design choices

-   The use of the `minecraft:` namespace is mandatory anywhere it can be used.
    This does mean that it will not necessarily validate against all vanilla
    files

## File Struture

- `src`: Stores all JSON Schemas.
    - `shared`: Stores all common JSON Schemas. Should be generated by `./scripts/convert.js` so you don't change it manually.
    - `tags`: Stores JSON Schemas for [tags](https://minecraft.gamepedia.com/Tag).
    - `advancement.json`: JSON Schema for [advancements](https://minecraft.gamepedia.com/Advancements).
    - `loot_table.json`: JSON Schema for [loot tables](https://minecraft.gamepedia.com/Loot_table).
    - `pack.mcmeta.json`: JSON Schema for [`pack.mcmeta`](https://minecraft.gamepedia.com/Data_pack#pack.mcmeta).
    - `recipe.json`: JSON Schema for [recipes](https://minecraft.gamepedia.com/Recipe).
- `scripts`: Stores useful tools.
    - `convert.js`: Convert `registries.json` generated by Minecraft data generator to `shared` files

## License

<a rel="license" href="http://creativecommons.org/licenses/by/4.0/"><img alt="Creative Commons Licence" style="border-width:0" src="https://i.creativecommons.org/l/by/4.0/88x31.png" /></a><br />This
work is licensed under a
<a rel="license" href="http://creativecommons.org/licenses/by/4.0/">Creative
Commons Attribution 4.0 International License</a>.

This work is based on [SPGoding/datapack-json-schemass](https://github.com/SPGoding/datapack-json-schemass) created by [@Levertion](https://github.com/Levertion) which is released under a [CC BY 4.0 license](https://creativecommons.org/licenses/by/4.0/). I keep it updated with Minecraft.

## Contributing

Contributions are welcome!
