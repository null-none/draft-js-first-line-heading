# draft-js-first-line-heading
The plugin force block style on first line for a heading/title.

## Install

```bash
$ npm install draft-js-first-line-heading
```

## Usage

```js
import createFirstLineHeadingPLugin from 'draft-js-first-line-heading';
const firstLineHeading = createFirstLineHeadingPLugin();

...

const plugins = [firstLineHeading];

let lines = this.state.story.getCurrentContent().getPlainText().split('\n');
let title = lines[0];
lines.shift();
let body = lines.join('\n');

console.log(title, body)

...

```

## License
MIT
