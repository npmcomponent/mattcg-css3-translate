*This repository is a mirror of the [component](http://component.io) module [mattcg/css3-translate](http://github.com/mattcg/css3-translate). It has been modified to work with NPM+Browserify. You can install it using the command `npm install npmcomponent/mattcg-css3-translate`. Please do not open issues or send pull requests against this repo. If you have issues with this repo, report it to [npmcomponent](https://github.com/airportyh/npmcomponent).*
# CSS3 translate #

A tiny (900 bytes minified, 470 bytes gziped), functional CSS3 translation transforms API for JavaScript. Supports all browsers supporting CSS3 Transforms. Check out the [support grid](http://caniuse.com/transforms2d).

3D transforms - `translate.z` and `translate.d3` - have a [separate support grid](http://caniuse.com/transforms3d).

## Install ##

```bash
git clone https://github.com/mattcg/css3-translate.git
cd css3-translate/
make
cp build/translate.min.js /path/to/my-project/js/
```

Alternatively, use [Component](https://github.com/component/component), [Bower](http://bower.io/) or [npm](https://npmjs.org/) to install to your project as a dependency.

## API ##

For all translation methods, if a length does not include units, `px` will be used.

### translate(el, tx, ty) ###

Apply a `translate(tx, ty)` CSS transform to the given element, moving the position of the element on the plane.

If missing, `ty` is assumed to be equal to `tx`: `translate(el, 2)` means `translate(el, 2, 2)`.

### translate.x(el, tx) ###

Apply a `translateX(tx)` CSS transform to the given element, moving the element horizontally on the plane.

### translate.y(el, ty) ###

Apply a `translateY(ty)` CSS transform to the given element, moving the element vertically on the plane.

### translate.z(el, tz) ###

Apply a `translateZ(tz)` CSS transform to the given element, moving the element along the z-axis of the 3D space.

### translate.d3(el, tx, ty, tz) or translate\['3d'\](tx, ty, tz) ###

Apply a `translate3d(tx, ty, tz)` CSS transform to the given element, moving the position of the element in the 3D space.

### translate.rule() ###

Get the browser-specific transform rule e.g. 'webkitTransform' or 'transform'.

## License ##

Copyright © 2013 [Matthew Caruana Galizia](http://twitter.com/mcaruanagalizia), licensed under an [MIT license](http://mattcg.mit-license.org/).
