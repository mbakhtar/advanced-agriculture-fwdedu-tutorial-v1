# Advanced Agriculture CAK V2.1 fwdEDU

```package
``` 
## @showhint
Add the ``||Input:on Button A Pressed||`` block
```blocks
input.onButtonPressed(Button.A, function () {
})
```
## @showhint
Add the ``||basic: showIcon||`` block nested under ``||Input:on Button A Pressed||`` select the umbrella icon from the dropdown
```blocks
input.onButtonPressed(Button.A, function () {
    basic.showIcon(IconNames.Umbrella)
})
```
## @showhint
Add ``||cakLandPump:run right pump at speed 0 for 0 seconds||`` nested in the ``||input:on Button A pressed||`` block and under ``||basic:showIcon||`` block. Change the speed to 60 and time to 4.
```blocks
input.onButtonPressed(Button.A, function () {
    basic.showIcon(IconNames.Umbrella)
        fwdMotors.pump.fwdTimedRun(4000)
    })
```
## @showhint
The last step is a check step to identify the pump has run for the set duration. Add ``||basic:clearScreen||`` it will turn off the ``||basic:Umbrella||`` icon
```blocks
input.onButtonPressed(Button.A, function () {
    basic.showIcon(IconNames.Umbrella)
        fwdMotors.pump.fwdTimedRun(4000)
    basic.clearScreen()
})
``` 

## @showhint
Here is the final code
```blocks
input.onButtonPressed(Button.A, function () {
    basic.showIcon(IconNames.Umbrella)
        fwdMotors.pump.fwdTimedRun(4000)
    basic.clearScreen()
})
```
