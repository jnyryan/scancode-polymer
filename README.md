#scancode-element

polymer element to display quickread codes and barcodes

## Demo

You'll find a live working demo of scancode on [heroku](http://scancode-demo.herokuapp.com)

## Installation

``` bash
bower install scancode
```

## Usage

``` html
<!DOCTYPE html>
<html lang="en">
  <head>
    <script src="bower_components/webcomponentsjs/webcomponents-lite.min.js"></script>
    <link rel="import" href="bower_components/scancode/scancode.html">
  </head>
  <body>
    <scan-code id="my_qrcode" type="qrcode" data="http://www.johnryan.io" height="100" width="100"></scan-code>
    <scan-code id="my_barcode" type="barcode" format="ean8" data="12345678" height="40" width="1"></scan-code>
  </body>
</html>

```

## API
The following attributes are available

|attribute| value|description|
| ------------- |:-------------| :-----|
|type|  barcode  |  renders a BarCode |
||  qrcode  |  renders a QRCode |
|format <BR/> (required for barcode only)| codabar |  * e.g. 12345678901234567890|
|| code11 (code 11)|  * e.g. 12345678901234567890|
|| code39 (code 39)|  * e.g. abc12345678901234567890|
|| code93 (code 93)|  * e.g. abc12345678901234567890|
|| code128 (code 128)|  * e.g. 12345678901234567890|
|| ean8 (ean 8)|  * e.g. 1234567|
|| ean13 (ean 13)|  * e.g. 1234567890128|
|| std25 (standard 2 of 5 - industrial 2 of 5)|  * e.g. 1234, 1234567891234567812345678|
|| int25 (interleaved 2 of 5)|  * e.g. 1234567|
|| msi|  * e.g. 12345678901234567890|
|| datamatrix (ASCII + extended)|  * e.g. AABC12345678901234567890|
|height|number| specifies the height of the scancode  |  
|width|number|specifies the width of the scancode|
|colordark <BR/> (qrcode only)|hex color value|* e.g. #4747FF <br/> default: #000000|
|colorlight <BR/> (qrcode only)|hex color value|* e.g. #FF9900 <br/> default: #ffffff|



## Contributing

If you have any ideas on features or bug fixes you'd like in this project then why not consider contributing! It's as easy as :

1. Fork the repository!
2. Create your feature branch: `git checkout -b my-new-feature`
3. Commit your changes: `git commit -m 'Add some feature'`
4. Push to the branch: `git push origin my-new-feature`
5. Submit a pull request

## History

For detailed changelog, check [Releases](https://github.com/jnyryan/scancode-polymer/releases).


## References

The following came in handy during this project

- [The Polymer Project](https://www.polymer-project.org/0.5/)
- [QRCode Js](https://github.com/janantala/qrcode.js)
- [Barcode Creator](http://barcode-coder.com/en/barcode-jquery-plugin-201.html)
- [qrcodejs sample](http://davidshimjs.github.io/qrcodejs/)

### Tagging

``` bash
git tag -a v0.0.7 -m "Tagging v0.0.7"
```
