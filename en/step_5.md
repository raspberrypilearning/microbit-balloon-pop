## Add the code

Now you have completed your circuit you need to write code to trigger the transistor, allowing current to flow through the resistor, which will pop the balloon.

### Open MakeCode

--- task ---

Open the MakeCode editor at [makecode.microbit.org](https://makecode.microbit.org){:target="_blank"}.

--- /task ---

--- collapse ---

---
title: Offline version of the editor
---

There is also a [downloadable version of the MakeCode editor](https://makecode.microbit.org/offline-app){:target="_blank"}.

--- /collapse ---

--- /task ---

### First micro:bit project?

[[[makecode-tour]]]

### Create your project

--- task ---

Click on the **New Project** button.

<img src="images/new-project-button.png" alt="The New Project button inside MakeCode." width="250"/>

--- /task ---

--- task ---

Give your project a name. 

--- /task ---

--- task ---

- Drag the `show icon`{:class="microbitbasic"} block into the code editor. 
  
- Place it inside the  `on start`{:class="microbitbasic"} block. 

- Select a tick icon to show when the micro:bit is ready.

--- /task ---

--- task ---

- From the `Input`{:class="microbitinput"} menu, drag the `on button [A]`{:class="microbitinput"} block to the code editor panel.

- Click `Advanced`. From the `Pin` {:class="microbitpins"} menu drag the `digital write pin`{:class="microbitpins"} block. Place it in the `on button [A]`{:class="microbitinput"} block in the code editor panel.

--- /task ---

```microbit
input.onButtonPressed(Button.A, function () {
    pins.digitalWritePin(DigitalPin.P0, 1)
})
basic.showIcon(IconNames.Yes)
```

--- task ---

Download your program onto your micro:bit!

--- /task ---

[[[download-to-microbit]]]

### Test your program

--- task ---

Wait for the tick to show and then press button A.

Depending on the thickness of your balloon and how much it has been blown up and stretched, this may take five seconds or more.

--- /task ---

