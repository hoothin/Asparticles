ASParticles
===========

Rework of http://code.google.com/p/haxe-particle-designer/ 

As Tilesheet of openfl do not support rotation, alpha, scale and RGB under flash target, BitmapData.Draw will be used instead of Tilesheet, and it will be shown only above (0,0)

Install via haxelib with

```
haxelib git asparticles https://github.com/hoothin/asparticles
```

```
var particles = ASParticleSystem.particleWithFile("fire.plist", "particles/");
addChild(particles);

```

Call destroy while complete
```
particles.destroy();
```

U can do sth before add a particle
```
particles.beforeAddCallBack = function(a){particles.sourcePosition.x = a*500;};
```
