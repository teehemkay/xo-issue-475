# xo-issue-475

SSCCE for xo issue #475

First, install `xo`

``` sh
$ npm i
```

Now run the following command:

``` sh
$ xo foo/bar.js
```

Observe that there are no errors or warnings

Now run the following commands:

``` sh
$ cd foo
$ xo bar.js
```

Observe the following error message:

``` sh
bar.js:2:1
  ✖  2:1  Expected indentation of 1 tab but found 2 spaces.  indent
```

