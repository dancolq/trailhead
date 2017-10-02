## Linter For Lightning Components

Example:

$ heroku lightning:lint ./path/to/be/linted/



Option | Description
--- | --- 
```-i, --ignore IGNORE``` | Pattern to ignore some folders. Example: --ignore **/foo/**
```-j, --json``` | Output JSON to facilitate integration with other tools. Defaults to standard text output format. Example: --json
```--config CONFIG``` | Path to a custom ESLint configuration. Only code styles rules will be picked up, the rest will be ignored. Example: --config path/to/.eslintrc
```--exit``` | Exit with zero code 1 when there are lint issues. Defaults to exit without error code. Example: --exit
```--files FILES``` | Pattern to include specific files. Defaults to all .js files. Example: --files **/*Controller.js
```--verbose``` | Report warnings in addition to errors. Defaults to reporting only errors. Example: --verbose
