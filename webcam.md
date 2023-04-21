🎥Webcam
========

make sure you allow webcam!

```hydra
s0.initCam()
src(s0).out()
```



Colors
--------

```hydra
src(s0).color(1,0,0).out()
```

```hydra
src(s0).colorama(0.01).out()
```

```hydra
src(s0).saturate(8).out()
```

```hydra
src(s0).thresh(0.3).out()
```

```hydra
src(s0).luma(0.3).out()
```

Rhythm
--------

```hydra
src(s0).color([1,1,0],1,[0,1]).out()
```


Geometry
--------

```hydra
src(s0).repeat(2,2).out()
```

```hydra
src(s0).scale(2).out()
```

```hydra
src(s0).scale(1,-1,1).out()
```

```hydra
src(s0).kaleid(4).out()
```

```hydra
src(s0).scrollX(0,0.1).out()
```

```hydra
src(s0).scrollY(0,0.1).out()
```


```hydra
src(s0).rotate(0,0.1).out()
```


Combination
--------

```hydra
src(s0).repeat(2,2).color(1,-1,1).out()
```

[next: sources](sources)
