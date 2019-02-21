# tslint-line-before-class-property
[![npm version](https://badge.fury.io/js/tslint-line-before-class-property.svg)](https://github.com/toxity/tslint-line-before-class-property)
[![CircleCI](https://travis-ci.org/toxity/tslint-line-before-class-property.svg?branch=master)](https://github.com/toxity/tslint-line-before-class-property)

Custom rule for TSLint to assure that each class property has new line before declaration

## Install
```bash
npm install --save-dev tslint-line-before-class-property
```

## Configuration
Update `tslint.json` file and add new rules directory with new rule itself
```json
{
    "rulesDirectory": [
      "tslint-line-before-class-property"
    ],
    "rules": {
      "tslint-line-before-class-property": true
    }
}
```

## Example
```javascript
// Bad
class Name {
    public boolean: boolean;
    public string: string;
    public array: Array<string>;
}

// Good
class Name {

    public boolean: boolean;

    public string: string;

    public array: Array<string>;
}
```

