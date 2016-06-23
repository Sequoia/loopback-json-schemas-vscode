This extension links some [JSONSchemas](http://json-schema.org) to [Loopback](https://docs.strongloop.com/display/APIC/Using+LoopBack+with+IBM+API+Connect) configuration files.

**THIS IS AN INCOMPLETE BETA RELEASE**. Given the nature of loopback, schemas may never be 100% complete. Schemas used by this plugin can be found [here](https://github.com/Sequoia/loopback-json-schemas).

# Currently implemented schemas
1. `model-config.json`
2. Model definitions (`/common/models/customer.json` etc.)

Lots to-do!

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
