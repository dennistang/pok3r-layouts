# POK3R keyboard layouts for macOS and Windows
For those who don't know what a POK3R keyboard is, this is a decent [review](https://www.youtube.com/watch?v=8wjW-Or1jg8).
Multiple sources to buy, e.g. [amazon](http://smile.amazon.com/Mechanical-Keyboard-Keycaps-Cherry-Mx-Blue/dp/B00OFM51L2/), [mechanicalkeyboards.com](https://mechanicalkeyboards.com/shop/index.php?l=product_detail&p=1233)

The following layers are used in either OS:
* macOS: Layer 2 (red LED), switch with: `FN + ,<`
* Windows: Layer 3 (blue LED), switch to it with: `FN + .>`

## General POK3R programming info
* [POK3R User Manual](files/POK3R.User.Manual.V1.5.2.pdf); Vortex keeps shifting their URLs, so local copy (thanks @couto, @josephfusco)
* Current POK3R version is: [1.17](http://vortexgear.tw/db/upload/webdata4/6vortex_2016522355271164.exe), which includes shortcuts for media control, e.g., prev/next/pause/play, and volume controls.
* Factory reset: Hold both the left and right `ALT` keys
* Reset selected layer only: `FN + R` until LED under spacebar stops flashing

### Programming of layers 2-4:
* Default layer cannot be programmed
* `FN + R_Ctrl`  (use `L_Ctrl` if `FN` has been reassigned already) -> second LED under space bar is now lit
* hit `target key`, then: `new content` (can be up to 32 char), then: `PN` (second LED will blink while programming)
* `FN + R_Ctrl` to exit programming -> second LED extinguishes
* During programming, use the keys as labelled on the keyboard, irrespective of any reassignments

## Layer 2 (Blue) for macOS:
`FN + ,<` to switch to Layer 2
* [Move FN to L_Ctrl](#Move_FN)
* `FN + R_Ctrl` to enter programming
* [Common bindings](#common_bindings)
* Swap Cmd/Opt keys on both sides of space bar:
  * L_Cmd: `L_Alt` then: `L_WIN` then: `PN`
  * L_Option: `L_WIN` then: `L_Alt` then: `PN`
  * R_CMD: `R_Alt` then: `R_FN` (Win) then: `PN`
  * R_Option: `R_FN` (Win) then: `R_Alt` then: `PN`
* Do it again for the `FN` combos (otherwise you get the default behavior for text selection shortcuts):
  * L_Cmd: `FN + L_Alt` then: `FN + L_WIN` then: `PN`
  * L_Option: `FN + L_WIN` then: `FN + L_Alt` then: `PN`
  * R_CMD: `FN + R_Alt` then: `FN + R_FN` (Win) then: `PN`
  * R_Option: `FN + R_FN` (Win) then: `FN + R_Alt` then: `PN`
* `FN + R_Ctrl` to exit programming

Resulting programming:
![macOS layout](img/layout-macos.png)

macOS Layout on [keyboard-layout-editor.com](http://www.keyboard-layout-editor.com/##@_name=Pok3r%20Layer%203%20for%20macOS&author=dennistang&notes=See%20%5Bgithub%5D(https%2F:%2F%2F%2F%2Fgithub.com%2F%2Fdennistang%2F%2Fpok3r-layouts)%3B&@_y:1.5&c=%233c4041&t=%23aba18b&p=DCS&a:7%3B&=Esc%0A%0A%0A%0A%60%20~&_a:4%3B&=!%0A1%0A%0A%0AF1&=%2F@%0A2%0A%0A%0AF2&=%23%0A3%0A%0A%0AF3&=$%0A4%0A%0A%0AF4&=%25%0A5%0A%0A%0AF5&=%5E%0A6%0A%0A%0AF6&=%2F&%0A7%0A%0A%0AF7&=*%0A8%0A%0A%0AF8&=(%0A9%0A%0A%0AF9&=)%0A0%0A%0A%0AF10&=%2F_%0A-%0A%0A%0AF11&=+%0A%2F=%0A%0A%0AF12&_w:2%3B&=%0ABackspace%0A%0A%0ADel%3B&@_w:1.5%3B&=%0ATab&=Q%0A%0A%0A%0APrev&=W%0A%0A%0A%0APlay&=E%0A%0A%0A%0ANext&=R%0A%0A%0A%0AReset&=T%0A%0A%0A%0A15ms&=Y%0A%0A%0A%0ACal&=U%0A%0A%0A%0APgUp&_c=%23c7c3b5&t=%23ba1312%3B&=I%0A%0A%0A%0AHome&_c=%233c4041&t=%23aba18b%3B&=O%0A%0A%0A%0APgDn&=P%0A%0A%0A%0APrtSc&=%7B%0A%5B%0A%0A%0ABright%20-&=%7D%0A%5D%0A%0A%0ABright%20+&_w:1.5%3B&=%7C%0A%5C%3B&@_c=%23c7c3b5&t=%23ba1312&w:1.25&w2:1.75%3B&=%0ACtrl&_x:0.5%3B&=A%0A%0A%0A%0AVol-&=S%0A%0A%0A%0AVol+&=D%0A%0A%0A%0AMute&=F%0A%0A%0A%0APgDn&_c=%233c4041&t=%23aba18b%3B&=G%0A%0A%0A%0A0.1s&_c=%23c7c3b5&t=%23ba1312%3B&=H%0A%0A%0A%0ALeft&=J%0A%0A%0A%0ADown&=K%0A%0A%0A%0AUp&=L%0A%0A%0A%0ARight&_c=%233c4041&t=%23aba18b%3B&=%2F:%0A%2F%3B%0A%0A%0AIns&=%22%0A'%0A%0A%0ADel&_w:2.25%3B&=%0AEnter%3B&@_w:2.25%3B&=%0AShift&=Z%0A%0A%0A%0AApp&=X&=C&=V&_c=%23c7c3b5&t=%23ba1312%3B&=B%0A%0A%0A%0APgUp&_c=%233c4041&t=%23aba18b%3B&=N%0A%0A%0A%0AEnd&=M%0A%0A%0A%0ADefault&=%3C%0A,%0A%0A%0ALayer%202&=%3E%0A.%0A%0A%0ALayer%203&=%3F%0A%2F%2F%0A%0A%0ALayer%204&_w:2.75%3B&=%0AShift%3B&@_c=%23c7c3b5&t=%23ba1312&w:1.25%3B&=%0AFN&_w:1.25%3B&=%0AOption&_w:1.25%3B&=%0ACMD&_c=%233c4041&t=%23aba18b&p=DCS%20SPACE&a:7&w:6.25%3B&=&_c=%23c7c3b5&t=%23ba1312&p=DCS&a:4&w:1.25%3B&=%0ACMD&_w:1.25%3B&=%0AOption&_c=%233c4041&t=%23aba18b&w:1.25%3B&=%0APn&_w:1.25%3B&=%0ACtrl)

## Layer 3 (Red) for Windows:
`FN + .` to switch to Layer  3
* [Move FN to L_Ctrl](#Move_FN)
* `FN + R_Ctrl` to enter programming
* [Common bindings](#common_bindings)
* `FN + R_Ctrl` to exit programming

Resulting programming:
![Windows layout](img/layout-windows.png)

Windows Layout on [keyboard-layout-editor.com](http://www.keyboard-layout-editor.com/##@_name=Pok3r%20Layer%203%20for%20Windows&author=dennistang&notes=See%20%5Bgithub%5D(https%2F:%2F%2F%2F%2Fgithub.com%2F%2Fdennistang%2F%2Fpok3r-layouts)%3B&@_y:1.5&c=%233c4041&t=%23aba18b&p=DCS&a:7%3B&=Esc%0A%0A%0A%0A%60%20~&_a:4%3B&=!%0A1%0A%0A%0AF1&=%2F@%0A2%0A%0A%0AF2&=%23%0A3%0A%0A%0AF3&=$%0A4%0A%0A%0AF4&=%25%0A5%0A%0A%0AF5&=%5E%0A6%0A%0A%0AF6&=%2F&%0A7%0A%0A%0AF7&=*%0A8%0A%0A%0AF8&=(%0A9%0A%0A%0AF9&=)%0A0%0A%0A%0AF10&=%2F_%0A-%0A%0A%0AF11&=+%0A%2F=%0A%0A%0AF12&_w:2%3B&=%0ABackspace%0A%0A%0ADel%3B&@_w:1.5%3B&=%0ATab&=Q%0A%0A%0A%0APrev&=W%0A%0A%0A%0APlay&=E%0A%0A%0A%0ANext&=R%0A%0A%0A%0AReset&=T%0A%0A%0A%0A15ms&=Y%0A%0A%0A%0ACal&=U%0A%0A%0A%0APgUp&_c=%23c7c3b5&t=%23ba1312%3B&=I%0A%0A%0A%0AHome&_c=%233c4041&t=%23aba18b%3B&=O%0A%0A%0A%0APgDn&=P%0A%0A%0A%0APrtSc&=%7B%0A%5B%0A%0A%0AScrlk&=%7D%0A%5D%0A%0A%0APause&_w:1.5%3B&=%7C%0A%5C%3B&@_c=%23c7c3b5&t=%23ba1312&w:1.25&w2:1.75%3B&=%0ACtrl&_x:0.5%3B&=A%0A%0A%0A%0AVol-&=S%0A%0A%0A%0AVol+&=D%0A%0A%0A%0AMute&=F%0A%0A%0A%0APgDn&_c=%233c4041&t=%23aba18b%3B&=G%0A%0A%0A%0A0.1s&_c=%23c7c3b5&t=%23ba1312%3B&=H%0A%0A%0A%0ALeft&=J%0A%0A%0A%0ADown&=K%0A%0A%0A%0AUp&=L%0A%0A%0A%0ARight&_c=%233c4041&t=%23aba18b%3B&=%2F:%0A%2F%3B%0A%0A%0AIns&=%22%0A'%0A%0A%0ADel&_w:2.25%3B&=%0AEnter%3B&@_w:2.25%3B&=%0AShift&=Z%0A%0A%0A%0AApp&=X&=C&=V&_c=%23c7c3b5&t=%23ba1312%3B&=B%0A%0A%0A%0APgUp&_c=%233c4041&t=%23aba18b%3B&=N%0A%0A%0A%0AEnd&=M%0A%0A%0A%0ADefault&=%3C%0A,%0A%0A%0ALayer%202&=%3E%0A.%0A%0A%0ALayer%203&=%3F%0A%2F%2F%0A%0A%0ALayer%204&_w:2.75%3B&=%0AShift%3B&@_c=%23c7c3b5&t=%23ba1312&w:1.25%3B&=%0AFN&_c=%233c4041&t=%23aba18b&w:1.25%3B&=%0AWin&_w:1.25%3B&=%0AAlt&_p=DCS%20SPACE&a:7&w:6.25%3B&=&_p=DCS&a:4&w:1.25%3B&=%0AAlt&_c=%23c7c3b5&t=%23ba1312&w:1.25%3B&=%0AWin&_c=%233c4041&t=%23aba18b&w:1.25%3B&=%0APn&_w:1.25%3B&=%0ACtrl)

## <a name="common_bindings"></a>Common key bindings for all OSs
* CapsLock always as Ctrl:
  * `CapsLock` then: `L_Ctrl` then: `PN` to confirm
  * `FN + CapsLock` then: `L_Ctrl` then: `PN` to confirm
* VIM like HJKL and Page Up/Down:
  * Left: `FN + H` then: `FN + J` then: `PN`
  * Down: `FN + J` then: `FN + K` then: `PN`
  * Up: `FN + K` then: `FN + I` then: `PN`
  * PgDown: `FN + F` then: `FN + O` then: `PN`
  * PgUp: `FN + B` then: `FN + U` then: `PN`
* Home: `FN + I` then: `FN + H` then: `PN`
* Volume controls:
  * Vol-: `FN + A` then: `FN + S` then: `PN`
  * Vol+: `FN + S` then: `FN + D` then: `PN`
  * Mute: `FN + D` then: `FN + F` then: `PN`

## <a name="Move_FN"></a>Move FN to L_Ctrl
HJKL as cursor keys are more ergonomical to reach by moving the FN to the left Ctrl key location:
* Switch to Layer 2 (or 3, 4); this programming is per layer
* Unplug keyboard
* DIP switch 4 to ON
* Plugin keyboard again, then press `FN` then: `L_Ctrl` then: `PN` then: `PN` (to leave it in its original location)
* DIP switch 4 back to OFF (no need to unplug)

## Sources
The how-to for these mappings is from 2 reddit threads:
* [r/mk: HowTo program pok3r](http://www.reddit.com/r/MechanicalKeyboards/comments/35uy60/guide_howto_program_your_pok3r_programming_layers/)
* [r/mk: HowTo media controls pok3r](http://www.reddit.com/r/MechanicalKeyboards/comments/37j3sx/guide_modification_pok3r_media_volume_controls_hw/)
 
<a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/4.0/88x31.png" /></a><br />This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/">Creative Commons Attribution-ShareAlike 4.0 International License</a>.
