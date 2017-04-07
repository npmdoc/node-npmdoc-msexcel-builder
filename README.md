# api documentation for  [msexcel-builder (v0.0.2)](https://github.com/chuanyi/msexcel-builder#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-msexcel-builder.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-msexcel-builder) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-msexcel-builder.svg)](https://travis-ci.org/npmdoc/node-npmdoc-msexcel-builder)
#### A tiny library to create Microsoft Office Excel(2007) files under Nodejs.

[![NPM](https://nodei.co/npm/msexcel-builder.png?downloads=true)](https://www.npmjs.com/package/msexcel-builder)

[![apidoc](https://npmdoc.github.io/node-npmdoc-msexcel-builder/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-msexcel-builder_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-msexcel-builder/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-msexcel-builder/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-msexcel-builder/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Charlie Zheng",
        "email": "chuanyi.zheng@gmail.com"
    },
    "bugs": {
        "url": "https://github.com/chuanyi/msexcel-builder/issues"
    },
    "dependencies": {
        "async": "~0.2.6",
        "easy-zip": "~0.0.4",
        "fs-extra": "~0.5.0",
        "xmlbuilder": ">=0.4.2"
    },
    "description": "A tiny library to create Microsoft Office Excel(2007) files under Nodejs.",
    "devDependencies": {},
    "directories": {},
    "dist": {
        "shasum": "dec552f0fb6f3bf368e5bd32bd926535677b03d0",
        "tarball": "https://registry.npmjs.org/msexcel-builder/-/msexcel-builder-0.0.2.tgz"
    },
    "engines": {
        "node": "*"
    },
    "homepage": "https://github.com/chuanyi/msexcel-builder#readme",
    "main": "./lib/msexcel-builder.js",
    "maintainers": [
        {
            "name": "chuanyi",
            "email": "chuanyi.zheng@gmail.com"
        }
    ],
    "name": "msexcel-builder",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git://github.com/chuanyi/msexcel-builder.git"
    },
    "tags": [
        "xlsx",
        "excel"
    ],
    "version": "0.0.2"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module msexcel-builder](#apidoc.module.msexcel-builder)
1.  [function <span class="apidocSignatureSpan">msexcel-builder.</span>createWorkbook (fpath, fname)](#apidoc.element.msexcel-builder.createWorkbook)



# <a name="apidoc.module.msexcel-builder"></a>[module msexcel-builder](#apidoc.module.msexcel-builder)

#### <a name="apidoc.element.msexcel-builder.createWorkbook"></a>[function <span class="apidocSignatureSpan">msexcel-builder.</span>createWorkbook (fpath, fname)](#apidoc.element.msexcel-builder.createWorkbook)
- description and source-code
```javascript
createWorkbook = function (fpath, fname) {
  return new Workbook(fpath, fname);
}
```
- example usage
```shell
...
var excelbuilder = require('msexcel-builder');
'''

Then create a sample workbook with one sheet and some data.

'''javascript
// Create a new workbook file in current working-path
var workbook = excelbuilder.createWorkbook('./', 'sample.xlsx')

// Create a new worksheet with 10 columns and 12 rows
var sheet1 = workbook.createSheet('sheet1', 10, 12);

// Fill some data
sheet1.set(1, 1, 'I am title');
for (var i = 2; i < 5; i++)
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
