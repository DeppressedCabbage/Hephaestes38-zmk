<h1 align="left">Intro</h1>

### Hands Down
"Hands Down Layout variations were developed on a sound linguistic foundation (phonotactics) and an obsessive attention to corpus statistics using a variety of keyboard layout analyzers and methods that are all tested in live real-world situations to produce exceptionally comfortable long duration typing on modern keyboards." 
  - R. Alan Reiser
Who better to describe the layout than the very one who coined the layout and created such a strong foundation for the variation I landed on. Hands down layouts tend to yield extremely low SFBs, low redirects and low center column usage. This results in a very steady rythym when typing, creating a more comfortable, relaxed, and overall smoother experience.

### HD Promethium
I could personally never expect to explain the variation of the hands down layout as well as the two geniouses who first created it, u/phbonachi and u/RoastBeefer, so if you want an in depth writeup of the layout itself, please see [this](https://www.reddit.com/r/KeyboardLayouts/comments/1g66ivi/hands_down_promethium_snth_meets_hd_silverengram/) post. For a more high level overview, read ahead. 

A "SYNTH" and "AEI" home row help to make the in:out rolling ratio over 2:1, the H-Digrams have been maximized, pinky/ring scissors, same finger bigrams, lateral stretch, and center column usage have all been minimalized. 

![HDPM Canonical layout](https://github.com/user-attachments/assets/60cb91be-0f32-49f8-a9ed-509a008d0796)

I had to modify my layout to work with the 38 keys on my keyboard, so it differs slightly from the "canonical" Layout pictured above. You can see the changes I made below. On a high level I moved the backspace key from the thumb cluster and replaced it with a oneshot shift key. Enter was also moved to a combo and replaced with the left alt, and the "Z" key was moved in place of the "/". TAB and Left CTR have been moved down in place of the "Backslash" key. 

<img width="1415" height="637" alt="image" src="https://github.com/user-attachments/assets/0eda7f88-bf70-4292-bc56-668e2144e39f" />



### Layers and combos
A small keyboard is great, but if you only have alpha keys, it tends to not work the best for day to day productivity. To fix this, I use a Number and Symbol layer, as well as a dedicated Navigation layer. You can see them pictured below. To get to and from the layers, I use combos that utilize both the home row and the thumb. I found that this combination of fingers allows for very few false activations while still easily being activated when on purpose. 

To get to the Number Layer, the keys "E"and "Space" are used. ZMK studio doesn't like to show what is actually being sent to the computer sometimes, so this layout looks a bit odd. For example, on the left side of the keyboard you may notice some duplicate numbers, these are actualy sent to the computer with a modifier. You're left pinkey ("1") send an eclamation point, Left ring (/) sends a Qestion mark, Left middle and index ("9, 0") Send Parenthesis, and so on. 
<img width="1401" height="662" alt="image" src="https://github.com/user-attachments/assets/4849e8f5-cee3-4c29-8539-33bd3346e686" />

"T" and "R" allow access to the navigation layer, and is the same as the number layer, just mirrored.
<img width="1408" height="726" alt="image" src="https://github.com/user-attachments/assets/9e36d89e-00d4-4463-b3b4-5c1387ee9137" />
This layer also has bluetooth and screen controls, along with the ability to unlock ZMK studio so that you can make any changes you want in a GUI. Just as zmk studio doesn't display the correct modifiers, it also doesn't show keyboard controls. For that to be visualized you need to go into the actual keymap, but I will explain them all here. EP on, off, and tog all control the external power of the Nice!Nano, which in turn turns the screen on and off. BT_SEL will connect the keyboard to up to 5 different bluetooth profiles, meaning the keyboard could be connected to up to 5 different devices simultaneously. Lastly, the studio unlock key is used to unlock zmk studio, allowing changes to the keymap without the need to re-flash the firmware.
<img width="948" height="79" alt="image" src="https://github.com/user-attachments/assets/6105707c-eb00-4a02-95c4-ea771a379b17" />


For those of you who would prefer to use the traditional QWERTY Layout, I have also added it into the keymap so that you can switch back and forth between this and the default HD Promethium. The combo "X"+"Backspace" is used to toggle this layer. The blank keys on this visualization are simply transparent, which means that it will just use they keys from the default layer, being Tab, Left control, Left Alt, Sticky Shift, and Space. 
<img width="1459" height="659" alt="image" src="https://github.com/user-attachments/assets/41e41a19-9e93-4ab6-9b74-5423f5730934" />


I also have several empty layers that you can set up in zmk studio without having to mess with the keymap firmware. To unlock zmk studio, use the navigation layer and the "Studio Unlock" key ("M" Key on the alpha layer). These layers use the combo's "K"+",", and "J"+"-". To get back to the default alpha layer, you can press the same combo that got you to the layer to get out, as these combo's are set up as layer toggles. Alternatively, on the Number and Navigation Layers, you can hit the outermost thumb key on the right hand (Oneshot Shift key on the alpha layer) to get back to the default layer. I would recommend using this same key on all layers you add, as this really streamlines swithcing to and from the alpha layer.

You may have noticed that none of these layers contain common keys that we all use from day to day. For these keys, we use the combo's listed below. 

Enter is the index, middle and ring finger of the right hand resting in the home position ("A","E","I" on the alpha layer)
Escape is the index and middle finger of the left hand resting in the home position ("T", "H" on the alpha layer)
The OS Key is the ring an  index finger of the left hand resting in the home position ("N", "H" on the alpha layer)
Delete is the index ande middle finger of the left hand one row above the home position ("D", "L" on the alpha layer)

All of the modifier combos work on all layers, but all layer combo's do not work on all layers. ZMK firmware only allows for direct switching to a layer above, or going back to the default layer. Because of this, you can go from the Navigation layer up to the Number layer, but not from the Number layer down to the Navigation layer. You would need to go back to the alpha layer, and then to the Navigation layer from the Number layer. 
