# multi-sass

Compile multiple sass projects using a single node-sass instance.

## Installation

```shell
npm install -g multi-sass
```

## Usage

Supply any combination of `node-sass` command line options, separating each configuration by `-n` or `--next`.

**Example:**

```shell
multi-sass --directory project1/src --output project1/css --source-map
    --next --file project2/src/component.scss -o project2/dist/comp.min.css
```

**Options:**

All [command-line options available to node-sass](https://www.npmjs.com/package/node-sass#command-line-interface) should work, as should [any option specified in the documentation](https://github.com/sass/node-sass#options) prefixed with `--`.

The flags defined by `multi-sass` either exist because they are named differently or because that part of the functionality is provided by `multi-sass` (such as `--watch`).

```shell
-h, --help             output usage information
-V, --version          output the version number
--name <name>          Name config
-n, --next             Start next config
-w, --watch            Enable watch
-i, --input <file>     Input file
-d, --directory <dir>  Input directory
-r, --recursive        Recursively watch directories or files
-o, --output <file>    Output file or directory
--include-path <dir>   Path to look for imported files
```

## Contributing

If you have some issue or code you would like to add, feel free to open a Pull Request or Issue and I will look into it as soon as I can.

## License

I am releasing this under a MIT License.

## About me

Find me on [GitHub](https://github.com/JorgenEvens) or [Twitter](https://twitter.com/JorgenEvens).
