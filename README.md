# Homomorphic Filtering

This code implement an [Homomorphic filter](https://en.wikipedia.org/wiki/Homomorphic_filtering) in the frequency domain.

An image can be expressed as the product of its illumination, _i(x,y)_, and reflectance, _r(x,y): f(x,y)=i(x,y)r(x,y)_. In general _i(x,y)_ and _r(x,y)_ are unkown but we want to operate this component separately.

This filter is useful for attenuate the contribution made by the low frequencies(illumination) and amplify the contribution made by high frequencies(reflectance): The result is simultaneaous dynamic range compression and contrast enhacement.

The costant _C_ control the sharpness of the function as it transition between deltaL and deltaH.

If _gH>=1_ and _0<gL<1_ the high frequencies are amplified and the low frequencies are cutted off, _gL_ is also used to preserve the tonality of the image.
