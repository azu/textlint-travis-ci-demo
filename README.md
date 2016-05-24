# textlint-travis-ci-demo

textlint with Travis CI demo repository

## Install

Install with [npm](https://www.npmjs.com/):

    npm install

## Usage

    npm run textlint
    # lint `docs/*` files with textlint

See [docs](docs).

## Travis CI setting

Add `npm scripts textlint` to `package.json`.

You can run textlint by `$ npm run textlint`.

```json
{
  "private": true,
  "scripts": {
    "textlint": "textlint -f pretty-error docs/"
  },
  "devDependencies": {
    "textlint": "^6.8.0",
    "textlint-rule-common-misspellings": "^1.0.1",
    "textlint-rule-preset-japanese": "^1.3.0"
  }
}
```

`.travis.yml`:

```yaml
sudo: false
language: node_js
node_js: "stable"
script:
  - npm run textlint
```


## Contributing

Pull requests and stars are always welcome.
For bugs and feature requests, [please create an issue](https://github.com/azu/textlint-travis-ci-demo/issues).

1. Fork it!
2. Create your feature branch: `git checkout -b my-new-feature`
3. Commit your changes: `git commit -am 'Add some feature'`
4. Push to the branch: `git push origin my-new-feature`
5. Submit a pull request :D

## Author

- [github/azu](https://github.com/azu)
- [twitter/azu_re](http://twitter.com/azu_re)

## License

MIT © azu
