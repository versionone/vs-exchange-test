# vs-exchange
A place to exchange VersionOne VS automation and other system customizations.

## What should an item that I want to add to the exchange contain?
An exchange item should include three things:
1. a `README.md` file to explain what the item is and how it is used,
2. a `src/` directory containing the Continuum assets as json. It can contain one or more of the following:
    1. a `catalog/` directory that matches the directory structure from the `ctm-export-catalog` command. It can contain any of the types exported by that command (packages, pipelines, projects, tasks)
    2. a `canvas/` directory that matches the directory structure of the ctm-export-canvas command. I can contain any number of canvas items.
    3. a file named `registry` that contains a global registry document as json.
3. a `.tgz` file that is the result of `tar -czf {tar name} src/`
