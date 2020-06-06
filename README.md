# bspwm-termux
steps for compiling and using bspwm on Termux
## dependencies
the dependencies are included in the termux repos, no additional compiling required:
* ```xcb-util-renderutil```
* ```xcb-util-image```
* ```xcb-util-keysyms```
* ```xcb-util-wm```
* ```xcb-util```
* ```xcb-util-cursor```
* ```libxcb``` (can't verify if it's truly needed)

you will also need the basic tools for compilation:

* ```make```
* ```cmake```
* ```clang```


it's adviseable to use a hotkey daemon, like ```sxhkd```. 

clone the repository:

```git clone https://github.com/baskerville/bspwm.git```

apply the ```bspwm-on-termux.patch``` patch (**note**: the Makefile is not patched for the correct ```/bin``` folder, after compilation you'll have to move the binaries manually).
