# Example Data Packages

[![goodtables.io](https://goodtables.io/badge/github/frictionlessdata/example-data-packages.svg)](https://goodtables.io/github/frictionlessdata/example-data-packages)


This repository contains example data packages to help you learn about [Frictionless Data](https://frictionlessdata.io/). The example data packages:

- illustrate the current Frictionless Data [Specification](https://frictionlessdata.io/specs/)
- support the Frictionless Data [Guides](https://frictionlessdata.io/guides/)
- demonstrate Frictionless Data [Patterns](https://frictionlessdata.io/specs/patterns/) - ways to solve common problems that are not (yet) in the specification

The Guides are a great place to [start to learn](https://frictionlessdata.io/guides/). Alternatively, dive in and open a data package directory, view the `README.md`, then view the `datapackage.json` to understand the data.

*Warning: some data packages are out-of-date. (See [Issue #4](https://github.com/frictionlessdata/example-data-packages/issues/4))*

## Data Packages

The `datapackage.json` will describe the [data package](https://frictionlessdata.io/specs/data-package/) as a whole, and one or more [data resources](https://frictionlessdata.io/specs/data-resource/) (each optionally with a [schema](https://frictionlessdata.io/specs/data-resource/#resource-schemas) or a [view](https://frictionlessdata.io/specs/views/)).

If all the data is tabular (i.e. [CSV files](https://frictionlessdata.io/guides/csv/)), then it will be described as a [tabular data package](https://frictionlessdata.io/specs/tabular-data-package/) with one or more [tabular data resources](https://frictionlessdata.io/specs/tabular-data-package/) each with a [table schema](https://frictionlessdata.io/specs/table-schema/) and, if needed, a [CSV dialect](https://frictionlessdata.io/specs/csv-dialect/).

There are other specialised [profiles](https://frictionlessdata.io/specs/profiles/) that describe different types of data, such as [fiscal data](https://frictionlessdata.io/specs/fiscal-data-package/).

Each data package is stored in it's own directory:

```
|- data-package-name-1
   |- README.md
   |- datapackage.json
   |- data
      |- data.csv
      |- ...
```

It contains a:

- `README.md` to explain the provenance of the data
- `datapackage.json` a machine readable file that explains the structure and meaning of the data
- one or more data files, typically grouped in a `data` directory

The data package directory may also contain [other files or sub-directories](https://frictionlessdata.io/specs/data-package/#illustrative-structure). These files may be scripts used to prepare the data package or other related resources.

## Validation

With each commit to the repository, the data package is validated using [goodtables.io](http://goodtables.io/). The validation results for the whole repository are indicated with a badge: [![goodtables.io](https://goodtables.io/badge/github/frictionlessdata/example-data-packages.svg)](https://goodtables.io/github/frictionlessdata/example-data-packages)


*Ideally an individual badge could also be awarded for each data package and displayed in its `README.md` file but this is not possible yet. (See goodtables.io [issue #285](https://github.com/frictionlessdata/goodtables.io/issues/285))*

The validation is controlled by the [goodtables.yaml](https://github.com/frictionlessdata/example-data-packages/blob/master/goodtables.yml) file. It should be configured to test all the data packages in the repository. This can be changed if your working locally to [validate specific data packages](https://github.com/frictionlessdata/goodtables.io/blob/master/docs/goodtables_yml.md).

## Zipped Data Packages

With each commit to the repository, the data package directory is converted into a .zip file so it can be used with [software that supports Frictionless Data ](https://frictionlessdata.io/software/) such as the [Data Curator](http://data-curator.io) app or the [DataPackage.js](https://github.com/frictionlessdata/datapackage-js) library. The zip files are stored in the `zip` directory.

*To do: script needed*

## Formatted JSON

With each commit, the `datapackage.json` file is [formatted to make it easier to read](https://frictionlessdata.io/guides/publish-faq/#alignment). Although this formatting is not needed by computer programs, it makes it easier for you to read the contents of the file.

*To do: script (or linting) needed*

## Resources

A resources directory contains a template `README.md` and example `datapackage.json` snippets.

### `README.md` template

In this repository, each data package must have a `README.md`. The `README.md` should follow [good practices](https://frictionlessdata.io/guides/publish-faq/#readme).

### `datapackage.json` snippets

JSON snippets provide a fragment of a `datapackage.json` file to help you learn about that specific property or cut and paste into your own data package. E.g. `licenses.json` could include JSON for each [recommended Open Definition conformant license](http://opendefinition.org/licenses/#conformant-licenses).

## Repository Structure

```
|
|- data-package-name-1
|  |- README.md
|   |- datapackage.json
|   |- data
|     |- data.csv
|     |- data.geojson
|     |- ...
|     
|- data-package-name-2
|  |- etc.
|
|- resources
|  |- README-template.md
|  |- licenses.json
|  |- contributors.json
|  |- dialect.json
|  |- ...
|
|- zip
|  |- data-package-name-1.zip
|  |- data-package-name-2.zip
|
|
|- goodtables.yaml
|- README.md   

```

## Contributing

We value all types of contributions:
- documentation
- data packages
- [issues](https://github.com/frictionlessdata/example-data-packages/issues) and [requests](https://github.com/frictionlessdata/example-data-packages/issues)
- code

We thank the generous [contributors](https://github.com/frictionlessdata/example-data-packages/graphs/contributors) to this project.

To join them, please read [`CONTRIBUTING.md`](.github/CONTRIBUTING.md) for details on our code of conduct and how to submit a pull request. Each contributed data package should be licensed as openly as possible.

## Licenses

Data Packages in this project are licensed as specified in each individual `datapackage.json` file.  If a license is not specified, it is provided under a [CC0 1.0 Universal](https://creativecommons.org/publicdomain/zero/1.0/) Public Domain Dedication.

The code in this project, unless otherwise noted, is licensed  as described in [`LICENSE.md`](LICENSE.md).
