# textpattern-curated-themes-list

[![Build Status](https://travis-ci.com/textpattern/textpattern-curated-themes-list.svg?branch=master)](https://travis-ci.com/textpattern/textpattern-curated-themes-list)

A curated list of [Textpattern CMS](https://textpattern.com) themes listed in the [Textpattern themes website](https://github.com/textpattern/textpattern-themes-website).

## JSON structure

Each theme has a JSON-formatted 'library card', located within the `library-of-themes` directory of this repository.

The Textpattern themes website digests the information for each card to provide the relevant details of the theme. Each card expects a set of [required entries](#required-entries) plus any [optional entries](#optional-entries) as appropriate. **It is recommended** that you complete as many fields as possible in the JSON file, as this helps provide the most information to users within the Textpattern themes site and assists with ongoing maintenance.

```JSON
{
  "name": "example",
  "repositories": [
    {
      "repoType": "homepage",
      "repoUrl": "https://example.com/example-theme/"
    },
    {
      "repoType": "github",
      "repoUrl": "https://github.com/exampleuser/example-theme"
    },
    {
      "repoType": "bitbucket",
      "repoUrl": "https://bitbucket.org/exampleuser/example-theme"
    },
    {
      "repoType": "gitlab",
      "repoUrl": "https://gitlab.com/exampleuser/example-theme"
    }
  ],
  "version": "2.2.0",
  "datePublished": "2020-09-04",
  "downloadUrl": "https://example.com/example-theme/download.zip",
  "demoUrl": "https://example.com/example-theme/demo/",
  "require": {
    "abc_extra_example1": ">=2.0.0",
    "abc_extra_example2": "1.5.1"
  }
}
```

A [JSON template](https://raw.githubusercontent.com/textpattern/textpattern-curated-themes-list/master/template.json) is provided as a useful starting point.

### Required entries

* `name`:\
  The name of the theme.
* `version`:\
  In `semver` format (e.g. `1.3.8`).
* `downloadUrl`:\
  A URL endpoint to download the theme source code (in `.zip` format).

### Example minimum structure

This is the minimum that is required in each JSON file:

```JSON
{
  "name": "example",
  "version": "2.2.0",
  "downloadUrl": "https://example.com/example-theme/download.zip"
}
```

### Optional (but recommended) entries

TODO

### Manifests for themes

TODO

### Linting

You can run a linter over the JSON files to check validity as follows (requires [Node.js](https://nodejs.org/)):

```ShellSession
$ cd textpattern-curated-themes-list
$ npm install
$ npm run jsonlint
```

## License

Licensed under [MIT license](https://github.com/textpattern/textpattern-curated-themes-list/blob/master/LICENSE).
