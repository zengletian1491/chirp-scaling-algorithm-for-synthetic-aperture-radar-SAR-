chirp scaling algorithm(CSA) for synthetic aperture radar (SAR) imaging

1.Run

You can run the following three .m programs directly on Matlab. These programs are tested on Matlab 2015a.

1）Final_cs_broadside.m :

working conditions：height of flying platform is 0；broadside mode；slant plane imaging （不考虑高度、正侧视、斜平面成像、cs算法）

2）Final_cs_squint5.m :

working conditions：height of flying platform is 0；squint angle is 5 degree；slant plane imaging. The imaging results are poor for the range sampling rate (Fs = 200e6) is too low, which leads to the folding of two-dimension spectrum. 不考虑高度、斜视 5 度、斜平面cs成像算法，效果不好；因为二维频谱折叠，需提高距离向采样率 Fs

Improved versions for squint mode imaging:

3）Final_cs_squint5_new.m :

working conditions：height of flying platform is 0；squint angle is 5 degree；slant plane imaging; Fs = 400e6. 不考虑高度、斜视 5 度、斜平面cs成像算法，效果好

2.Note

1）You can change the value of "nan" (in the .m programs), making it satisfy the length of a synthetic aperture.


2）The peak sidelobe ratio (PSLR) and the integrated sidelobe ratio (ISLR) are calculated by the functions PSLR() and ISLR(), respectively. In addition, the contour map can be drown by the function Interplate2D().

3.Imaging results

1）Contour map

![Uploading 2024-06-13_221403.png…]()
