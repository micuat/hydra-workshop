🌈Sources
========

Basics
--------

```hydra
osc(30).out()
```

```hydra
osc(30,0.1,1.5).out()
```

```hydra
noise(5).out()
```

```hydra
gradient().out()
```

Blending
--------

```hydra
s0.initCam()
src(s0).blend(noise(5), 0.5).out()
```

```hydra
s0.initCam()
src(s0).add(osc(5,0.1,1.5), 0.5).out()
```

```hydra
s0.initCam()
src(s0).diff(osc(5,0.1,1.5)).out()
```

```hydra
s0.initCam()
src(s0).mult(osc(5)).out()
```


Modulate
--------

```hydra
s0.initCam()
src(s0).modulate(noise(5)).out()
```

```hydra
s0.initCam()
osc(3,0.1,1.5).modulate(src(s0),0.8).out()
```

[next: practice](practice)
