This extension links some [JSONSchemas](http://json-schema.org) to [Loopback](https://docs.strongloop.com/display/APIC/Using+LoopBack+with+IBM+API+Connect) configuration files.

:information_source: Schemas used by this plugin can be found [here](https://github.com/Sequoia/loopback-json-schemas). **Please do not file schema bugs on this repo!!** This repo is just for the plugin. :smile_cat: File schema bugs [here](https://github.com/Sequoia/loopback-json-schemas).

# Currently implemented schemas

1. `model-config.json`
1. `model-config.json`
1. `datasources.json`
1. `config.json`
1. `middleware.json`
2. Model definitions (`/common/models/customer.json` etc.)

Check the [package.json.contibutes.jsonValidation](https://github.com/Sequoia/loopback-json-schemas-vscode/blob/master/package.json#L22) for the actual configurations.

# Gifs!

## Code hints
The plugin prompts you as you type

![demo of code hinting](hints.gif)

## Green Squiggles
If you have a mismatched type or missing property, you'll get a green squiggle underline

![demo of green squiggles on problems](green-squiggles.gif)

## `Ctrl+Space`
Hit `ctrl+space` to be shown available properties

![ctrl+space demo](ctrl-space.gif)

It also works for enum types

![ctrl+space demo for enumerated type](ctrl-space-type.gif)

## Links
You can click links to read extended documentation

![clicking links from tooltip](links.gif)
