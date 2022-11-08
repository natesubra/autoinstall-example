# VSCode AutoInstall Schema Validation

See [settings.json](.vscode/settings.json)

Essentially, the schema is available [here](https://raw.githubusercontent.com/canonical/subiquity/main/autoinstall-schema.json)

Example of adding a schema config is [here](https://dev.to/brpaz/how-to-create-your-own-auto-completion-for-json-and-yaml-files-on-vs-code-with-the-help-of-json-schema-k1i)

Lots of examples [here](https://github.com/canonical/subiquity/tree/22.10.1/examples)

This is a working [template](https://raw.githubusercontent.com/canonical/subiquity/22.10.1/examples/autoinstall.yaml)

I've included a local copy [here](autoinstall.yml) that works

Note that they wrap the hash in `'`

Also, the installer version can change, might not be a bad idea to keep this in your yml, to make sure you're getting the latest stable installer. Schemas can change between versions:

```yml
refresh-installer:
    update: true
```
