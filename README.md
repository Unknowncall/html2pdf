
# HTML2PDF-TS

#### NPM badges

  

<!-- [START badges] -->

[![NPM html2pdf-ts package](https://img.shields.io/npm/v/html2pdf-ts.svg)](https://npmjs.org/package/html2pdf-ts)

[![npm downloads](https://img.shields.io/npm/dm/html2pdf-ts.svg?maxAge=604800)](https://npm-stat.com/charts.html?package=html2pdf-ts&from=2017-01-1)

[![npm downloads](https://img.shields.io/npm/dt/html2pdf-ts.svg?maxAge=604800)](https://npm-stat.com/charts.html?package=html2pdf-ts&from=2017-01-1)

<!-- [END badges] -->

  

# Description

Simple lib to convert HTML to PDF, using puppeteer.


# Install

  

```javascript
npm i html2pdf-ts
```

  

```javacript
yarn add html2pdf-ts
```

  

# Example

  To execute an example, just run:

```javascript
npm  run  start
```

ou 


```javascript
yarn start
```

Using the package:

```javascript
const fs = require('fs');
const { html2pdf } = require('html2pdf-ts');

const example = async () => {

    const html = fs.readFileSync('./page.html', 'utf-8');
    const options = {
        format: 'A4',
    };

    await html2pdf.createPDF(html, `./lotr.pdf`, options);
    console.log('PDF Generated...');
};

example();
```

You can read a html file and pass the content to create the PDF, or you can pass a pure HTML as param.
  

# License

Released under the MIT License.