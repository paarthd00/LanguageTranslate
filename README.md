# LanguageTranslate

## Installation

```bash
npm install @google-cloud/translate
```

## Initialization

```javascript
const { Translate } = require('@google-cloud/translate').v2;
const translate = new Translate();
```

## Translate Text

```javascript
const text = 'Hello Friends!';
const target = 'hi';

async function translateText() {
    const [translations] = await translate.translate(text, target);
    console.log('Translations:', translations);
}

translateText();
```

Customize the `text` and `target` variables as needed for seamless text translation with the Google Cloud Translate API in JavaScript.
