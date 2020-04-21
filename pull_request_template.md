## Usage

### With Husky


### From CLI

```bash
$ validate-commit-msg 'chore(package): some message'
$ validate-commit-msg -p eslint 'New: Awesome feature'
$ validate-commit-msg -p ember '[DOC beta] Update CONTRIBUTING.md'
$ validate-commit-msg -p jshint '[[DOCS]] Awesome JS docs'
$ ...
```

When a wrong commit message is given it outputs an explaination.

```bash
$ validate-commit-msg 'unknown(something): wrong'
# 'unknown' is not an allowed type!
# Valid types are: feat, fix, docs, style, refactor, perf, test, chore, revert
```

However you can mute it:

```bash
$ validate-commit-msg -s 'unknown(something): wrong'
```


Validate a commit with .git directory in another location

```bash
$ validate-commit-msg --mf ../../some/.git/module/COMMIT_EDITMSG
```

## License

Apache-2.0 © [Will Soto](http://github.com/willsoto)

[npm-url]: https://npmjs.org/package/validate-commit
[npm-image]: https://img.shields.io/npm/v/validate-commit.svg?style=flat-square

[download-badge]: http://img.shields.io/npm/dm/validate-commit.svg?style=flat-square

[chalk-url]: https://www.npmjs.com/package/chalk
[husky-url]: https://www.npmjs.com/package/husky
