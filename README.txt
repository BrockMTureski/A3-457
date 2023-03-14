Brock Tureski, 20151968, 18bmt1

note: I included only the unfiltered back projection of the foot as filtered was not specified.


Q1. A good numSinoAngles for filtered backprojections to not see noticeable improvements is 360 angles, this is because that would be the same 
as a 360 degree rotation during reconstruction which is equivalent to a full rotation of the image. After this amount there is not much of an 
improvement in quality of the filtered back projection of the sinogram.

Q2. The circle around everything in the back projection image is due to the rotation in the back projection and sinogram construction algorithms, 
this rotation causes for parts of the image to be cutoff during these processes. This is evident in the fact that the circle is the same diameter
of the image width. This could be avoided by padding the image with the distance from the center of the original image to the corner of the image
(the maximum distance from center to edge) on all sides of the image before both of said algorithms are performed and then dropping the padding
after performing the backprojection.