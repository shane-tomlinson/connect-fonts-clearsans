# connect-fonts-clearsans

Clear Sans fontpack for [connect-fonts](https://github.com/shane-tomlinson/connect-fonts).

## Usage

1. Include [connect-fonts](https://github.com/shane-tomlinson/connect-fonts) in a node module.
```js
const font_middleware = require("connect-fonts");
```

2. Include the font packs that you want to serve.
```js
const font_pack  = require("connect-fonts-clearsans");
```

3. Add a middleware by calling the `setup` function.
```js
    app.use(font_middleware.setup({
      fonts: [ font_pack ],
      allow_origin: "https://exampledomain.com"
    }));
```

4. Add a link tag to include the font CSS.
```html
<link href="/clearsans-bold/fonts.css" type="text/css" rel="stylesheet"/ >
```

Multiple fonts from the family can be included by using a comma separated list of fonts:
```html
<link href="/clearsans-bold,clearsans-bolditalic,clearsans-italic,clearsans-light,clearsans-medium,clearsans-mediumitalic,clearsans-regular,clearsans-thin/fonts.css" type="text/css" rel="stylesheet"/ >
```

Available fonts:
* clearsans-bold
* clearsans-bolditalic
* clearsans-italic
* clearsans-light
* clearsans-medium
* clearsans-mediumitalic
* clearsans-regular
* clearsans-thin

Locale-optimised font sets can be served by specifying the locale in the fonts.css URL.
```html
<link href="/latin/clearsans-bold/fonts.css" type="text/css" rel="stylesheet"/ >
```

Available subsets:
* latin

5. Set your CSS up to use the new font by using the "Clear Sans" font-family.
```
    body {
      font-family: 'Clear Sans', 'sans-serif', 'serif';
    }
```

## Font Info
Clear Sans

* Copyright: Font software Copyright © 2012 Intel Corporation. Licensed under the Apache License, Version 2.0.  http://www.apache.org/licenses/LICENSE-2.0
* Designer URL: http://01.org/clearsans
* Vendor: Intel Corporation
* Vendor URL: http://01.org/

## Development Info
* Homepage: https://github.com/shane-tomlinson/connect-fonts-clearsans
* Repo: https://github.com/shane-tomlinson/connect-fonts-clearsans.git
* Bugs: https://github.com/shane-tomlinson/connect-fonts-clearsans/issues

## Author
* Shane Tomlinson
* shane@shanetomlinson.com
* stomlinson@mozilla.com
* set117@yahoo.com
* https://shanetomlinson.com
* https://github.com/shane-tomlinson
* @shane_tomlinson


## License

Software: Licenced under version 2.0 of the MPL

  https://www.mozilla.org/MPL/

Fonts: Licensed under version 2.0 of the Apache

  http://www.apache.org/licenses/LICENSE-2.0

