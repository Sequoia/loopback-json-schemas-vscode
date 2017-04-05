# Contributing

**If you want to correct or augment an existing schema, you don't need to modify this plugin!** The schemas themselves are in https://github.com/Sequoia/loopback-json-schemas, and this is the place to fix a schema bug or omission.

For fixing **schemas only**, the easiest way is to **not** use this plugin (disable if it's installed), but to serve the schemas locally & point to them on a per-file basis (see instructions [here](https://github.com/Sequoia/loopback-json-schemas/blob/master/CONTRIBUTING.md#2-working-on-schemas)).

The process for working on this and testing it locally is, roughly:

0. Disable this plugin if you have it already installed in your VS Code
1. Clone the [**schemas**](https://github.com/Sequoia/loopback-json-schemas) repo
2. Follow [the instructions in that repository](https://github.com/Sequoia/loopback-json-schemas/blob/master/CONTRIBUTING.md) for serving schemas locally
3. Clone this **plugin** repo
4. `npm install` this project
5. Open this project in VS Code
6. **Edit the package.json on this project to `http://localhost:8090/` for the schema you wish to work on.** This isn't a very graceful solution but I haven't figured out a better one.
7. Run the "launch extension" debug configuration
8. In the `[Extension Development Host]` window, open a LoopBack project for testing
9. Before pushing your changes for *this* repo, **edit the package.json to point back to `https://raw.githubusercontent.com/Sequoia/loopback-json-schemas/master/dist/`**.
10. Before pushing changes for the **schemas** repo, run `npm run build` on it.

If you wish to add a *whole new schema* that this plugin doesn't currently support, you'd need to:

1. Create the schema in *that* repository
2. Add a new entry to [`package.json.contribues.jsonValidation`](https://code.visualstudio.com/docs/extensionAPI/extension-points#_contributesjsonvalidation) for *this* repository points to your new schema (locally).
3. Be sure to follow the "replace localhost links with `raw.githubusercontent.com` upon publishing.

For information on setting up, debugging, and building VSCode plugins generally, please consult the [VS Code guide](https://code.visualstudio.com/docs/extensions/overview) on this subject.