<!--

@license Apache-2.0

Copyright (c) 2021 The Stdlib Authors.

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

   http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.

-->

# add

[![NPM version][npm-image]][npm-url] [![Build Status][test-image]][test-url] [![Coverage Status][coverage-image]][coverage-url] <!-- [![dependencies][dependencies-image]][dependencies-url] -->

> Compute the sum of two double-precision floating-point numbers.

<!-- Section to include introductory text. Make sure to keep an empty line after the intro `section` element and another before the `/section` close. -->

<section class="intro">

</section>

<!-- /.intro -->

<!-- Package usage documentation. -->

<section class="installation">

## Installation

```bash
npm install @stdlib/math-base-ops-add
```

</section>

<section class="usage">

## Usage

```javascript
var add = require( '@stdlib/math-base-ops-add' );
```

#### add( x, y )

Computes the sum of two double-precision floating-point numbers.

```javascript
var v = add( -1.0, 5.0 );
// returns 4.0

v = add( 2.0, 5.0 );
// returns 7.0

v = add( 0.0, 5.0 );
// returns 5.0

v = add( -0.0, 0.0 );
// returns 0.0

v = add( NaN, NaN );
// returns NaN
```

</section>

<!-- /.usage -->

<!-- Package usage notes. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->

<section class="notes">

</section>

<!-- /.notes -->

<!-- Package usage examples. -->

<section class="examples">

## Examples

<!-- eslint no-undef: "error" -->

```javascript
var rand = require( '@stdlib/random-base-discrete-uniform' );
var add = require( '@stdlib/math-base-ops-add' );

var x;
var y;
var i;

for ( i = 0; i < 100; i++ ) {
    x = rand( -50, 50 );
    y = rand( -50, 50 );
    console.log( '%d + %d = %d', x, y, add( x, y ) );
}
```

</section>

<!-- /.examples -->

<!-- C interface documentation. -->

* * *

<section class="c">

## C APIs

<!-- Section to include introductory text. Make sure to keep an empty line after the intro `section` element and another before the `/section` close. -->

<section class="intro">

</section>

<!-- /.intro -->

<!-- C usage documentation. -->

<section class="installation">

## Installation

```bash
npm install @stdlib/math-base-ops-add
```

</section>

<section class="usage">

### Usage

```c
#include "stdlib/math/base/ops/add.h"
```

#### stdlib_base_add( x, y )

Computes the sum of two double-precision floating-point numbers.

```c
double v = stdlib_base_add( -5.0, 2.0 );
// returns -3.0
```

The function accepts the following arguments:

-   **x**: `[in] double` first input value.
-   **y**: `[in] double` second input value.

```c
double stdlib_base_add( const double x, const double y );
```

</section>

<!-- /.usage -->

<!-- C API usage notes. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->

<section class="notes">

</section>

<!-- /.notes -->

<!-- C API usage examples. -->

<section class="examples">

### Examples

```c
#include "stdlib/math/base/ops/add.h"
#include <stdio.h>

int main() {
    double x[] = { 3.14, -3.14, 0.0, 0.0/0.0 };
    double y[] = { 3.14, -3.14, -0.0, 0.0/0.0 };

    double z;
    int i;
    for ( i = 0; i < 4; i++ ) {
        z = stdlib_base_add( x[ i ], y[ i ] );
        printf( "%lf + %lf = %lf\n", x[ i ], y[ i ], z );
    }
}
```

</section>

<!-- /.examples -->

</section>

<!-- /.c -->

<!-- Section for related `stdlib` packages. Do not manually edit this section, as it is automatically populated. -->

<section class="related">

</section>

<!-- /.related -->

<!-- Section for all links. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->


<section class="main-repo" >

* * *

## Notice

This package is part of [stdlib][stdlib], a standard library for JavaScript and Node.js, with an emphasis on numerical and scientific computing. The library provides a collection of robust, high performance libraries for mathematics, statistics, streams, utilities, and more.

For more information on the project, filing bug reports and feature requests, and guidance on how to develop [stdlib][stdlib], see the main project [repository][stdlib].

#### Community

[![Chat][chat-image]][chat-url]

---

## License

See [LICENSE][stdlib-license].


## Copyright

Copyright &copy; 2016-2021. The Stdlib [Authors][stdlib-authors].

</section>

<!-- /.stdlib -->

<!-- Section for all links. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->

<section class="links">

[npm-image]: http://img.shields.io/npm/v/@stdlib/math-base-ops-add.svg
[npm-url]: https://npmjs.org/package/@stdlib/math-base-ops-add

[test-image]: https://github.com/stdlib-js/math-base-ops-add/actions/workflows/test.yml/badge.svg
[test-url]: https://github.com/stdlib-js/math-base-ops-add/actions/workflows/test.yml

[coverage-image]: https://img.shields.io/codecov/c/github/stdlib-js/math-base-ops-add/main.svg
[coverage-url]: https://codecov.io/github/stdlib-js/math-base-ops-add?branch=main

<!--

[dependencies-image]: https://img.shields.io/david/stdlib-js/math-base-ops-add.svg
[dependencies-url]: https://david-dm.org/stdlib-js/math-base-ops-add/main

-->

[chat-image]: https://img.shields.io/gitter/room/stdlib-js/stdlib.svg
[chat-url]: https://gitter.im/stdlib-js/stdlib/

[stdlib]: https://github.com/stdlib-js/stdlib

[stdlib-authors]: https://github.com/stdlib-js/stdlib/graphs/contributors

[stdlib-license]: https://raw.githubusercontent.com/stdlib-js/math-base-ops-add/main/LICENSE

</section>

<!-- /.links -->
