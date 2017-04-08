# api documentation for  [react-ui-builder (v0.3.4)](https://github.com/ipselon/react-ui-builder#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-react-ui-builder.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-react-ui-builder) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-react-ui-builder.svg)](https://travis-ci.org/npmdoc/node-npmdoc-react-ui-builder)
#### The visual tool for prototyping UI for ReactJS components and Web applications.

[![NPM](https://nodei.co/npm/react-ui-builder.png?downloads=true)](https://www.npmjs.com/package/react-ui-builder)

[![apidoc](https://npmdoc.github.io/node-npmdoc-react-ui-builder/build/screenCapture.buildApidoc.browser.%252Fhome%252Ftravis%252Fbuild%252Fnpmdoc%252Fnode-npmdoc-react-ui-builder%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-react-ui-builder/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-react-ui-builder/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-react-ui-builder/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Alexander Pustovalov",
        "email": "apustovalov@gmail.com"
    },
    "bin": {
        "react-ui-builder": "react-ui-builder.js"
    },
    "bugs": {
        "url": "https://github.com/ipselon/react-ui-builder/issues"
    },
    "dependencies": {
        "babel-core": "5.8.3",
        "body-parser": "1.12.2",
        "escodegen": "1.6.1",
        "esformatter": "0.7.3",
        "esformatter-jsx": "2.0.11",
        "esprima": "2.2.0",
        "esprima-fb": "^15001.1001.0-dev-harmony-fb",
        "express": "4.12.3",
        "extract-text-webpack-plugin": "^0.8.2",
        "fs-extra": "0.17.0",
        "fstream": "1.0.6",
        "http-proxy": "1.11.1",
        "lodash": "^3.10.1",
        "request": "2.54.0",
        "socket.io": "1.3.5",
        "tar-fs": "1.5.1",
        "webpack": "1.10.1"
    },
    "description": "The visual tool for prototyping UI for ReactJS components and Web applications.",
    "devDependencies": {},
    "directories": {},
    "dist": {
        "shasum": "c6dfcdf8ed7a7cdb6ae167a3ec9224c4f1a697e7",
        "tarball": "https://registry.npmjs.org/react-ui-builder/-/react-ui-builder-0.3.4.tgz"
    },
    "engines": {
        "node": ">=0.12.2"
    },
    "homepage": "https://github.com/ipselon/react-ui-builder#readme",
    "keywords": [
        "reactjs",
        "UI",
        "web",
        "prototyping",
        "generating",
        "visual",
        "editor",
        "builder"
    ],
    "license": "MIT",
    "main": "react-ui-builder.js",
    "maintainers": [
        {
            "name": "ipselon",
            "email": "apustovalov@gmail.com"
        }
    ],
    "name": "react-ui-builder",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/ipselon/react-ui-builder.git"
    },
    "scripts": {
        "start": "node react-ui-builder.js"
    },
    "version": "0.3.4"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module react-ui-builder](#apidoc.module.react-ui-builder)
1.  object <span class="apidocSignatureSpan">react-ui-builder.</span>FileFormatter
1.  object <span class="apidocSignatureSpan">react-ui-builder.</span>FileParser
1.  object <span class="apidocSignatureSpan">react-ui-builder.</span>ModelParser
1.  object <span class="apidocSignatureSpan">react-ui-builder.</span>PathResolver

#### [module react-ui-builder.FileFormatter](#apidoc.module.react-ui-builder.FileFormatter)
1.  [function <span class="apidocSignatureSpan">react-ui-builder.FileFormatter.</span>formatJsFile (e)](#apidoc.element.react-ui-builder.FileFormatter.formatJsFile)

#### [module react-ui-builder.FileParser](#apidoc.module.react-ui-builder.FileParser)
1.  [function <span class="apidocSignatureSpan">react-ui-builder.FileParser.</span>getFileAst (e)](#apidoc.element.react-ui-builder.FileParser.getFileAst)
1.  [function <span class="apidocSignatureSpan">react-ui-builder.FileParser.</span>traverse (e, r)](#apidoc.element.react-ui-builder.FileParser.traverse)
1.  [function <span class="apidocSignatureSpan">react-ui-builder.FileParser.</span>validateSourceCode (e)](#apidoc.element.react-ui-builder.FileParser.validateSourceCode)

#### [module react-ui-builder.ModelParser](#apidoc.module.react-ui-builder.ModelParser)
1.  [function <span class="apidocSignatureSpan">react-ui-builder.ModelParser.</span>cleanModel (e)](#apidoc.element.react-ui-builder.ModelParser.cleanModel)
1.  [function <span class="apidocSignatureSpan">react-ui-builder.ModelParser.</span>getModelComponentMap (e)](#apidoc.element.react-ui-builder.ModelParser.getModelComponentMap)

#### [module react-ui-builder.PathResolver](#apidoc.module.react-ui-builder.PathResolver)
1.  [function <span class="apidocSignatureSpan">react-ui-builder.PathResolver.</span>replaceInPath (e, t)](#apidoc.element.react-ui-builder.PathResolver.replaceInPath)
1.  [function <span class="apidocSignatureSpan">react-ui-builder.PathResolver.</span>resolveFromComponentPerspective (e)](#apidoc.element.react-ui-builder.PathResolver.resolveFromComponentPerspective)
1.  [function <span class="apidocSignatureSpan">react-ui-builder.PathResolver.</span>resolveFromModulePerspective (e, t)](#apidoc.element.react-ui-builder.PathResolver.resolveFromModulePerspective)
1.  [function <span class="apidocSignatureSpan">react-ui-builder.PathResolver.</span>resolveFromProjectPerspective (e)](#apidoc.element.react-ui-builder.PathResolver.resolveFromProjectPerspective)



# <a name="apidoc.module.react-ui-builder"></a>[module react-ui-builder](#apidoc.module.react-ui-builder)



# <a name="apidoc.module.react-ui-builder.FileFormatter"></a>[module react-ui-builder.FileFormatter](#apidoc.module.react-ui-builder.FileFormatter)

#### <a name="apidoc.element.react-ui-builder.FileFormatter.formatJsFile"></a>[function <span class="apidocSignatureSpan">react-ui-builder.FileFormatter.</span>formatJsFile (e)](#apidoc.element.react-ui-builder.FileFormatter.formatJsFile)
- description and source-code
```javascript
function formatJsFile(e){try{return _esformatter2["default"].format(e,esformatterOptions)}catch(t){throw console.error(t),Error(
t.message)}}
```
- example usage
```shell
...







"use strict";function _interopRequireWildcard(e){if(e&&e.__esModule)return e;var r={};if(null!=e)for(var t in e)Object.prototype
.hasOwnProperty.call(e,t)&&(r[t]=e[t]);return r["default"]=e,r}function _interopRequireDefault(e){return e&&e.__esModule?e:{"default
":e}}function _classCallCheck(e,r){if(!(e instanceof r))throw new TypeError("Cannot call a class as a function")}Object.defineProperty
(exports,"__esModule",{value:!0});var _createClass=function(){function e(e,r){for(var t=0;t<r.length;t++){var n=r[t];n.enumerable
=n.enumerable||!1,n.configurable=!0,"value"in n&&(n.writable=!0),Object.defineProperty(e,n.key,n)}}return function(r,t,n){return
 t&&e(r.prototype,t),n&&e(r,n),r}}(),_lodash=require("lodash"),_lodash2=_interopRequireDefault(_lodash),_FileManagerJs=require("./
FileManager.js"),_FileManagerJs2=_interopRequireDefault(_FileManagerJs),_FileFormatterJs=require("./FileFormatter.js"),formatter
=_interopRequireWildcard(_FileFormatterJs),FileGenerator=function(){function e(){_classCallCheck(this,e),this.fileManager=new _FileManagerJs2
["default"]}return _createClass(e,[{key:"generateFile",value:function(e,r,t){var n=this;return this.fileManager.readFile(r).then
(function(r){var n=_lodash2["default"].template(r),a=n(t);return(-1!==e.indexOf(".js",e.length-3)||-1!==e.indexOf(".jsx",e.length
-4))&&(a=formatter.formatJsFile(a)),a}).then(function(r){return n.fileManager.ensureFilePath(e).then(function(){return r})}).then
(function(r){return n.fileManager.writeFile(e,r)})}}]),e}();exports["default"]=FileGenerator,module.exports=exports["default"];
...
```



# <a name="apidoc.module.react-ui-builder.FileParser"></a>[module react-ui-builder.FileParser](#apidoc.module.react-ui-builder.FileParser)

#### <a name="apidoc.element.react-ui-builder.FileParser.getFileAst"></a>[function <span class="apidocSignatureSpan">react-ui-builder.FileParser.</span>getFileAst (e)](#apidoc.element.react-ui-builder.FileParser.getFileAst)
- description and source-code
```javascript
function getFileAst(e){var r=null;try{r=_esprimaFb2["default"].parse(e,{tolerant:!0,range:!0,comment:!0})}catch(t){throw Error("
Can not parse file, error: "+t.message)}return r}
```
- example usage
```shell
...







"use strict";function _interopRequireWildcard(e){if(e&&e.__esModule)return e;var r={};if(null!=e)for(var n in e)Object.prototype
.hasOwnProperty.call(e,n)&&(r[n]=e[n]);return r["default"]=e,r}function _interopRequireDefault(e){return e&&e.__esModule?e:{"default
":e}}function _classCallCheck(e,r){if(!(e instanceof r))throw new TypeError("Cannot call a class as a function")}function findExportsNode
(e){var r=null;fileParser.traverse(e,function(e){"ExpressionStatement"===e.type&&"AssignmentExpression"===e.expression.type&&("Identifier
"===e.expression.left.type&&"exports"===e.expression.left.name?r=e.expression.right:"MemberExpression"===e.expression.left.type&&"
exports"===e.expression.left.property.name&&(r=e.expression.right))});var n=null;return"Identifier"===r.type&&(n=r.name,fileParser
.traverse(e,function(e){"VariableDeclarator"===e.type&&e.id.name===n&&(r=e.init)})),r}function appendToNode(e,r){var n=_esprimaFb2
["default"].parse("var c = {"+r+"}"),t=null;fileParser.traverse(n,function(e){"VariableDeclarator"===e.type&&"c"===e.id.name&&(t
=e.init.properties[0])}),e.properties&&e.properties.push(t)}function memberExpressionToString(e,r){var n=r||"";return"MemberExpression
"===e.type&&(n+=memberExpressionToString(e.object,n),n&&n.length>0?n+="."+e.property.name:n=e.property.name),n}Object.defineProperty
(exports,"__esModule",{value:!0});var _createClass=function(){function e(e,r){for(var n=0;n<r.length;n++){var t=r[n];t.enumerable
=t.enumerable||!1,t.configurable=!0,"value"in t&&(t.writable=!0),Object.defineProperty(e,t.key,t)}}return function(r,n,t){return
 n&&e(r.prototype,n),t&&e(r,t),r}}(),_lodash=require("lodash"),_lodash2=_interopRequireDefault(_lodash),_path=require("path"),_path2
=_interopRequireDefault(_path),_esprimaFb=require("esprima-fb"),_esprimaFb2=_interopRequireDefault(_esprimaFb),_escodegen=require
("escodegen"),_escodegen2=_interopRequireDefault(_escodegen),_FileManagerJs=require("./FileManager.js"),_FileManagerJs2=_interopRequireDefault
(_FileManagerJs),_FileParserJs=require("./FileParser.js"),fileParser=_interopRequireWildcard(_FileParserJs),group_keyword="@Group
:",resource_keyword="@Resources",IndexManager=function(){function e(r){var n=arguments.length<=1||void 0===arguments[1]?".builder
":arguments[1],t=arguments.length<=2||void 0===arguments[2]?"src":arguments[2],a=arguments.length<=3||void 0===arguments[3]?"index
.js":arguments[3];_classCallCheck(this,e),this.indexFilePath=_path2["default"].join(r,n,t,a),this.fileManager=new _FileManagerJs2
["default"]}return _createClass(e,[{key:"parseIndexFile",value:function(){var e=this;return this.fileManager.readFile(this.indexFilePath
).then(function(r){if(!r)throw Error("Index file is empty.");try{return fileParser.getFileAst(r)}catch(n){throw Error(n.message+".
File path: "+e.indexFilePath)}})}},{key:"getStructure",value:function(e){var r={requires:[],groups:{}};fileParser.traverse(e,function
(e){"ExpressionStatement"===e.type&&e.expression&&"CallExpression"===e.expression.type&&e.expression.callee&&"require"===e.expression
.callee.name&&r.requires.push({source:e.expression.arguments[0].value})});var n=findExportsNode(e);if(n){var t=n.properties;t&&t
.length>0&&t.map(function(e){var n=r.groups[e.key.name]={components:[]},t=e.value.properties;t&&t.length>0&&t.map(function(e){var
 r={name:e.key.name};fileParser.traverse(e,function(e){"CallExpression"===e.type&&e.callee&&"require"===e.callee.name&&e.arguments
&&e.arguments.length>0&&(r.source=e.arguments[0].value)}),"MemberExpression"===e.value.type&&(r.member=memberExpressionToString(
e.value)),n.components.push(r)})})}return r}},{key:"resolveAbsoluteSourcePath",value:function(e){var r=this,n=e.requires;n&&n.length
>0&&_lodash2["default"].forEach(n,function(e){e.source&&0===e.source.indexOf("../../")&&(e.absoluteSource=_path2["default"].resolve
(_path2["default"].dirname(r.indexFilePath),e.source))});var t=e.groups;return t&&_lodash2["default"].forOwn(t,function(e,n){e.components
&&e.components.length>0&&e.components.map(function(e){e.source&&0===e.source.indexOf("../../")&&(e.absoluteSource=_path2["default
"].resolve(_path2["default"].dirname(r.indexFilePath),e.source))})}),e}},{key:"initIndex",value:function(){var e=this;return this
.parseIndexFile().then(function(r){var n=e.getStructure(r);return n=e.resolveAbsoluteSourcePath(n)})}},{key:"getComponentsTree",
value:function(){return this.initIndex().then(function(e){var r={};return e&&e.groups&&_lodash2["default"].forOwn(e.groups,function
(e,n){r[n]={},e.components&&e.components.length>0&&e.components.map(function(e){r[n][e.name]={name:e.name,absoluteSource:e.absoluteSource
}})}),r})}},{key:"getComponentsNames",value:function(){var e=this;return this.getComponentsTree().then(function(r){return e.getComponentsNamesFromTree
(r)})}},{key:"getComponentsNamesFromTree",value:function(e){var r=[];return _lodash2["default"].forOwn(e,function(e,n){_lodash2["
default"].forOwn(e,function(e,n){r.push(n)})}),r}},{key:"addComponent",value:function(e,r,n){var t=this;return this.parseIndexFile
().then(function(t){var a=findExportsNode(t);if(a){var o=null;fileParser.traverse(a,function(r){"Property"===r.type&&"Identifier
"===r.key.type&&"ObjectExpression"===r.value.type&&r.key.name===e&&(o=r.value)}),o?appendToNode(o,r+': require("'+n+'")'):appendToNode
(a,e+": {"+r+': require("'+n+'")}')}return _escodegen2["default"].generate(t)}).then(function(e){return t.fileManager.writeFile(
t.indexFilePath,e,!0)}).then(function(){return t.initIndex()})}}]),e}();exports["default"]=IndexManager,module.exports=exports["
default"];
...
```

#### <a name="apidoc.element.react-ui-builder.FileParser.traverse"></a>[function <span class="apidocSignatureSpan">react-ui-builder.FileParser.</span>traverse (e, r)](#apidoc.element.react-ui-builder.FileParser.traverse)
- description and source-code
```javascript
function traverse(e, r){r(e);for(var t in e)if(e.hasOwnProperty(t)){var a=e[t];"object"==typeof a&&null!==a&&traverse(a,r)}}
```
- example usage
```shell
...







"use strict";function _interopRequireWildcard(e){if(e&&e.__esModule)return e;var r={};if(null!=e)for(var n in e)Object.prototype
.hasOwnProperty.call(e,n)&&(r[n]=e[n]);return r["default"]=e,r}function _interopRequireDefault(e){return e&&e.__esModule?e:{"default
":e}}function _classCallCheck(e,r){if(!(e instanceof r))throw new TypeError("Cannot call a class as a function")}function findExportsNode
(e){var r=null;fileParser.traverse(e,function(e){"ExpressionStatement"===e.type&&"AssignmentExpression"===e.expression.type&&("Identifier
"===e.expression.left.type&&"exports"===e.expression.left.name?r=e.expression.right:"MemberExpression"===e.expression.left.type&&"
exports"===e.expression.left.property.name&&(r=e.expression.right))});var n=null;return"Identifier"===r.type&&(n=r.name,fileParser
.traverse(e,function(e){"VariableDeclarator"===e.type&&e.id.name===n&&(r=e.init)})),r}function appendToNode(e,r){var n=_esprimaFb2
["default"].parse("var c = {"+r+"}"),t=null;fileParser.traverse(n,function(e){"VariableDeclarator"===e.type&&"c"===e.id.name&&(t
=e.init.properties[0])}),e.properties&&e.properties.push(t)}function memberExpressionToString(e,r){var n=r||"";return"MemberExpression
"===e.type&&(n+=memberExpressionToString(e.object,n),n&&n.length>0?n+="."+e.property.name:n=e.property.name),n}Object.defineProperty
(exports,"__esModule",{value:!0});var _createClass=function(){function e(e,r){for(var n=0;n<r.length;n++){var t=r[n];t.enumerable
=t.enumerable||!1,t.configurable=!0,"value"in t&&(t.writable=!0),Object.defineProperty(e,t.key,t)}}return function(r,n,t){return
 n&&e(r.prototype,n),t&&e(r,t),r}}(),_lodash=require("lodash"),_lodash2=_interopRequireDefault(_lodash),_path=require("path"),_path2
=_interopRequireDefault(_path),_esprimaFb=require("esprima-fb"),_esprimaFb2=_interopRequireDefault(_esprimaFb),_escodegen=require
("escodegen"),_escodegen2=_interopRequireDefault(_escodegen),_FileManagerJs=require("./FileManager.js"),_FileManagerJs2=_interopRequireDefault
(_FileManagerJs),_FileParserJs=require("./FileParser.js"),fileParser=_interopRequireWildcard(_FileParserJs),group_keyword="@Group
:",resource_keyword="@Resources",IndexManager=function(){function e(r){var n=arguments.length<=1||void 0===arguments[1]?".builder
":arguments[1],t=arguments.length<=2||void 0===arguments[2]?"src":arguments[2],a=arguments.length<=3||void 0===arguments[3]?"index
.js":arguments[3];_classCallCheck(this,e),this.indexFilePath=_path2["default"].join(r,n,t,a),this.fileManager=new _FileManagerJs2
["default"]}return _createClass(e,[{key:"parseIndexFile",value:function(){var e=this;return this.fileManager.readFile(this.indexFilePath
).then(function(r){if(!r)throw Error("Index file is empty.");try{return fileParser.getFileAst(r)}catch(n){throw Error(n.message+".
File path: "+e.indexFilePath)}})}},{key:"getStructure",value:function(e){var r={requires:[],groups:{}};fileParser.traverse(e,function
(e){"ExpressionStatement"===e.type&&e.expression&&"CallExpression"===e.expression.type&&e.expression.callee&&"require"===e.expression
.callee.name&&r.requires.push({source:e.expression.arguments[0].value})});var n=findExportsNode(e);if(n){var t=n.properties;t&&t
.length>0&&t.map(function(e){var n=r.groups[e.key.name]={components:[]},t=e.value.properties;t&&t.length>0&&t.map(function(e){var
 r={name:e.key.name};fileParser.traverse(e,function(e){"CallExpression"===e.type&&e.callee&&"require"===e.callee.name&&e.arguments
&&e.arguments.length>0&&(r.source=e.arguments[0].value)}),"MemberExpression"===e.value.type&&(r.member=memberExpressionToString(
e.value)),n.components.push(r)})})}return r}},{key:"resolveAbsoluteSourcePath",value:function(e){var r=this,n=e.requires;n&&n.length
>0&&_lodash2["default"].forEach(n,function(e){e.source&&0===e.source.indexOf("../../")&&(e.absoluteSource=_path2["default"].resolve
(_path2["default"].dirname(r.indexFilePath),e.source))});var t=e.groups;return t&&_lodash2["default"].forOwn(t,function(e,n){e.components
&&e.components.length>0&&e.components.map(function(e){e.source&&0===e.source.indexOf("../../")&&(e.absoluteSource=_path2["default
"].resolve(_path2["default"].dirname(r.indexFilePath),e.source))})}),e}},{key:"initIndex",value:function(){var e=this;return this
.parseIndexFile().then(function(r){var n=e.getStructure(r);return n=e.resolveAbsoluteSourcePath(n)})}},{key:"getComponentsTree",
value:function(){return this.initIndex().then(function(e){var r={};return e&&e.groups&&_lodash2["default"].forOwn(e.groups,function
(e,n){r[n]={},e.components&&e.components.length>0&&e.components.map(function(e){r[n][e.name]={name:e.name,absoluteSource:e.absoluteSource
}})}),r})}},{key:"getComponentsNames",value:function(){var e=this;return this.getComponentsTree().then(function(r){return e.getComponentsNamesFromTree
(r)})}},{key:"getComponentsNamesFromTree",value:function(e){var r=[];return _lodash2["default"].forOwn(e,function(e,n){_lodash2["
default"].forOwn(e,function(e,n){r.push(n)})}),r}},{key:"addComponent",value:function(e,r,n){var t=this;return this.parseIndexFile
().then(function(t){var a=findExportsNode(t);if(a){var o=null;fileParser.traverse(a,function(r){"Property"===r.type&&"Identifier
"===r.key.type&&"ObjectExpression"===r.value.type&&r.key.name===e&&(o=r.value)}),o?appendToNode(o,r+': require("'+n+'")'):appendToNode
(a,e+": {"+r+': require("'+n+'")}')}return _escodegen2["default"].generate(t)}).then(function(e){return t.fileManager.writeFile(
t.indexFilePath,e,!0)}).then(function(){return t.initIndex()})}}]),e}();exports["default"]=IndexManager,module.exports=exports["
default"];
...
```

#### <a name="apidoc.element.react-ui-builder.FileParser.validateSourceCode"></a>[function <span class="apidocSignatureSpan">react-ui-builder.FileParser.</span>validateSourceCode (e)](#apidoc.element.react-ui-builder.FileParser.validateSourceCode)
- description and source-code
```javascript
function validateSourceCode(e){try{_esprimaFb2["default"].parse(e,{tolerant:!0})}catch(r){throw Error("File is not valid, error: "+
r.message)}}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.react-ui-builder.ModelParser"></a>[module react-ui-builder.ModelParser](#apidoc.module.react-ui-builder.ModelParser)

#### <a name="apidoc.element.react-ui-builder.ModelParser.cleanModel"></a>[function <span class="apidocSignatureSpan">react-ui-builder.ModelParser.</span>cleanModel (e)](#apidoc.element.react-ui-builder.ModelParser.cleanModel)
- description and source-code
```javascript
function cleanModel(e){if(e.props&&e.props["data-umyid"]&&(e.props["data-umyid"]=void 0,delete e.props["data-umyid"]),_lodash2["
default"].forOwn(e.props,function(e,o){_lodash2["default"].isObject(e)&&e.type&&cleanModel(e)}),e.children&&e.children.length>0)
for(var o=0;o<e.children.length;o++)cleanModel(e.children[o])}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-ui-builder.ModelParser.getModelComponentMap"></a>[function <span class="apidocSignatureSpan">react-ui-builder.ModelParser.</span>getModelComponentMap (e)](#apidoc.element.react-ui-builder.ModelParser.getModelComponentMap)
- description and source-code
```javascript
function getModelComponentMap(e){var o=arguments.length<=1||void 0===arguments[1]?{}:arguments[1];if(o[e.type]={},e.props&&_lodash2
["default"].forOwn(e.props,function(e,t){_lodash2["default"].isObject(e)&&e.type&&getModelComponentMap(e,o)}),e.children&&e.children
.length>0)for(var t=0;t<e.children.length;t++)getModelComponentMap(e.children[t],o);return o}
```
- example usage
```shell
...







"use strict";function _interopRequireWildcard(e){if(e&&e.__esModule)return e;var t={};if(null!=e)for(var r in e)Object.prototype
.hasOwnProperty.call(e,r)&&(t[r]=e[r]);return t["default"]=e,t}function _interopRequireDefault(e){return e&&e.__esModule?e:{"default
":e}}function _classCallCheck(e,t){if(!(e instanceof t))throw new TypeError("Cannot call a class as a function")}Object.defineProperty
(exports,"__esModule",{value:!0});var _createClass=function(){function e(e,t){for(var r=0;r<t.length;r++){var n=t[r];n.enumerable
=n.enumerable||!1,n.configurable=!0,"value"in n&&(n.writable=!0),Object.defineProperty(e,n.key,n)}}return function(t,r,n){return
 r&&e(t.prototype,r),n&&e(t,n),t}}(),_lodash=require("lodash"),_lodash2=_interopRequireDefault(_lodash),_path=require("path"),_path2
=_interopRequireDefault(_path),_FileManagerJs=require("./FileManager.js"),_FileManagerJs2=_interopRequireDefault(_FileManagerJs),
_IndexManagerJs=require("./IndexManager.js"),_IndexManagerJs2=_interopRequireDefault(_IndexManagerJs),_ModelParserJs=require("./
ModelParser.js"),modelParser=_interopRequireWildcard(_ModelParserJs),_PathResolverJs=require("./PathResolver.js"),pathResolver=_interopRequireWildcard
(_PathResolverJs),_FileFormatterJs=require("./FileFormatter.js"),formatter=_interopRequireWildcard(_FileFormatterJs),GeneratorManager
=function(){function e(t){var r=arguments.length<=1||void 0===arguments[1]?".builder":arguments[1],n=arguments.length<=2||void 0
===arguments[2]?"generators":arguments[2],o=arguments.length<=3||void 0===arguments[3]?"src":arguments[3],a=arguments.length<=4||
void 0===arguments[4]?"scripts":arguments[4];_classCallCheck(this,e),this.projectDirPath=t,this.builderDirPath=_path2["default"].
join(t,r),this.generatorsDirPath=_path2["default"].join(this.builderDirPath,n),this.sourceDirPath=_path2["default"].join(this.builderDirPath
,o),this.indexFilePath=_path2["default"].join(this.sourceDirPath,"index.js"),this.scriptsDirName=a,this.fileManager=new _FileManagerJs2
["default"],this.indexManager=new _IndexManagerJs2["default"](this.projectDirPath)}return _createClass(e,[{key:"initGenerator",value
:function(e){var t=this;return this.fileManager.readDirectory(this.generatorsDirPath,["generator.json"]).then(function(r){if(!r.
files||r.files.length<=0)throw Error("Current project does not have a generator, please add a generator.");return r.files.reduce
(function(r,n){return r.then(function(r){return r?r:t.fileManager.readJson(n).then(function(t){return t.name===e?{dirPath:_path2
["default"].dirname(n),filePath:n,config:t}:null})})["catch"](function(e){throw Error(e.message+". Generator file path: "+n)})},
Promise.resolve())})}},{key:"getGeneratorList",value:function(){var e=this;return this.fileManager.readDirectory(this.generatorsDirPath
,["generator.json"]).then(function(t){if(!t.files||t.files.length<=0)throw Error("Current project does not have a generator, please
 add a generator.");var r=[],n=t.files.reduce(function(t,n){return t.then(function(t){return t?t:e.fileManager.readJson(n).then(
function(e){r.push({dirPath:_path2["default"].dirname(n),filePath:n,config:e})})})["catch"](function(e){throw Error(e.message+".
Generator file path: "+n)})},Promise.resolve());return n.then(function(){return r.sort(function(e,t){return e.config.name>t.config
.name?1:e.config.name<t.config.name?-1:0}),r})})}},{key:"createDataObject",value:function(e,t,r){var n=this,o={component:{model:
e,componentName:r.componentName,groupName:r.groupName,indexFilePath:this.indexFilePath}};return this.indexManager.initIndex().then
(function(r){o.component.imports=[];var a=modelParser.getModelComponentMap(e);return r.groups&&_lodash2["default"].forOwn(r.groups
,function(e,t){e.components&&e.components.length>0&&e.components.map(function(e){a[e.name]&&o.component.imports.push({name:e.name
,source:e.source,member:e.member})})}),n.initGenerator(t).then(function(e){if(!e.config)throw Error("Generator "+e.filePath+" is
 not configured properly.");if(!e.config.component)throw Error("Generator "+e.filePath+" configuration does not have component section
.");return o.component.outputFilePath=_path2["default"].join(n.projectDirPath,pathResolver.replaceInPath(e.config.component.destDirPath
,_lodash2["default"].pick(o.component,["componentName","groupName"])),o.component.componentName+"."+e.config.component.fileExtension
),o.component.generatorScriptPath=_path2["default"].join(e.dirPath,n.scriptsDirName,e.config.component.script),o.modules={},e.config
.modules&&e.config.modules.length>0&&e.config.modules.map(function(t,r){var a=_lodash2["default"].pick(o.component,["componentName
","groupName"]);o.modules[t.id]={outputFilePath:_path2["default"].join(n.projectDirPath,pathResolver.replaceInPath(t.destDirPath
,a),pathResolver.replaceInPath(t.name,a)+".js"),name:pathResolver.replaceInPath(t.name,a),generatorScriptPath:_path2["default"].
join(e.dirPath,n.scriptsDirName,t.script),validateJS:t.validateJS}}),o})})}},{key:"doGeneration",value:function(e,t,r){var n=this
;return this.createDataObject(e,t,r).then(function(e){var t={component:{},modules:{}},r=Promise.resolve();return r=r.then(function
(){var r=pathResolver.resolveFromComponentPerspective(e);return n.generateText(r.component.generatorScriptPath,r).then(function(
e){t.component.sourceCode=e,t.component.outputFilePath=r.component.outputFilePath,t.component.relativeFilePathInIndex=r.component
.relativeFilePathInIndex,t.component.componentName=r.component.componentName,t.component.groupName=r.component.groupName})}),_lodash2
["default"].forOwn(e.modules,function(o,a){r=r.then(function(){try{var r=function(){var r=pathResolver.resolveFromModulePerspective
(e,a);return{v:n.generateText(o.generatorScriptPath,r).then(function(e){t.modules[a]={sourceCode:e,outputFilePath:r.modules[a].outputFilePath
,name:r.modules[a].name}})}}();if("object"==typeof r)return r.v}catch(i){throw Error(i)}})}),r=r.then(function(){return n.fileManager
.removeFile(_path2["default"].join(n.projectDirPath,".errors")).then(function(){return t})})})}},{key:"commitGeneration",value:function
(e){var t=this,r=Promise.resolve();return _lodash2["default"].forOwn(e.modules,function(e,n){r=r.then(function(){return t.fileManager
.ensureFilePath(e.outputFilePath).then(function(){return t.fileManager.writeFile(e.outputFilePath,e.sourceCode,!0)})})}),r=r.then
(function(){return t.fileManager.ensureFilePath(e.component.outputFilePath).then(function(){return t.fileManager.writeFile(e.component
.outputFilePath,e.component.sourceCode,!0).then(function(){return t.indexManager.addComponent(e.component.groupName,e.component.
componentName,e.component.relativeFilePathInIndex)})})})}},{key:"generateText",value:function(e,t){var r=this,n=arguments.length
<=2||void 0===arguments[2]?!0:arguments[2];return new Promise(function(o,a){try{var i=require.resolve(e);i&&require.cache[i]&&delete
 require.cache[i];var u=require(e);u(t,function(t){n?!function(){var n=t;try{var i=formatter.formatJsFile(t);o(i)}catch(u){!function
(){var t=_path2["default"].join(r.projectDirPath,".errors","generators",_path2["default"].basename(e));r.fileManager.ensureFilePath
(t).then(function(){r.fileManager.writeFile(t,n)})["catch"](function(e){console.error("Writing bad file. Error: "+e)}),a("Validation
 failed. "+u+". Generator script file path: "+e)}()}}():o(t)},function(t){a("Processing generator's method is failed. Error: "+t
+". File path: "+e)})}catch(s){a("Loading generator's script is failed. Error: "+s+". File path: "+e)}})}}]),e}();exports["default
"]=GeneratorManager,module.exports=exports["default"];
...
```



# <a name="apidoc.module.react-ui-builder.PathResolver"></a>[module react-ui-builder.PathResolver](#apidoc.module.react-ui-builder.PathResolver)

#### <a name="apidoc.element.react-ui-builder.PathResolver.replaceInPath"></a>[function <span class="apidocSignatureSpan">react-ui-builder.PathResolver.</span>replaceInPath (e, t)](#apidoc.element.react-ui-builder.PathResolver.replaceInPath)
- description and source-code
```javascript
function replaceInPath(e, t){var r=e;return _lodash2["default"].forOwn(t,function(e,t){r=r.replace("{"+t+"}",e)}),r}
```
- example usage
```shell
...







"use strict";function _interopRequireWildcard(e){if(e&&e.__esModule)return e;var t={};if(null!=e)for(var r in e)Object.prototype
.hasOwnProperty.call(e,r)&&(t[r]=e[r]);return t["default"]=e,t}function _interopRequireDefault(e){return e&&e.__esModule?e:{"default
":e}}function _classCallCheck(e,t){if(!(e instanceof t))throw new TypeError("Cannot call a class as a function")}Object.defineProperty
(exports,"__esModule",{value:!0});var _createClass=function(){function e(e,t){for(var r=0;r<t.length;r++){var n=t[r];n.enumerable
=n.enumerable||!1,n.configurable=!0,"value"in n&&(n.writable=!0),Object.defineProperty(e,n.key,n)}}return function(t,r,n){return
 r&&e(t.prototype,r),n&&e(t,n),t}}(),_lodash=require("lodash"),_lodash2=_interopRequireDefault(_lodash),_path=require("path"),_path2
=_interopRequireDefault(_path),_FileManagerJs=require("./FileManager.js"),_FileManagerJs2=_interopRequireDefault(_FileManagerJs),
_IndexManagerJs=require("./IndexManager.js"),_IndexManagerJs2=_interopRequireDefault(_IndexManagerJs),_ModelParserJs=require("./
ModelParser.js"),modelParser=_interopRequireWildcard(_ModelParserJs),_PathResolverJs=require("./PathResolver.js"),pathResolver=_interopRequireWildcard
(_PathResolverJs),_FileFormatterJs=require("./FileFormatter.js"),formatter=_interopRequireWildcard(_FileFormatterJs),GeneratorManager
=function(){function e(t){var r=arguments.length<=1||void 0===arguments[1]?".builder":arguments[1],n=arguments.length<=2||void 0
===arguments[2]?"generators":arguments[2],o=arguments.length<=3||void 0===arguments[3]?"src":arguments[3],a=arguments.length<=4||
void 0===arguments[4]?"scripts":arguments[4];_classCallCheck(this,e),this.projectDirPath=t,this.builderDirPath=_path2["default"].
join(t,r),this.generatorsDirPath=_path2["default"].join(this.builderDirPath,n),this.sourceDirPath=_path2["default"].join(this.builderDirPath
,o),this.indexFilePath=_path2["default"].join(this.sourceDirPath,"index.js"),this.scriptsDirName=a,this.fileManager=new _FileManagerJs2
["default"],this.indexManager=new _IndexManagerJs2["default"](this.projectDirPath)}return _createClass(e,[{key:"initGenerator",value
:function(e){var t=this;return this.fileManager.readDirectory(this.generatorsDirPath,["generator.json"]).then(function(r){if(!r.
files||r.files.length<=0)throw Error("Current project does not have a generator, please add a generator.");return r.files.reduce
(function(r,n){return r.then(function(r){return r?r:t.fileManager.readJson(n).then(function(t){return t.name===e?{dirPath:_path2
["default"].dirname(n),filePath:n,config:t}:null})})["catch"](function(e){throw Error(e.message+". Generator file path: "+n)})},
Promise.resolve())})}},{key:"getGeneratorList",value:function(){var e=this;return this.fileManager.readDirectory(this.generatorsDirPath
,["generator.json"]).then(function(t){if(!t.files||t.files.length<=0)throw Error("Current project does not have a generator, please
 add a generator.");var r=[],n=t.files.reduce(function(t,n){return t.then(function(t){return t?t:e.fileManager.readJson(n).then(
function(e){r.push({dirPath:_path2["default"].dirname(n),filePath:n,config:e})})})["catch"](function(e){throw Error(e.message+".
Generator file path: "+n)})},Promise.resolve());return n.then(function(){return r.sort(function(e,t){return e.config.name>t.config
.name?1:e.config.name<t.config.name?-1:0}),r})})}},{key:"createDataObject",value:function(e,t,r){var n=this,o={component:{model:
e,componentName:r.componentName,groupName:r.groupName,indexFilePath:this.indexFilePath}};return this.indexManager.initIndex().then
(function(r){o.component.imports=[];var a=modelParser.getModelComponentMap(e);return r.groups&&_lodash2["default"].forOwn(r.groups
,function(e,t){e.components&&e.components.length>0&&e.components.map(function(e){a[e.name]&&o.component.imports.push({name:e.name
,source:e.source,member:e.member})})}),n.initGenerator(t).then(function(e){if(!e.config)throw Error("Generator "+e.filePath+" is
 not configured properly.");if(!e.config.component)throw Error("Generator "+e.filePath+" configuration does not have component section
.");return o.component.outputFilePath=_path2["default"].join(n.projectDirPath,pathResolver.replaceInPath(e.config.component.destDirPath
,_lodash2["default"].pick(o.component,["componentName","groupName"])),o.component.componentName+"."+e.config.component.fileExtension
),o.component.generatorScriptPath=_path2["default"].join(e.dirPath,n.scriptsDirName,e.config.component.script),o.modules={},e.config
.modules&&e.config.modules.length>0&&e.config.modules.map(function(t,r){var a=_lodash2["default"].pick(o.component,["componentName
","groupName"]);o.modules[t.id]={outputFilePath:_path2["default"].join(n.projectDirPath,pathResolver.replaceInPath(t.destDirPath
,a),pathResolver.replaceInPath(t.name,a)+".js"),name:pathResolver.replaceInPath(t.name,a),generatorScriptPath:_path2["default"].
join(e.dirPath,n.scriptsDirName,t.script),validateJS:t.validateJS}}),o})})}},{key:"doGeneration",value:function(e,t,r){var n=this
;return this.createDataObject(e,t,r).then(function(e){var t={component:{},modules:{}},r=Promise.resolve();return r=r.then(function
(){var r=pathResolver.resolveFromComponentPerspective(e);return n.generateText(r.component.generatorScriptPath,r).then(function(
e){t.component.sourceCode=e,t.component.outputFilePath=r.component.outputFilePath,t.component.relativeFilePathInIndex=r.component
.relativeFilePathInIndex,t.component.componentName=r.component.componentName,t.component.groupName=r.component.groupName})}),_lodash2
["default"].forOwn(e.modules,function(o,a){r=r.then(function(){try{var r=function(){var r=pathResolver.resolveFromModulePerspective
(e,a);return{v:n.generateText(o.generatorScriptPath,r).then(function(e){t.modules[a]={sourceCode:e,outputFilePath:r.modules[a].outputFilePath
,name:r.modules[a].name}})}}();if("object"==typeof r)return r.v}catch(i){throw Error(i)}})}),r=r.then(function(){return n.fileManager
.removeFile(_path2["default"].join(n.projectDirPath,".errors")).then(function(){return t})})})}},{key:"commitGeneration",value:function
(e){var t=this,r=Promise.resolve();return _lodash2["default"].forOwn(e.modules,function(e,n){r=r.then(function(){return t.fileManager
.ensureFilePath(e.outputFilePath).then(function(){return t.fileManager.writeFile(e.outputFilePath,e.sourceCode,!0)})})}),r=r.then
(function(){return t.fileManager.ensureFilePath(e.component.outputFilePath).then(function(){return t.fileManager.writeFile(e.component
.outputFilePath,e.component.sourceCode,!0).then(function(){return t.indexManager.addComponent(e.component.groupName,e.component.
componentName,e.component.relativeFilePathInIndex)})})})}},{key:"generateText",value:function(e,t){var r=this,n=arguments.length
<=2||void 0===arguments[2]?!0:arguments[2];return new Promise(function(o,a){try{var i=require.resolve(e);i&&require.cache[i]&&delete
 require.cache[i];var u=require(e);u(t,function(t){n?!function(){var n=t;try{var i=formatter.formatJsFile(t);o(i)}catch(u){!function
(){var t=_path2["default"].join(r.projectDirPath,".errors","generators",_path2["default"].basename(e));r.fileManager.ensureFilePath
(t).then(function(){r.fileManager.writeFile(t,n)})["catch"](function(e){console.error("Writing bad file. Error: "+e)}),a("Validation
 failed. "+u+". Generator script file path: "+e)}()}}():o(t)},function(t){a("Processing generator's method is failed. Error: "+t
+". File path: "+e)})}catch(s){a("Loading generator's script is failed. Error: "+s+". File path: "+e)}})}}]),e}();exports["default
"]=GeneratorManager,module.exports=exports["default"];
...
```

#### <a name="apidoc.element.react-ui-builder.PathResolver.resolveFromComponentPerspective"></a>[function <span class="apidocSignatureSpan">react-ui-builder.PathResolver.</span>resolveFromComponentPerspective (e)](#apidoc.element.react-ui-builder.PathResolver.resolveFromComponentPerspective)
- description and source-code
```javascript
function resolveFromComponentPerspective(e){var t=_lodash2["default"].clone(e,!0),r=t.component.outputFilePath,a=_path2["default
"].dirname(r),o=_path2["default"].dirname(t.component.indexFilePath);return t.component.relativeFilePathInIndex=_path2["default"].
relative(o,r).replace(/\\/g,"/"),t.component.imports.map(function(e,t){if("../../"===e.source.substr(0,6)){var r=_path2["default"].resolve(o,e.source);e.relativeSource=repairPath(_path2["default"].relative(a,r)).replace(/\\/g,"/")}else e.relativeSource=e.source}),_lodash2["default"].forOwn(t.modules,function(e,t){e.relativeFilePath=repairPath(_path2["default"].relative(a,e.outputFilePath)).replace(/\\/g,"/")}),t}
```
- example usage
```shell
...







"use strict";function _interopRequireWildcard(e){if(e&&e.__esModule)return e;var t={};if(null!=e)for(var r in e)Object.prototype
.hasOwnProperty.call(e,r)&&(t[r]=e[r]);return t["default"]=e,t}function _interopRequireDefault(e){return e&&e.__esModule?e:{"default
":e}}function _classCallCheck(e,t){if(!(e instanceof t))throw new TypeError("Cannot call a class as a function")}Object.defineProperty
(exports,"__esModule",{value:!0});var _createClass=function(){function e(e,t){for(var r=0;r<t.length;r++){var n=t[r];n.enumerable
=n.enumerable||!1,n.configurable=!0,"value"in n&&(n.writable=!0),Object.defineProperty(e,n.key,n)}}return function(t,r,n){return
 r&&e(t.prototype,r),n&&e(t,n),t}}(),_lodash=require("lodash"),_lodash2=_interopRequireDefault(_lodash),_path=require("path"),_path2
=_interopRequireDefault(_path),_FileManagerJs=require("./FileManager.js"),_FileManagerJs2=_interopRequireDefault(_FileManagerJs),
_IndexManagerJs=require("./IndexManager.js"),_IndexManagerJs2=_interopRequireDefault(_IndexManagerJs),_ModelParserJs=require("./
ModelParser.js"),modelParser=_interopRequireWildcard(_ModelParserJs),_PathResolverJs=require("./PathResolver.js"),pathResolver=_interopRequireWildcard
(_PathResolverJs),_FileFormatterJs=require("./FileFormatter.js"),formatter=_interopRequireWildcard(_FileFormatterJs),GeneratorManager
=function(){function e(t){var r=arguments.length<=1||void 0===arguments[1]?".builder":arguments[1],n=arguments.length<=2||void 0
===arguments[2]?"generators":arguments[2],o=arguments.length<=3||void 0===arguments[3]?"src":arguments[3],a=arguments.length<=4||
void 0===arguments[4]?"scripts":arguments[4];_classCallCheck(this,e),this.projectDirPath=t,this.builderDirPath=_path2["default"].
join(t,r),this.generatorsDirPath=_path2["default"].join(this.builderDirPath,n),this.sourceDirPath=_path2["default"].join(this.builderDirPath
,o),this.indexFilePath=_path2["default"].join(this.sourceDirPath,"index.js"),this.scriptsDirName=a,this.fileManager=new _FileManagerJs2
["default"],this.indexManager=new _IndexManagerJs2["default"](this.projectDirPath)}return _createClass(e,[{key:"initGenerator",value
:function(e){var t=this;return this.fileManager.readDirectory(this.generatorsDirPath,["generator.json"]).then(function(r){if(!r.
files||r.files.length<=0)throw Error("Current project does not have a generator, please add a generator.");return r.files.reduce
(function(r,n){return r.then(function(r){return r?r:t.fileManager.readJson(n).then(function(t){return t.name===e?{dirPath:_path2
["default"].dirname(n),filePath:n,config:t}:null})})["catch"](function(e){throw Error(e.message+". Generator file path: "+n)})},
Promise.resolve())})}},{key:"getGeneratorList",value:function(){var e=this;return this.fileManager.readDirectory(this.generatorsDirPath
,["generator.json"]).then(function(t){if(!t.files||t.files.length<=0)throw Error("Current project does not have a generator, please
 add a generator.");var r=[],n=t.files.reduce(function(t,n){return t.then(function(t){return t?t:e.fileManager.readJson(n).then(
function(e){r.push({dirPath:_path2["default"].dirname(n),filePath:n,config:e})})})["catch"](function(e){throw Error(e.message+".
Generator file path: "+n)})},Promise.resolve());return n.then(function(){return r.sort(function(e,t){return e.config.name>t.config
.name?1:e.config.name<t.config.name?-1:0}),r})})}},{key:"createDataObject",value:function(e,t,r){var n=this,o={component:{model:
e,componentName:r.componentName,groupName:r.groupName,indexFilePath:this.indexFilePath}};return this.indexManager.initIndex().then
(function(r){o.component.imports=[];var a=modelParser.getModelComponentMap(e);return r.groups&&_lodash2["default"].forOwn(r.groups
,function(e,t){e.components&&e.components.length>0&&e.components.map(function(e){a[e.name]&&o.component.imports.push({name:e.name
,source:e.source,member:e.member})})}),n.initGenerator(t).then(function(e){if(!e.config)throw Error("Generator "+e.filePath+" is
 not configured properly.");if(!e.config.component)throw Error("Generator "+e.filePath+" configuration does not have component section
.");return o.component.outputFilePath=_path2["default"].join(n.projectDirPath,pathResolver.replaceInPath(e.config.component.destDirPath
,_lodash2["default"].pick(o.component,["componentName","groupName"])),o.component.componentName+"."+e.config.component.fileExtension
),o.component.generatorScriptPath=_path2["default"].join(e.dirPath,n.scriptsDirName,e.config.component.script),o.modules={},e.config
.modules&&e.config.modules.length>0&&e.config.modules.map(function(t,r){var a=_lodash2["default"].pick(o.component,["componentName
","groupName"]);o.modules[t.id]={outputFilePath:_path2["default"].join(n.projectDirPath,pathResolver.replaceInPath(t.destDirPath
,a),pathResolver.replaceInPath(t.name,a)+".js"),name:pathResolver.replaceInPath(t.name,a),generatorScriptPath:_path2["default"].
join(e.dirPath,n.scriptsDirName,t.script),validateJS:t.validateJS}}),o})})}},{key:"doGeneration",value:function(e,t,r){var n=this
;return this.createDataObject(e,t,r).then(function(e){var t={component:{},modules:{}},r=Promise.resolve();return r=r.then(function
(){var r=pathResolver.resolveFromComponentPerspective(e);return n.generateText(r.component.generatorScriptPath,r).then(function(
e){t.component.sourceCode=e,t.component.outputFilePath=r.component.outputFilePath,t.component.relativeFilePathInIndex=r.component
.relativeFilePathInIndex,t.component.componentName=r.component.componentName,t.component.groupName=r.component.groupName})}),_lodash2
["default"].forOwn(e.modules,function(o,a){r=r.then(function(){try{var r=function(){var r=pathResolver.resolveFromModulePerspective
(e,a);return{v:n.generateText(o.generatorScriptPath,r).then(function(e){t.modules[a]={sourceCode:e,outputFilePath:r.modules[a].outputFilePath
,name:r.modules[a].name}})}}();if("object"==typeof r)return r.v}catch(i){throw Error(i)}})}),r=r.then(function(){return n.fileManager
.removeFile(_path2["default"].join(n.projectDirPath,".errors")).then(function(){return t})})})}},{key:"commitGeneration",value:function
(e){var t=this,r=Promise.resolve();return _lodash2["default"].forOwn(e.modules,function(e,n){r=r.then(function(){return t.fileManager
.ensureFilePath(e.outputFilePath).then(function(){return t.fileManager.writeFile(e.outputFilePath,e.sourceCode,!0)})})}),r=r.then
(function(){return t.fileManager.ensureFilePath(e.component.outputFilePath).then(function(){return t.fileManager.writeFile(e.component
.outputFilePath,e.component.sourceCode,!0).then(function(){return t.indexManager.addComponent(e.component.groupName,e.component.
componentName,e.component.relativeFilePathInIndex)})})})}},{key:"generateText",value:function(e,t){var r=this,n=arguments.length
<=2||void 0===arguments[2]?!0:arguments[2];return new Promise(function(o,a){try{var i=require.resolve(e);i&&require.cache[i]&&delete
 require.cache[i];var u=require(e);u(t,function(t){n?!function(){var n=t;try{var i=formatter.formatJsFile(t);o(i)}catch(u){!function
(){var t=_path2["default"].join(r.projectDirPath,".errors","generators",_path2["default"].basename(e));r.fileManager.ensureFilePath
(t).then(function(){r.fileManager.writeFile(t,n)})["catch"](function(e){console.error("Writing bad file. Error: "+e)}),a("Validation
 failed. "+u+". Generator script file path: "+e)}()}}():o(t)},function(t){a("Processing generator's method is failed. Error: "+t
+". File path: "+e)})}catch(s){a("Loading generator's script is failed. Error: "+s+". File path: "+e)}})}}]),e}();exports["default
"]=GeneratorManager,module.exports=exports["default"];
...
```

#### <a name="apidoc.element.react-ui-builder.PathResolver.resolveFromModulePerspective"></a>[function <span class="apidocSignatureSpan">react-ui-builder.PathResolver.</span>resolveFromModulePerspective (e, t)](#apidoc.element.react-ui-builder.PathResolver.resolveFromModulePerspective)
- description and source-code
```javascript
function resolveFromModulePerspective(e, t){var r=_lodash2["default"].clone(e,!0),a=_path2["default"].dirname(e.component.indexFilePath
),o=r.modules[t].outputFilePath,l=_path2["default"].dirname(o);return r.component.relativeFilePath=_path2["default"].relative(l,
r.component.outputFilePath).replace(/\\/g,"/"),r.modules[t].relativeFilePathInIndex=_path2["default"].relative(a,o).replace(/\\/g,"/"),r.component.imports.map(function(e,t){if("../../"===e.source.substr(0,6)){var r=_path2["default"].resolve(a,e.source);e.relativeSource=repairPath(_path2["default"].relative(l,r)).replace(/\\/g,"/")}else e.relativeSource=e.source}),_lodash2["default"].forOwn(r.modules,function(e,t){e.relativeFilePath=repairPath(_path2["default"].relative(l,e.outputFilePath)).replace(/\\/g,"/")}),r}
```
- example usage
```shell
...







"use strict";function _interopRequireWildcard(e){if(e&&e.__esModule)return e;var t={};if(null!=e)for(var r in e)Object.prototype
.hasOwnProperty.call(e,r)&&(t[r]=e[r]);return t["default"]=e,t}function _interopRequireDefault(e){return e&&e.__esModule?e:{"default
":e}}function _classCallCheck(e,t){if(!(e instanceof t))throw new TypeError("Cannot call a class as a function")}Object.defineProperty
(exports,"__esModule",{value:!0});var _createClass=function(){function e(e,t){for(var r=0;r<t.length;r++){var n=t[r];n.enumerable
=n.enumerable||!1,n.configurable=!0,"value"in n&&(n.writable=!0),Object.defineProperty(e,n.key,n)}}return function(t,r,n){return
 r&&e(t.prototype,r),n&&e(t,n),t}}(),_lodash=require("lodash"),_lodash2=_interopRequireDefault(_lodash),_path=require("path"),_path2
=_interopRequireDefault(_path),_FileManagerJs=require("./FileManager.js"),_FileManagerJs2=_interopRequireDefault(_FileManagerJs),
_IndexManagerJs=require("./IndexManager.js"),_IndexManagerJs2=_interopRequireDefault(_IndexManagerJs),_ModelParserJs=require("./
ModelParser.js"),modelParser=_interopRequireWildcard(_ModelParserJs),_PathResolverJs=require("./PathResolver.js"),pathResolver=_interopRequireWildcard
(_PathResolverJs),_FileFormatterJs=require("./FileFormatter.js"),formatter=_interopRequireWildcard(_FileFormatterJs),GeneratorManager
=function(){function e(t){var r=arguments.length<=1||void 0===arguments[1]?".builder":arguments[1],n=arguments.length<=2||void 0
===arguments[2]?"generators":arguments[2],o=arguments.length<=3||void 0===arguments[3]?"src":arguments[3],a=arguments.length<=4||
void 0===arguments[4]?"scripts":arguments[4];_classCallCheck(this,e),this.projectDirPath=t,this.builderDirPath=_path2["default"].
join(t,r),this.generatorsDirPath=_path2["default"].join(this.builderDirPath,n),this.sourceDirPath=_path2["default"].join(this.builderDirPath
,o),this.indexFilePath=_path2["default"].join(this.sourceDirPath,"index.js"),this.scriptsDirName=a,this.fileManager=new _FileManagerJs2
["default"],this.indexManager=new _IndexManagerJs2["default"](this.projectDirPath)}return _createClass(e,[{key:"initGenerator",value
:function(e){var t=this;return this.fileManager.readDirectory(this.generatorsDirPath,["generator.json"]).then(function(r){if(!r.
files||r.files.length<=0)throw Error("Current project does not have a generator, please add a generator.");return r.files.reduce
(function(r,n){return r.then(function(r){return r?r:t.fileManager.readJson(n).then(function(t){return t.name===e?{dirPath:_path2
["default"].dirname(n),filePath:n,config:t}:null})})["catch"](function(e){throw Error(e.message+". Generator file path: "+n)})},
Promise.resolve())})}},{key:"getGeneratorList",value:function(){var e=this;return this.fileManager.readDirectory(this.generatorsDirPath
,["generator.json"]).then(function(t){if(!t.files||t.files.length<=0)throw Error("Current project does not have a generator, please
 add a generator.");var r=[],n=t.files.reduce(function(t,n){return t.then(function(t){return t?t:e.fileManager.readJson(n).then(
function(e){r.push({dirPath:_path2["default"].dirname(n),filePath:n,config:e})})})["catch"](function(e){throw Error(e.message+".
Generator file path: "+n)})},Promise.resolve());return n.then(function(){return r.sort(function(e,t){return e.config.name>t.config
.name?1:e.config.name<t.config.name?-1:0}),r})})}},{key:"createDataObject",value:function(e,t,r){var n=this,o={component:{model:
e,componentName:r.componentName,groupName:r.groupName,indexFilePath:this.indexFilePath}};return this.indexManager.initIndex().then
(function(r){o.component.imports=[];var a=modelParser.getModelComponentMap(e);return r.groups&&_lodash2["default"].forOwn(r.groups
,function(e,t){e.components&&e.components.length>0&&e.components.map(function(e){a[e.name]&&o.component.imports.push({name:e.name
,source:e.source,member:e.member})})}),n.initGenerator(t).then(function(e){if(!e.config)throw Error("Generator "+e.filePath+" is
 not configured properly.");if(!e.config.component)throw Error("Generator "+e.filePath+" configuration does not have component section
.");return o.component.outputFilePath=_path2["default"].join(n.projectDirPath,pathResolver.replaceInPath(e.config.component.destDirPath
,_lodash2["default"].pick(o.component,["componentName","groupName"])),o.component.componentName+"."+e.config.component.fileExtension
),o.component.generatorScriptPath=_path2["default"].join(e.dirPath,n.scriptsDirName,e.config.component.script),o.modules={},e.config
.modules&&e.config.modules.length>0&&e.config.modules.map(function(t,r){var a=_lodash2["default"].pick(o.component,["componentName
","groupName"]);o.modules[t.id]={outputFilePath:_path2["default"].join(n.projectDirPath,pathResolver.replaceInPath(t.destDirPath
,a),pathResolver.replaceInPath(t.name,a)+".js"),name:pathResolver.replaceInPath(t.name,a),generatorScriptPath:_path2["default"].
join(e.dirPath,n.scriptsDirName,t.script),validateJS:t.validateJS}}),o})})}},{key:"doGeneration",value:function(e,t,r){var n=this
;return this.createDataObject(e,t,r).then(function(e){var t={component:{},modules:{}},r=Promise.resolve();return r=r.then(function
(){var r=pathResolver.resolveFromComponentPerspective(e);return n.generateText(r.component.generatorScriptPath,r).then(function(
e){t.component.sourceCode=e,t.component.outputFilePath=r.component.outputFilePath,t.component.relativeFilePathInIndex=r.component
.relativeFilePathInIndex,t.component.componentName=r.component.componentName,t.component.groupName=r.component.groupName})}),_lodash2
["default"].forOwn(e.modules,function(o,a){r=r.then(function(){try{var r=function(){var r=pathResolver.resolveFromModulePerspective
(e,a);return{v:n.generateText(o.generatorScriptPath,r).then(function(e){t.modules[a]={sourceCode:e,outputFilePath:r.modules[a].outputFilePath
,name:r.modules[a].name}})}}();if("object"==typeof r)return r.v}catch(i){throw Error(i)}})}),r=r.then(function(){return n.fileManager
.removeFile(_path2["default"].join(n.projectDirPath,".errors")).then(function(){return t})})})}},{key:"commitGeneration",value:function
(e){var t=this,r=Promise.resolve();return _lodash2["default"].forOwn(e.modules,function(e,n){r=r.then(function(){return t.fileManager
.ensureFilePath(e.outputFilePath).then(function(){return t.fileManager.writeFile(e.outputFilePath,e.sourceCode,!0)})})}),r=r.then
(function(){return t.fileManager.ensureFilePath(e.component.outputFilePath).then(function(){return t.fileManager.writeFile(e.component
.outputFilePath,e.component.sourceCode,!0).then(function(){return t.indexManager.addComponent(e.component.groupName,e.component.
componentName,e.component.relativeFilePathInIndex)})})})}},{key:"generateText",value:function(e,t){var r=this,n=arguments.length
<=2||void 0===arguments[2]?!0:arguments[2];return new Promise(function(o,a){try{var i=require.resolve(e);i&&require.cache[i]&&delete
 require.cache[i];var u=require(e);u(t,function(t){n?!function(){var n=t;try{var i=formatter.formatJsFile(t);o(i)}catch(u){!function
(){var t=_path2["default"].join(r.projectDirPath,".errors","generators",_path2["default"].basename(e));r.fileManager.ensureFilePath
(t).then(function(){r.fileManager.writeFile(t,n)})["catch"](function(e){console.error("Writing bad file. Error: "+e)}),a("Validation
 failed. "+u+". Generator script file path: "+e)}()}}():o(t)},function(t){a("Processing generator's method is failed. Error: "+t
+". File path: "+e)})}catch(s){a("Loading generator's script is failed. Error: "+s+". File path: "+e)}})}}]),e}();exports["default
"]=GeneratorManager,module.exports=exports["default"];
...
```

#### <a name="apidoc.element.react-ui-builder.PathResolver.resolveFromProjectPerspective"></a>[function <span class="apidocSignatureSpan">react-ui-builder.PathResolver.</span>resolveFromProjectPerspective (e)](#apidoc.element.react-ui-builder.PathResolver.resolveFromProjectPerspective)
- description and source-code
```javascript
function resolveFromProjectPerspective(e){var t=_path2["default"].dirname(e.indexFilePath),r=e.outputDirPath;return e.pages.map(
function(e,a){e.imports&&e.imports.length>0&&e.imports.map(function(e,a){if("../../"===e.source.substr(0,6)){var o=_path2["default
"].resolve(t,e.source);e.relativeSource=repairPath(_path2["default"].relative(r,o)).replace(/\\/g,"/")}else e.relativeSource=e.source}),e.resources&&e.resources.requires.map(function(e,a){if("../../"===e.source.substr(0,6)){var o=_path2["default"].resolve(t,e.source);e.relativeSource=repairPath(_path2["default"].relative(r,o)).replace(/\\/g,"/")}else e.relativeSource=e.source})}),e}
```
- example usage
```shell
...







"use strict";function _interopRequireWildcard(e){if(e&&e.__esModule)return e;var t={};if(null!=e)for(var r in e)Object.prototype
.hasOwnProperty.call(e,r)&&(t[r]=e[r]);return t["default"]=e,t}function _interopRequireDefault(e){return e&&e.__esModule?e:{"default
":e}}function _classCallCheck(e,t){if(!(e instanceof t))throw new TypeError("Cannot call a class as a function")}Object.defineProperty
(exports,"__esModule",{value:!0});var _createClass=function(){function e(e,t){for(var r=0;r<t.length;r++){var a=t[r];a.enumerable
=a.enumerable||!1,a.configurable=!0,"value"in a&&(a.writable=!0),Object.defineProperty(e,a.key,a)}}return function(t,r,a){return
 r&&e(t.prototype,r),a&&e(t,a),t}}(),_lodash=require("lodash"),_lodash2=_interopRequireDefault(_lodash),_path=require("path"),_path2
=_interopRequireDefault(_path),_FileManagerJs=require("./FileManager.js"),_FileManagerJs2=_interopRequireDefault(_FileManagerJs),
_IndexManagerJs=require("./IndexManager.js"),_IndexManagerJs2=_interopRequireDefault(_IndexManagerJs),_ModelParserJs=require("./
ModelParser.js"),modelParser=_interopRequireWildcard(_ModelParserJs),_PathResolverJs=require("./PathResolver.js"),pathResolver=_interopRequireWildcard
(_PathResolverJs),_FileFormatterJs=require("./FileFormatter.js"),formatter=_interopRequireWildcard(_FileFormatterJs),_ProjectCompilerJs
=require("./ProjectCompiler.js"),_ProjectCompilerJs2=_interopRequireDefault(_ProjectCompilerJs),configFileName="react-ui-builder
.json",templateDirName="templates",storageDirName=".data",builderDirName=".builder",buildDirName="build",generatorsDirName="generators
",sourceDirName="src",scriptsDirName="scripts",docsDirName="docs",fileConfigName="config.json",indexFileName="index.js",npmPackageFileName
="package.json",previewTemplateDirName="live-preview",LivePreviewManager=function(){function e(t){_classCallCheck(this,e),this.serverDirPath
=t,this.serverConfigFilePath=_path2["default"].join(this.serverDirPath,configFileName),this.serverTemplateDirPath=_path2["default
"].join(this.serverDirPath,templateDirName),this.packageFilePath=_path2["default"].join(this.serverDirPath,npmPackageFileName),this
.storageDirPath=_path2["default"].join(this.serverDirPath,storageDirName),this.previewTemplateDirPath=_path2["default"].join(this
.serverTemplateDirPath,previewTemplateDirName),this.fileManager=new _FileManagerJs2["default"],this.compiler=new _ProjectCompilerJs2
["default"]}return _createClass(e,[{key:"setProjectDirPath",value:function(e){this.projectDirPath=e,this.builderDirPath=_path2["
default"].join(e,builderDirName),this.buildDirPath=_path2["default"].join(this.builderDirPath,buildDirName),this.generatorsDirPath
=_path2["default"].join(this.builderDirPath,generatorsDirName),this.sourceDirPath=_path2["default"].join(this.builderDirPath,sourceDirName
),this.indexFilePath=_path2["default"].join(this.sourceDirPath,indexFileName),this.docsDirPath=_path2["default"].join(this.builderDirPath
,docsDirName),this.scriptsDirName=scriptsDirName,this.configFilePath=_path2["default"].join(this.builderDirPath,fileConfigName)}},{
key:"createPageDataObject",value:function(e,t){var r={model:e,pageName:e.pageName,pageTitle:e.pageTitle,pageMetaInfo:e.pageMetaInfo
,imports:[]},a=modelParser.getModelComponentMap(_lodash2["default"].extend(e,{type:e.pageName}));return t.groups&&_lodash2["default
"].forOwn(t.groups,function(e,t){e.components&&e.components.length>0&&e.components.map(function(e){a[e.name]&&r.imports.push({name
:e.name,source:e.source,member:e.member})})}),r}},{key:"createResourcesDataObject",value:function(e){var t={requires:[]};return
e.requires&&e.requires.length>0&&e.requires.map(function(e){t.requires.push({source:e.source})}),t}},{key:"createProjectDataObject
",value:function(e,t,r){var a=this,i={outputDirPath:_path2["default"].join(this.buildDirPath,"live-preview"),indexFilePath:this.
indexFilePath,pages:[]};if(!(e&&e.pages&&e.pages.length>0))throw Error("Project does not have pages.");return e.pages.map(function
(e,n){if(r[e.pageName]){var u=a.createPageDataObject(e,t);u.isIndexPage=r[e.pageName].isIndexPage,i.pages.push(u)}}),i.resources
=this.createResourcesDataObject(t),i=pathResolver.resolveFromProjectPerspective(i)}},{key:"doGeneration",value:function(e,t,r){var
 a=this,i={pages:[]},n=this.createProjectDataObject(e,t,r),u=_path2["default"].join(this.previewTemplateDirPath,"Page.tpl"),o=_path2
["default"].join(this.previewTemplateDirPath,"Html.tpl"),l=_path2["default"].join(this.previewTemplateDirPath,"Resources.tpl"),s
=null,h=null,p=null;return this.fileManager.readFile(u).then(function(e){s=_lodash2["default"].template(e)}).then(function(){return
 a.fileManager.readFile(o).then(function(e){h=_lodash2["default"].template(e)})}).then(function(){return a.fileManager.readFile(
l).then(function(e){p=_lodash2["default"].template(e)})}).then(function(){return i.outputDirPath=n.outputDirPath,n.pages.map(function
(e,t){var r=e.isIndexPage?"index":e.pageName;i.pages.push({pageOutputFilePath:_path2["default"].join(n.outputDirPath,e.pageName+".
js"),pageSourceCode:s(e),htmlOutputFilePath:_path2["default"].join(n.outputDirPath,r+".html"),htmlSourceCode:h(e),bundleFileName
:e.pageName})}),i.resources={outputFilePath:_path2["default"].join(n.outputDirPath,"resources.js"),sourceCode:p(n.resources),bundleFileName
:"resources.bundle.js"},i})}},{key:"commitGeneration",value:function(e){var t=this,r=_path2["default"].join(this.projectDirPath,"
node_modules"),a=Promise.resolve();return a=a.then(function(){return t.fileManager.removeFile(e.outputDirPath)}),a=a.then(function
(){return t.fileManager.ensureFilePath(e.resources.outputFilePath).then(function(){return t.fileManager.writeFile(e.resources.outputFilePath
,e.resources.sourceCode,!0)}).then(function(){return t.compiler.compileNotOptimized(e.resources.outputFilePath,e.outputDirPath,e
.resources.bundleFileName,r)})}),e.pages.map(function(e,r){a=a.then(function(){return t.fileManager.ensureFilePath(e.pageOutputFilePath
).then(function(){return t.fileManager.writeFile(e.pageOutputFilePath,e.pageSourceCode,!0)}).then(function(){return t.fileManager
.ensureFilePath(e.htmlOutputFilePath)}).then(function(){return t.fileManager.writeFile(e.htmlOutputFilePath,e.htmlSourceCode,!1)})})}),
a=a.then(function(){var a={};return e.pages.map(function(e,t){a[e.bundleFileName]=e.pageOutputFilePath}),t.compiler.compileNotOptimized
(a,e.outputDirPath,"[name].bundle.js",r,!0)}),a=a.then(function(){return"live-preview/index.html"})}}]),e}();exports["default"]=
LivePreviewManager,module.exports=exports["default"];
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
