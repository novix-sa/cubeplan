# Function List
You can use any of numpy’s or scipy’s many [ufunc](http://docs.scipy.org/doc/numpy/reference/ufuncs.html) functions directly on a DataArray:
There are currently more than [60 universal functions](https://docs.scipy.org/doc/numpy/reference/ufuncs.html#math-operations) defined in [`numpy`](https://docs.scipy.org/doc/numpy/reference/index.html#module-numpy "numpy") on one or more types, covering a wide variety of operations.

## **Math operations**[](https://docs.scipy.org/doc/numpy/reference/ufuncs.html#math-operations "Permalink to this headline")

[`add`](https://docs.scipy.org/doc/numpy/reference/generated/numpy.add.html#numpy.add "numpy.add")(x1, x2, /[, out, where, casting, order, …])
Add arguments element-wise.

[`subtract`](https://docs.scipy.org/doc/numpy/reference/generated/numpy.subtract.html#numpy.subtract "numpy.subtract")(x1, x2, /[, out, where, casting, …])
Subtract arguments, element-wise.

[`multiply`](https://docs.scipy.org/doc/numpy/reference/generated/numpy.multiply.html#numpy.multiply "numpy.multiply")(x1, x2, /[, out, where, casting, …])
Multiply arguments element-wise.

[`divide`](https://docs.scipy.org/doc/numpy/reference/generated/numpy.divide.html#numpy.divide "numpy.divide")(x1, x2, /[, out, where, casting, …])
Returns a true division of the inputs, element-wise.

[`logaddexp`](https://docs.scipy.org/doc/numpy/reference/generated/numpy.logaddexp.html#numpy.logaddexp "numpy.logaddexp")(x1, x2, /[, out, where, casting, …])
Logarithm of the sum of exponentiations of the inputs.

[`logaddexp2`](https://docs.scipy.org/doc/numpy/reference/generated/numpy.logaddexp2.html#numpy.logaddexp2 "numpy.logaddexp2")(x1, x2, /[, out, where, casting, …])
Logarithm of the sum of exponentiations of the inputs in base-2.

[`true_divide`](https://docs.scipy.org/doc/numpy/reference/generated/numpy.true_divide.html#numpy.true_divide "numpy.true_divide")(x1, x2, /[, out, where, …])
Returns a true division of the inputs, element-wise.

[`floor_divide`](https://docs.scipy.org/doc/numpy/reference/generated/numpy.floor_divide.html#numpy.floor_divide "numpy.floor_divide")(x1, x2, /[, out, where, …])
Return the largest integer smaller or equal to the division of the inputs.

[`negative`](https://docs.scipy.org/doc/numpy/reference/generated/numpy.negative.html#numpy.negative "numpy.negative")(x, /[, out, where, casting, order, …])
Numerical negative, element-wise.

[`positive`](https://docs.scipy.org/doc/numpy/reference/generated/numpy.positive.html#numpy.positive "numpy.positive")(x, /[, out, where, casting, order, …])
Numerical positive, element-wise.

[`power`](https://docs.scipy.org/doc/numpy/reference/generated/numpy.power.html#numpy.power "numpy.power")(x1, x2, /[, out, where, casting, …])
First array elements raised to powers from second array, element-wise.

[`remainder`](https://docs.scipy.org/doc/numpy/reference/generated/numpy.remainder.html#numpy.remainder "numpy.remainder")(x1, x2, /[, out, where, casting, …])
Return element-wise remainder of division.

[`mod`](https://docs.scipy.org/doc/numpy/reference/generated/numpy.mod.html#numpy.mod "numpy.mod")(x1, x2, /[, out, where, casting, order, …])
Return element-wise remainder of division.

[`fmod`](https://docs.scipy.org/doc/numpy/reference/generated/numpy.fmod.html#numpy.fmod "numpy.fmod")(x1, x2, /[, out, where, casting, …])
Return the element-wise remainder of division.

[`divmod`](https://docs.scipy.org/doc/numpy/reference/generated/numpy.divmod.html#numpy.divmod "numpy.divmod")(x1, x2[, out1, out2], / [[, out, …])
Return element-wise quotient and remainder simultaneously.

[`absolute`](https://docs.scipy.org/doc/numpy/reference/generated/numpy.absolute.html#numpy.absolute "numpy.absolute")(x, /[, out, where, casting, order, …])
Calculate the absolute value element-wise.

[`fabs`](https://docs.scipy.org/doc/numpy/reference/generated/numpy.fabs.html#numpy.fabs "numpy.fabs")(x, /[, out, where, casting, order, …])

Compute the absolute values element-wise.

[`rint`](https://docs.scipy.org/doc/numpy/reference/generated/numpy.rint.html#numpy.rint "numpy.rint")(x, /[, out, where, casting, order, …])
Round elements of the array to the nearest integer.

[`sign`](https://docs.scipy.org/doc/numpy/reference/generated/numpy.sign.html#numpy.sign "numpy.sign")(x, /[, out, where, casting, order, …])
Returns an element-wise indication of the sign of a number.

[`heaviside`](https://docs.scipy.org/doc/numpy/reference/generated/numpy.heaviside.html#numpy.heaviside "numpy.heaviside")(x1, x2, /[, out, where, casting, …])
Compute the Heaviside step function.

[`conj`](https://docs.scipy.org/doc/numpy/reference/generated/numpy.conj.html#numpy.conj "numpy.conj")(x, /[, out, where, casting, order, …])
Return the complex conjugate, element-wise.

[`exp`](https://docs.scipy.org/doc/numpy/reference/generated/numpy.exp.html#numpy.exp "numpy.exp")(x, /[, out, where, casting, order, …])
Calculate the exponential of all elements in the input array.

[`exp2`](https://docs.scipy.org/doc/numpy/reference/generated/numpy.exp2.html#numpy.exp2 "numpy.exp2")(x, /[, out, where, casting, order, …])
Calculate  _2**p_  for all  _p_  in the input array.

[`log`](https://docs.scipy.org/doc/numpy/reference/generated/numpy.log.html#numpy.log "numpy.log")(x, /[, out, where, casting, order, …])
Natural logarithm, element-wise.

[`log2`](https://docs.scipy.org/doc/numpy/reference/generated/numpy.log2.html#numpy.log2 "numpy.log2")(x, /[, out, where, casting, order, …])
Base-2 logarithm of  _x_.

[`log10`](https://docs.scipy.org/doc/numpy/reference/generated/numpy.log10.html#numpy.log10 "numpy.log10")(x, /[, out, where, casting, order, …])
Return the base 10 logarithm of the input array, element-wise.

[`expm1`](https://docs.scipy.org/doc/numpy/reference/generated/numpy.expm1.html#numpy.expm1 "numpy.expm1")(x, /[, out, where, casting, order, …])
Calculate  `exp(x)  -  1`  for all elements in the array.

[`log1p`](https://docs.scipy.org/doc/numpy/reference/generated/numpy.log1p.html#numpy.log1p "numpy.log1p")(x, /[, out, where, casting, order, …])

Return the natural logarithm of one plus the input array, element-wise.

[`sqrt`](https://docs.scipy.org/doc/numpy/reference/generated/numpy.sqrt.html#numpy.sqrt "numpy.sqrt")(x, /[, out, where, casting, order, …])
Return the non-negative square-root of an array, element-wise.

[`square`](https://docs.scipy.org/doc/numpy/reference/generated/numpy.square.html#numpy.square "numpy.square")(x, /[, out, where, casting, order, …])
Return the element-wise square of the input.

[`cbrt`](https://docs.scipy.org/doc/numpy/reference/generated/numpy.cbrt.html#numpy.cbrt "numpy.cbrt")(x, /[, out, where, casting, order, …])
Return the cube-root of an array, element-wise.

[`reciprocal`](https://docs.scipy.org/doc/numpy/reference/generated/numpy.reciprocal.html#numpy.reciprocal "numpy.reciprocal")(x, /[, out, where, casting, …])
Return the reciprocal of the argument, element-wise.

[`gcd`](https://docs.scipy.org/doc/numpy/reference/generated/numpy.gcd.html#numpy.gcd "numpy.gcd")(x1, x2, /[, out, where, casting, order, …])
Returns the greatest common divisor of  `|x1|`  and  `|x2|`

[`lcm`](https://docs.scipy.org/doc/numpy/reference/generated/numpy.lcm.html#numpy.lcm "numpy.lcm")(x1, x2, /[, out, where, casting, order, …])
Returns the lowest common multiple of  `|x1|`  and  `|x2|`

Tip

The optional output arguments can be used to help you save memory for large calculations. If your arrays are large, complicated expressions can take longer than absolutely necessary due to the creation and (later) destruction of temporary calculation spaces. For example, the expression  `G  =  a  *  b  +  c`  is equivalent to`t1  =  A  *  B;  G  =  T1  +  C;  del  t1`. It will be more quickly executed as  `G  =  A  *  B;  add(G,  C,  G)`  which is the same as  `G  =  A  *  B;  G  +=  C`.

### Trigonometric functions[](https://docs.scipy.org/doc/numpy/reference/ufuncs.html#trigonometric-functions "Permalink to this headline")

All trigonometric functions use radians when an angle is called for. The ratio of degrees to radians is  ![180^{\circ}/\pi.](https://docs.scipy.org/doc/numpy/_images/math/cb6057b10a288dd8a2d8e534202e3b19f9f683fa.svg)

[`sin`](https://docs.scipy.org/doc/numpy/reference/generated/numpy.sin.html#numpy.sin "numpy.sin")(x, /[, out, where, casting, order, …])
Trigonometric sine, element-wise.

[`cos`](https://docs.scipy.org/doc/numpy/reference/generated/numpy.cos.html#numpy.cos "numpy.cos")(x, /[, out, where, casting, order, …])
Cosine element-wise.

[`tan`](https://docs.scipy.org/doc/numpy/reference/generated/numpy.tan.html#numpy.tan "numpy.tan")(x, /[, out, where, casting, order, …])
Compute tangent element-wise.

[`arcsin`](https://docs.scipy.org/doc/numpy/reference/generated/numpy.arcsin.html#numpy.arcsin "numpy.arcsin")(x, /[, out, where, casting, order, …])
Inverse sine, element-wise.

[`arccos`](https://docs.scipy.org/doc/numpy/reference/generated/numpy.arccos.html#numpy.arccos "numpy.arccos")(x, /[, out, where, casting, order, …])
Trigonometric inverse cosine, element-wise.

[`arctan`](https://docs.scipy.org/doc/numpy/reference/generated/numpy.arctan.html#numpy.arctan "numpy.arctan")(x, /[, out, where, casting, order, …])
Trigonometric inverse tangent, element-wise.

[`arctan2`](https://docs.scipy.org/doc/numpy/reference/generated/numpy.arctan2.html#numpy.arctan2 "numpy.arctan2")(x1, x2, /[, out, where, casting, …])
Element-wise arc tangent of  `x1/x2`  choosing the quadrant correctly.

[`hypot`](https://docs.scipy.org/doc/numpy/reference/generated/numpy.hypot.html#numpy.hypot "numpy.hypot")(x1, x2, /[, out, where, casting, …])
Given the “legs” of a right triangle, return its hypotenuse.

[`sinh`](https://docs.scipy.org/doc/numpy/reference/generated/numpy.sinh.html#numpy.sinh "numpy.sinh")(x, /[, out, where, casting, order, …])
Hyperbolic sine, element-wise.

[`cosh`](https://docs.scipy.org/doc/numpy/reference/generated/numpy.cosh.html#numpy.cosh "numpy.cosh")(x, /[, out, where, casting, order, …])
Hyperbolic cosine, element-wise.

[`tanh`](https://docs.scipy.org/doc/numpy/reference/generated/numpy.tanh.html#numpy.tanh "numpy.tanh")(x, /[, out, where, casting, order, …])
Compute hyperbolic tangent element-wise.

[`arcsinh`](https://docs.scipy.org/doc/numpy/reference/generated/numpy.arcsinh.html#numpy.arcsinh "numpy.arcsinh")(x, /[, out, where, casting, order, …])

Inverse hyperbolic sine element-wise.

[`arccosh`](https://docs.scipy.org/doc/numpy/reference/generated/numpy.arccosh.html#numpy.arccosh "numpy.arccosh")(x, /[, out, where, casting, order, …])
Inverse hyperbolic cosine, element-wise.

[`arctanh`](https://docs.scipy.org/doc/numpy/reference/generated/numpy.arctanh.html#numpy.arctanh "numpy.arctanh")(x, /[, out, where, casting, order, …])
Inverse hyperbolic tangent element-wise.

[`deg2rad`](https://docs.scipy.org/doc/numpy/reference/generated/numpy.deg2rad.html#numpy.deg2rad "numpy.deg2rad")(x, /[, out, where, casting, order, …])
Convert angles from degrees to radians.

[`rad2deg`](https://docs.scipy.org/doc/numpy/reference/generated/numpy.rad2deg.html#numpy.rad2deg "numpy.rad2deg")(x, /[, out, where, casting, order, …])
Convert angles from radians to degrees.

### Bit-twiddling functions[](https://docs.scipy.org/doc/numpy/reference/ufuncs.html#bit-twiddling-functions "Permalink to this headline")

These function all require integer arguments and they manipulate the bit-pattern of those arguments.

[`bitwise_and`](https://docs.scipy.org/doc/numpy/reference/generated/numpy.bitwise_and.html#numpy.bitwise_and "numpy.bitwise_and")(x1, x2, /[, out, where, …])
Compute the bit-wise AND of two arrays element-wise.

[`bitwise_or`](https://docs.scipy.org/doc/numpy/reference/generated/numpy.bitwise_or.html#numpy.bitwise_or "numpy.bitwise_or")(x1, x2, /[, out, where, casting, …])
Compute the bit-wise OR of two arrays element-wise.

[`bitwise_xor`](https://docs.scipy.org/doc/numpy/reference/generated/numpy.bitwise_xor.html#numpy.bitwise_xor "numpy.bitwise_xor")(x1, x2, /[, out, where, …])
Compute the bit-wise XOR of two arrays element-wise.

[`invert`](https://docs.scipy.org/doc/numpy/reference/generated/numpy.invert.html#numpy.invert "numpy.invert")(x, /[, out, where, casting, order, …])
Compute bit-wise inversion, or bit-wise NOT, element-wise.

[`left_shift`](https://docs.scipy.org/doc/numpy/reference/generated/numpy.left_shift.html#numpy.left_shift "numpy.left_shift")(x1, x2, /[, out, where, casting, …])
Shift the bits of an integer to the left.

[`right_shift`](https://docs.scipy.org/doc/numpy/reference/generated/numpy.right_shift.html#numpy.right_shift "numpy.right_shift")(x1, x2, /[, out, where, …])

Shift the bits of an integer to the right.

### Comparison functions[](https://docs.scipy.org/doc/numpy/reference/ufuncs.html#comparison-functions "Permalink to this headline")

[`greater`](https://docs.scipy.org/doc/numpy/reference/generated/numpy.greater.html#numpy.greater "numpy.greater")(x1, x2, /[, out, where, casting, …])
Return the truth value of (x1 > x2) element-wise.

[`greater_equal`](https://docs.scipy.org/doc/numpy/reference/generated/numpy.greater_equal.html#numpy.greater_equal "numpy.greater_equal")(x1, x2, /[, out, where, …])
Return the truth value of (x1 >= x2) element-wise.

[`less`](https://docs.scipy.org/doc/numpy/reference/generated/numpy.less.html#numpy.less "numpy.less")(x1, x2, /[, out, where, casting, …])
Return the truth value of (x1 < x2) element-wise.

[`less_equal`](https://docs.scipy.org/doc/numpy/reference/generated/numpy.less_equal.html#numpy.less_equal "numpy.less_equal")(x1, x2, /[, out, where, casting, …])
Return the truth value of (x1 =< x2) element-wise.

[`not_equal`](https://docs.scipy.org/doc/numpy/reference/generated/numpy.not_equal.html#numpy.not_equal "numpy.not_equal")(x1, x2, /[, out, where, casting, …])
Return (x1 != x2) element-wise.

[`equal`](https://docs.scipy.org/doc/numpy/reference/generated/numpy.equal.html#numpy.equal "numpy.equal")(x1, x2, /[, out, where, casting, …])
Return (x1 == x2) element-wise.

Warning
Do not use the Python keywords  `and`  and  `or`  to combine logical array expressions. These keywords will test the truth value of the entire array (not element-by-element as you might expect). Use the bitwise operators & and | instead.

[`logical_and`](https://docs.scipy.org/doc/numpy/reference/generated/numpy.logical_and.html#numpy.logical_and "numpy.logical_and")(x1, x2, /[, out, where, …])
Compute the truth value of x1 AND x2 element-wise.

[`logical_or`](https://docs.scipy.org/doc/numpy/reference/generated/numpy.logical_or.html#numpy.logical_or "numpy.logical_or")(x1, x2, /[, out, where, casting, …])
Compute the truth value of x1 OR x2 element-wise.

[`logical_xor`](https://docs.scipy.org/doc/numpy/reference/generated/numpy.logical_xor.html#numpy.logical_xor "numpy.logical_xor")(x1, x2, /[, out, where, …])
Compute the truth value of x1 XOR x2, element-wise.

[`logical_not`](https://docs.scipy.org/doc/numpy/reference/generated/numpy.logical_not.html#numpy.logical_not "numpy.logical_not")(x, /[, out, where, casting, …])

Compute the truth value of NOT x element-wise.

Warning
The bit-wise operators & and | are the proper way to perform element-by-element array comparisons. Be sure you understand the operator precedence:  `(a  >  2)  &  (a  <  5)`  is the proper syntax because  `a  >  2  &  a  <  5`  will result in an error due to the fact that  `2  &  a`  is evaluated first.

[`maximum`](https://docs.scipy.org/doc/numpy/reference/generated/numpy.maximum.html#numpy.maximum "numpy.maximum")(x1, x2, /[, out, where, casting, …])
Element-wise maximum of array elements.

Tip
The Python function  `max()`  will find the maximum over a one-dimensional array, but it will do so using a slower sequence interface. The reduce method of the maximum ufunc is much faster. Also, the  `max()`  method will not give answers you might expect for arrays with greater than one dimension. The reduce method of minimum also allows you to compute a total minimum over an array.

[`minimum`](https://docs.scipy.org/doc/numpy/reference/generated/numpy.minimum.html#numpy.minimum "numpy.minimum")(x1, x2, /[, out, where, casting, …])
Element-wise minimum of array elements.

Warning
the behavior of  `maximum(a,  b)`  is different than that of  `max(a,  b)`. As a ufunc,  `maximum(a,  b)`  performs an element-by-element comparison of  _a_  and  _b_  and chooses each element of the result according to which element in the two arrays is larger. In contrast,  `max(a,  b)`  treats the objects  _a_  and  _b_  as a whole, looks at the (total) truth value of  `a  >  b`and uses it to return either  _a_  or  _b_  (as a whole). A similar difference exists between  `minimum(a,  b)`  and  `min(a,  b)`.

[`fmax`](https://docs.scipy.org/doc/numpy/reference/generated/numpy.fmax.html#numpy.fmax "numpy.fmax")(x1, x2, /[, out, where, casting, …])
Element-wise maximum of array elements.

[`fmin`](https://docs.scipy.org/doc/numpy/reference/generated/numpy.fmin.html#numpy.fmin "numpy.fmin")(x1, x2, /[, out, where, casting, …])
Element-wise minimum of array elements.

### Floating functions[](https://docs.scipy.org/doc/numpy/reference/ufuncs.html#floating-functions "Permalink to this headline")

Recall that all of these functions work element-by-element over an array, returning an array output. The description details only a single operation.

[`isfinite`](https://docs.scipy.org/doc/numpy/reference/generated/numpy.isfinite.html#numpy.isfinite "numpy.isfinite")(x, /[, out, where, casting, order, …])
Test element-wise for finiteness (not infinity or not Not a Number).

[`isinf`](https://docs.scipy.org/doc/numpy/reference/generated/numpy.isinf.html#numpy.isinf "numpy.isinf")(x, /[, out, where, casting, order, …])
Test element-wise for positive or negative infinity.

[`isnan`](https://docs.scipy.org/doc/numpy/reference/generated/numpy.isnan.html#numpy.isnan "numpy.isnan")(x, /[, out, where, casting, order, …])
Test element-wise for NaN and return result as a boolean array.

[`isnat`](https://docs.scipy.org/doc/numpy/reference/generated/numpy.isnat.html#numpy.isnat "numpy.isnat")(x, /[, out, where, casting, order, …])

Test element-wise for NaT (not a time) and return result as a boolean array.

[`fabs`](https://docs.scipy.org/doc/numpy/reference/generated/numpy.fabs.html#numpy.fabs "numpy.fabs")(x, /[, out, where, casting, order, …])
Compute the absolute values element-wise.

[`signbit`](https://docs.scipy.org/doc/numpy/reference/generated/numpy.signbit.html#numpy.signbit "numpy.signbit")(x, /[, out, where, casting, order, …])
Returns element-wise True where signbit is set (less than zero).

[`copysign`](https://docs.scipy.org/doc/numpy/reference/generated/numpy.copysign.html#numpy.copysign "numpy.copysign")(x1, x2, /[, out, where, casting, …])
Change the sign of x1 to that of x2, element-wise.

[`nextafter`](https://docs.scipy.org/doc/numpy/reference/generated/numpy.nextafter.html#numpy.nextafter "numpy.nextafter")(x1, x2, /[, out, where, casting, …])

Return the next floating-point value after x1 towards x2, element-wise.

[`spacing`](https://docs.scipy.org/doc/numpy/reference/generated/numpy.spacing.html#numpy.spacing "numpy.spacing")(x, /[, out, where, casting, order, …])
Return the distance between x and the nearest adjacent number.

[`modf`](https://docs.scipy.org/doc/numpy/reference/generated/numpy.modf.html#numpy.modf "numpy.modf")(x[, out1, out2], / [[, out, where, …])
Return the fractional and integral parts of an array, element-wise.

[`ldexp`](https://docs.scipy.org/doc/numpy/reference/generated/numpy.ldexp.html#numpy.ldexp "numpy.ldexp")(x1, x2, /[, out, where, casting, …])
Returns x1 * 2**x2, element-wise.

[`frexp`](https://docs.scipy.org/doc/numpy/reference/generated/numpy.frexp.html#numpy.frexp "numpy.frexp")(x[, out1, out2], / [[, out, where, …])
Decompose the elements of x into mantissa and twos exponent.

[`fmod`](https://docs.scipy.org/doc/numpy/reference/generated/numpy.fmod.html#numpy.fmod "numpy.fmod")(x1, x2, /[, out, where, casting, …])
Return the element-wise remainder of division.

[`floor`](https://docs.scipy.org/doc/numpy/reference/generated/numpy.floor.html#numpy.floor "numpy.floor")(x, /[, out, where, casting, order, …])

Return the floor of the input, element-wise.
[`ceil`](https://docs.scipy.org/doc/numpy/reference/generated/numpy.ceil.html#numpy.ceil "numpy.ceil")(x, /[, out, where, casting, order, …])

Return the ceiling of the input, element-wise.

[`trunc`](https://docs.scipy.org/doc/numpy/reference/generated/numpy.trunc.html#numpy.trunc "numpy.trunc")(x, /[, out, where, casting, order, …])
Return the truncated value of the input, element-wise.
<!--stackedit_data:
eyJoaXN0b3J5IjpbOTcyNTMzMDU5LDYxNzc4MzY2MCwxMzE5ND
EzOTc4LC0yMDk1MjYxNzMzLC0xMzY3Mzg3Mzk5LC00MjQ0NTUx
OTddfQ==
-->