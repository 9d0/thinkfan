# thinkfan
Tired of the hum? Me too. Thinkfan allows you to silence a ThinkPad laptop in Plan 9. It is inspired by [the identically named Linux program](http://thinkfan.sourceforge.net).  

The program is dead simple. Run thinkfan without arguments and it tells you the current fan speed. Give it a number in the range of 0 to 7, and it sets the fan speed accordingly. Zero means off, 7 indicates the maximum speed. That's all. I am relying on Intel to throttle their processor before it overheats. Zero fried chips this far. I also run stats -z on my desktop to keep an eye on the temperature. 

I have successfully tested this program on Lenovo ThinkPad models X220 and X230.

## Installation
`cp thinkfan /rc/bin/`

`echo thinkfan 1 >/cfg/$sysname/termrc`
