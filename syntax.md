## Sending Data
```s <frequency> <repeat?>```
- Frequency must be a number, the unit is ALPs.
- Repeat must also be a number, 1 is yes, 0 is no.

## Relaying Data
```r <bus> <frequency> <repeat?>```
- Bus requires hardware modification, it should be the number of the bus you are using to relay the data.
- Frequency must be a number, the unit is ALPs.
- Repeat must also be a number, 1 is yes, 0 is no.

## Encrypting Data
```e <mode>```
- Mode should be a number, it defines how the data should be shifted. There is no decrypt function so the reciever must know how to decrypt it themselves.

## Turning the networker on/off
```a <on/off?>```
- on/off should be a number, 1 to turn on the networker, 0 to turn off the networker.
