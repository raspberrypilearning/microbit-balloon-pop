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

- From the `Basic`{:class="microbitbasic"} menu, drag the `show icon`{:class="microbitbasic"} block into the code editor. 
  
- Place it inside the  `on start`{:class="microbitbasic"} block. 

- Select a tick icon to show when the micro:bit is ready.

--- /task ---

--- task ---

- From the `Input`{:class="microbitinput"} menu, drag the `on button [A]`{:class="microbitinput"} block to the code editor panel.

- Click `Advanced`. 
  
- From the `Pin`{:class="microbitpins"} menu, drag the `digital write pin`{:class="microbitpins"} block into the code editor. 

- Place it in the `on button [A]`{:class="microbitinput"} block.

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

Here are some more examples of people having fun with this project!

<html>
<video width="540" height="720" controls>
<source src="images/pop1.mp4" type="video/mp4">
Your browser does not support the video tag.
</video>
</html>
<html>
<video width="540" height="720" controls>
<source src="images/pop2.mp4" type="video/mp4">
Your browser does not support the video tag.
</video>
</html>
<html>
<video width="720" height="540" controls>
<source src="images/pop3.mp4" type="video/mp4">
Your browser does not support the video tag.
</video>
</html>