# Hack Synapse

Hack indicator synapse using [xdotool](https://github.com/jordansissel/xdotool) for ubuntu. 
inspired by Mac Spotlight, [Indicator Synapse](http://www.elementaryos-fr.org/documentation/indicators/indicator-synapse/) for Elementary OS, and [Xdotool](https://github.com/jordansissel/xdotool). Powered by [Piotr Wittchen](http://blog.wittchen.biz.pl/synapse-indicator-spotlight-for-ubuntu/).

<br>
<<<<<<< HEAD
=======


![](https://github.com/indrabinridwan/hack-synapse/blob/master/hack.gif)


### Installation
Install **Indicator Synapse** in ubuntu. Can be installed with the following commands,

```
sudo add-apt-repository ppa:noobslab/apps 
sudo apt-get update
sudo apt-get install indicator-synapse

```

Install [Xdotool](https://github.com/jordansissel/xdotool) with the following commands.

```
sudo apt-get install xdotool

```

<br>
### Adding keyboard shortcut for Synapse Indicator (Hack)

**Step 1 :** Move your mouse over the synapse icon and get mouse location via xdotool in terminal. Like this,


```
xdotool getmouselocation
```
and you should get output like this:
```
x:1003 y:13 screen:0 window:62914568
```
<br>
**Step 2 :** Add keyboard shortcut for Indicator Synapse. Go to
```System Settings``` -> ```Keyboard``` -> ```Shortcuts``` -> ```Custom Shortcuts``` <br>
Click add and for the command type like this,
```
xdotool mousemove <x> <y> click 1 mousemove restore

```
Replace x and y with getmouselocation value. example: 

```
xdotool mousemove 1003 13 click 1 mousemove restore

```
and finally add accelerator  ```ctrl + space``` for this shortcut.

