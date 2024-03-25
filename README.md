This repository reproduces the bug from https://github.com/stylus/stylelint-stylus/issues/29

Requirements:
* yarn

---

Correct run using stylelint 16.2.0:
1. Install: `yarn install`
2. Run linter: `yarn lint`

Outcome: Stylelint works as expected

---

False run using stylelint 16.3.0:

1. Upgrade to latest stylelint (16.3.0): `yarn add stylelint`
2. Run linter: `yarn lint`

Outcome is the following error:

```bash
$ stylelint '**/*.css'
Error: No configuration provided for /home/foo/Projekte/fix_stylus/src/foo.css
```
