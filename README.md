# jquery.inputfilter

jQuery plugin for adding filters to forms input and textarea, like numeric input only.

## Installation

```bash
npm install jquery.inputfilter
```

## Usage

Include _jquery.inputfilter.js_ after jQuery (1.7+) and set it to the objects you want to filter

```js
import "jquery.inputfilter";

// Standard options
$("input, textarea").inputfilter();
// Set options
const options = { allowNumeric: true, allowText: true };
$("input, textarea").inputfilter(options);
```

## Options

```js
const options = {
  allowNumeric: true, // is numbers allowed [0-9]
  allowText: false, // is text allowed [a-z|A-Z]
  allowEnter: true, // is Enter allowed
  allowCustom: [], // Array of chars to allow
  regex: null, // Regular expression of allowed chars
  maxLength: null, // Numeric value representing the maximum number of chars permitted
  actionLog: false, // Log actions
};
```

## License

Copyright &copy; 2015 Anders Fj&auml;llstr&ouml;m, licensed under the MIT License
