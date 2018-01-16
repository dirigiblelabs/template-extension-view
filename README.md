# Template V3 - Extension IDE View

[![Eclipse License](http://img.shields.io/badge/license-Eclipse-brightgreen.svg)](LICENSE)
[![GitHub contributors](https://img.shields.io/github/contributors/dirigiblelabs/template-v3-extension-view.svg)](https://github.com/dirigiblelabs/template-v3-extension-view/graphs/contributors)


## Overview

1. IDE view
```html
  ...
<body>
  <h1>Hello World!</h1>
</body>
  ...
```
2. View extension
```javascript
{
  "module": "{{view-template-definition-location}}",
  "extensionPoint": "ide-view",
  "description": "{{view-description}"
}
```

3. View template definition
```javascript
exports.getView = function() {
  return {
    "id": "{{view-id}}",
    "name": "{{view-name}}",
    "factory": "frame",
    "region": "center-bottom",
    "label": "{{view-label}}",
    "link": "{{view-page-location}}"
  };
};
```

## License

This project is copyrighted by [SAP SE](http://www.sap.com/) and is available under the [Eclipse Public License v 1.0](https://www.eclipse.org/legal/epl-v10.html). See [LICENSE](LICENSE) and [NOTICE.txt](NOTICE.txt) for further details.
