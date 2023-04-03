Webcam
========

```hydra
s0.initCam()
src(s0).out()
```

make sure you allow webcam!


Colors
--------

```hydra
s0.initCam()
src(s0).color(1,0,0).out()
```


```hydra
s0.initCam()
src(s0).colorama(0.01).out()
```

```hydra
s0.initCam()
src(s0).saturate(8).out()
```

```hydra
s0.initCam()
src(s0).thresh(0.3).out()
```

```hydra
s0.initCam()
src(s0).luma(0.3).out()
```


Geometry
--------

```hydra
s0.initCam()
src(s0).repeat(2,2).out()
```

```hydra
s0.initCam()
src(s0).scrollX(0,0.1).out()
```

```hydra
s0.initCam()
src(s0).scrollY(0,0.1).out()
```
