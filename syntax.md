# Commands

## I/O Control (Sending/Receiving)
```io <disk> <bus> <frequency> <invert?>```
- ```disk``` should be a input bus number (so the machine can use that bus to call data from the disk)
- ```bus``` should be a output bus number.
- ```frequency``` should be a number, the frequency unit is ALPs.
- ```invert?``` is a basic encryption feature, it should be a 1 for yes, 0 for no. (all it does is runs the data through a NOT gate)

## Controlling hardware
The following command can delete disk data:

```a k <disk>```
- ```disk``` should be a input bus number (so the machine can use that bus to call data from the disk)
The following command can block bus usage:

```a b <block/unblock?> <bus>```
- ```block/unblock?``` should be a number, 1 for yes (block), 0 for no (unblock).
- ```bus``` should be a input or output bus number.

## Functions
```f (<cmd>,<cmd>) <as>```
- ```cmd``` should be any command and it's syntax. Separate commands with commas. If you need to use a function in a function then the syntax is the same, and it will look something like this: ```f (f (io 1 1 4 0, io 1 2 4 0),a k 1)```
- ```as``` should be the name of the function.
```f <function>```
- ```function``` should be the name of the function, example:
```f (io 7 2 4 0) jk```
```f jk```
