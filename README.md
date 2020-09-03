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
      "repoUrl": "https://example.com/abc_example.html"
    },
    {
      "repoType": "github",
      "repoUrl": "https://github.com/exampleuser/abc_example"
    },
    {
      "repoType": "bitbucket",
      "repoUrl": "https://bitbucket.org/exampleuser/abc_example"
    },
    {
      "repoType": "gitlab",
      "repoUrl": "https://gitlab.com/exampleuser/abc_example"
    }
  ],
  TODO
}
```

A [JSON template](https://raw.githubusercontent.com/textpattern/textpattern-curated-themes-list/master/template.json) is provided as a useful starting point.

### Required entries

TODO

### Example minimum structure

TODO

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
