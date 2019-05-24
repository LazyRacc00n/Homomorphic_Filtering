# Homomorphic Filtering
This code implement a filter in the frequency domain.
An image can be expressed as the product of its illumination, i(x,y), and reflectance, r(x,y): f(x,y)=i(x,y)r(x,y). In general i(x,y) and r(x,y) are unkown but we want to operate this component separately.
This filter is useful for attenuate the contribution made by the low frequencies(illumination) and amplify the contribution made by high frequencies(reflectance): The result is simultaneaous dynamic range compression and contrast enhacement.
The costant C control the sharpness of the function as it transition between deltaL and deltaH.
If gH>=1 and 0<gL<1 the high frequencies are amplified and the low frequencies are cutted off, gL is also used to preserve the tonality of the image.
