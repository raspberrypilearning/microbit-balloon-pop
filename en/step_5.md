## Add the balloon to the code

Now we've completed our circuit we'll need to write code to trigger the transistor, allowing current to flow through the resistor, which will pop the balloon.

--- task ---

Drag the `show icon`{:class="microbitbasic"} block into the code editor. 

Place it inside the  `on start`{:class="microbitbasic"} block. 

Select a tick icon to show when the micro:bit is ready.

From the `Input`{:class="microbitinput"} menu, drag the `on button [A]`{:class="microbitinput"} block to the code editor panel.

Click `Advanced`. From the `Pin` {:class="microbitpins"} menu drag the `digital write pin`{:class="microbitpins"} block.

Place it in the `on button [A]`{:class="microbitinput"} block in the code editor panel.

```microbit
input.onButtonPressed(Button.A, function () {
    pins.digitalWritePin(DigitalPin.P0, 1)
})
basic.showIcon(IconNames.Yes)
```
--- /task ---

--- task ---

Now comes the code to pop the balloon.

--- task ---

Download your program onto your micro:bit!

--- /task ---

[[[download-to-microbit]]]

### Test your program

--- task ---

Wait for the tick to show and then press button A.

Depending on the thickness of your balloon and how much it has been blown up and stretched, this may take five seconds or more.

--- /task ---

