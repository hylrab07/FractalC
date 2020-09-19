

# FractalC  v0.4a-1
## Terminal Activated Mandelbrot & Julia Fractal Generator in C/C++
![example](https://i.imgur.com/xeWEB2n.png)
![logo](https://i.imgur.com/9MKpYtN.png)
## Setup;

### ---Compile From Source---
***Linux***: **$** `gcc -o FractalC_linux64 FractalCMain.C -lm -fno-threadsafe-statics -O2 -lstdc++`
- Requires GCC (any C++ compiler will do though), but it should already be installed

***Windows x86-x64***: **>** `i686-w64-mingw32-gcc -o FractalC.exe FractalCMain.C -lm -fno-threadsafe-statics -O2 -lstdc++`
- Requires MinGW

### ---Running the binaries---
***Linux***: **$** `./FractalCv0.3a-1 [ARGUMENTS]`

***Windows***: **>** `start FractalCv0.3a-1.exe [ARGUMENTS]`
# Input flags;
### You can input these in any order you want as long as they all appear no more than once in your input
## There are 21 possible flags
* **-mode**
	- `Mode of 0 = Mandelbrot`
	- `Mode of 1 = Burning Ship`

* **-name**
	- `Name ending in .png or .jpg`
	
* **-pos**
	 - `Complex Coordinate the image is centered on; two numbers`

* **-zoom**
	- `Multiplier of magnification`

* **-lim**
	- `The iteration limit`

* **-cExp**
	- `The scale tuning of colors`
	
* **-res**
	- `Multiplier of resolution ( Must be less than 101)`
	- `Image size = 60 * resolution * ratio`
	- `Pass lower-case "l" for maximum res possible
	
* **-ratio**
	- `Ratio of image`
	
* **-isJulia**
	- `if specified, it will render a Julia Fractal`

* **-jPos**
	- `Julia Coordinates; enter two numbers`

* **-fancy**
	- `If specified, it will enable trippy colors (slower rendering)`

* **-zMax**
	- `if Z.real or z.imag exceeds this value, it will stop the iteration for that pixel`

* **-log**
	- `Specifies number of console logs`

* **-cOffset**
	- `Multiple of 45 to offset the color`

* **-cScale**
	- `Multiplies frequency of color`
* **-bw**
	- `Specify for black and white`
* **-inverted**
	- `Inverts colors`
* **-fade**
	- `Specify for a fade effect`
	- `Input must be "in" or "out"`
* **-fadeDark**
	- `If specified, fade will be dark`
	_ `If unspecified, fade will be light`
* **-lScale**
	- `Fade scale`
* **-lExp**
	- `Fade exponent, similar to scale, idk`
	
**Example Of An Input;**
- **$** `./FractalC -pos 0 0 -isJulia -zoom 0.7 -jPos -0.1 -0.65287 -res 25 -cExp 0.2 -cScale 6 -fade in -fadeDark -lScale 0.25 -lExp 1.5 `
- **>** `start FractalC.exe -pos 0 0 -isJulia -zoom 0.7 -jPos -0.1 -0.65287 -res 25 -cExp 0.2 -cScale 6 -fade in -fadeDark -lScale 0.25 -lExp 1.5 `

![Example of use with new features](https://i.imgur.com/0aYx7Ig.png)
# License
```
MIT License

Copyright (c) 2020 ahhhh6980

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```

