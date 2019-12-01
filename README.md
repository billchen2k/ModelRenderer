# OpenGL Module Loader

<center><a href = 'README.md'><b>English</b></a> | <a href = 'README_CN.md'>简体中文</a></center>

### Intro

A simple 3D module renderer by `OpenGL` & `C# .Net Framework 4.5` with user-friendly GUI and detailed parameter tuning.

With:

- Detailed light adjustments, including ambient light, diffuse light & specular light.
- View matrix adjustment, rotating object automatically
- Partial rendering
- Render status logging and performance statistics

![image-20191201151506627](https://billc.oss-cn-shanghai.aliyuncs.com/img/2020-07-26-zZBY1B.png)

### Usage

#### Input data

The module file should be as following format:

`<point_id> <x> <y> <z>`

Eg.:

```
    1  .67917E+00  .48325E+01  .00000E+00
    2 -.22392E+03  .36400E+02  .00000E+00
    3 -.22392E+03  .00000E+00  .00000E+00
    4  .48800E+01  .00000E+00  .00000E+00
    5  .48106E+01  .81984E+00  .00000E+00
    6  .45908E+01  .16548E+01  .00000E+00
    7  .42125E+01  .24636E+01  .00000E+00
    8  .36830E+01  .32016E+01  .00000E+00
    9  .30259E+01  .38286E+01  .00000E+00
```

Will use `2.txt` by default.

#### Rendering

Select `Render All` to render all contents, including surfaces, dots and light (Ambient, Diffuse & Specular), or use different combinations to render part of the module.

Controlling the view point and light position by tuning the values of the textfields. Select `reset` to reset all parameters.

Check auto rotation to observe the module dynamically. The module would then rotate around y axis.

Uncheck `clear before repaint` will keep the rendered data before the new frame. Thus the accumulated rendering result can be seen. Note that resizing the window will also clear all the render buffers.

![image-20191201152538066](https://billc.oss-cn-shanghai.aliyuncs.com/img/2020-07-26-Cs8Wai.png)

---

> Bill Chen, East China Normal University.
> 2019.12.1
> https://billc.io

