# Problem with Logitech MX Master 3S mouse

My mouse behaves good at moving, clicking, scrolling after a fresh installation. But it always responses noticable latency on Drag-and-Move actions. Sometime, the delay is more than 300ms. It is quite annoying.

I tried other mice, like Apple MagicMouse, Dell wire mouse, all perform good without the delay.

Until, I re-pair the mouse and unifying receiver. The problem is fixed.

Install the pairing tool, `ltunify`

```shell
$ yay -S ltunify
```

Unpair and re-pair the mouse

```shell
$ ltunify unpair mouse
$ ltunify pair
Please turn your wireless device off and on to start pairing.
Found new device, id=0x01 Mouse
$ ltunify list
```

Now, the delay should be disappered when drag-and-move.

References:
- [Logitech Unifying Receiver](https://wiki.archlinux.org/title/Logitech_Unifying_Receiver)