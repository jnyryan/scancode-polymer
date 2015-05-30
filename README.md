#barcode-element-polymer

polymer element to display quickread codes and barcodes

## Demo

You'll find a live working demo of scancode on [heroku](http://scancode-demo.herokuapp.com)

## Installation

``` bash
bower install scancode
```

## Usage

``` html
<scan-code id="my_qrcode" type="qrcode" data="http://www.johnryan.io" height="100" width="100"></scan-code>

<scan-code id="my_qrcode" type="barcode" format="12345678" data="12345678" height="100" width="100"></scan-code>

```

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
git tag -a v0.0.5 -m "Tagging v0.0.5"
```
