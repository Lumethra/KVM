# KVM
## What is this?

Its a KVM, just there is a catch, it should be a KM, because it doesnt fulfill the criterias for the "V". A KVM is a device that can let you switch the connected USB-devices from one PC to another, so just press or toggle the switch and your mouse and keyboard are connected to the other device, for example a laptop. KVM stands for Keyboard, Video, Mouse and since my thingi only supports USB-devices it only supports keyboards, mice and maybe other usb devices. Thats also why I would call it a KM. 

### Features:
  - 2 USB-C-upstreams
      - for the 2 PC's
  - 4 USB-downstreams
      - 2 USB-C
      - 2 USB-A
  - 1 SL2.1S to bundle the 4 downstreams into 2 pins (D+, D-)
  - 1 Mux to switch between the 2 upstreams for PC switching
  - 1 slider, toggle, switch kinda thingi to set the state

---

## Why?

I thought it would be funny to try that out. It turned out to be quite easy. I also thought about USB3.0 and even USB4.0, but that was too complicated and I settled on USB2.0. A KVM is also sth that you can use in your daily workflow and could turn out to be really handy. 

---

## How??

It was simply replicating the USB-Hub, which I made for my keebs and connecting the upstream to the mux which handles the switching between the 2 USB-C(2.0) to archieve the switching between devices. 

---

## Renders 
> enjoy the raytracing

| PCB with Components | 
| --- |
| <img alt="KVM Front with Components" src="https://github.com/Lumethra/KVM/blob/main/Images/KVM-Front.png" /> |
| <img alt="KVM Back with Components" src="https://github.com/Lumethra/KVM/blob/main/Images/KVM-Back.png" /> |

| PCB without Components |
| --- |
| <img alt="KVM Front without Components" src="https://github.com/Lumethra/KVM/blob/main/Images/KVM-Front-No-Components.png" /> |
| <img alt="KVM Back without Compoenents" src="https://github.com/Lumethra/KVM/blob/main/Images/KVM-Back-No-Components.png" /> |

---

## PCB + Schematics

| Schematics |
| --- |
| <img alt="KVM-PCB" src="https://github.com/Lumethra/KVM/blob/main/Images/KVM-Schematics.png" /> |

| PCB |
| --- |
| <img alt="KVM-Schematics" src="https://github.com/Lumethra/KVM/blob/main/Images/KVM-PCB.png" /> |

---

<details>
  <summary>
    <h2>Zine</h2>
  </summary>

| Zine |
| --- |
| <img alt="KVM-Zine" src="https://github.com/Lumethra/KVM/blob/main/Images/zine.png" /> |

  ---
</details>

## BOM

| Part | Purpose | Cost | Quantity | Total Cost | LCSC/JLCPCB Number | Link |
| --- | --- | --- | --- | --- | --- | --- |
| PCB |connect everything together | $2 | 1(5) | $2 | ~ | [JLCPCB](https://jlcpcb.com) |
| Capacitors | reduce noise in the power | $0.0032 | 8 | $0.0256 | C15849, C14663 | [C15849](https://jlcpcb.com/partdetail/C15849) / [C14663](https://jlcpcb.com/partdetail/C14663) |
| Resistors | prevent things go boom | $0.0016 | 8 | $0.0138 | C23186, C23206 | [C23186](https://jlcpcb.com/partdetail/C23186),[C23206](https://jlcpcb.com/partdetail/C23206) |
| Toggle Switch | say which computer | $0.0579 | 1 | $0.0579 | C431541 | [JLCPCB](https://jlcpcb.com/partdetail/C431541)  |
| USB Mux | change computer (USB) | $0.3720 | 1 | $0.3720 | C42407092 | [JLCPCB](https://jlcpcb.com/partdetail/C42407092)  |
| USB Hub | bundle the downstream | $0.2258 | 1 | $0.2258 | C2684433 | [JLCPCB](https://jlcpcb.com/partdetail/C2684433)  |
| UCB-C | usb connectors | $0.0740 | 4 | $0.2960 | C2765186 | [JLCPCB](https://jlcpcb.com/partdetail/C2765186)  |
| USB-A | usb connectors big | $0.0636 | 2 | $0.1272 | C668591 | [JLCPCB](https://jlcpcb.com/partdetail/C668591)  |

> the prices can change depending on the provider and time <br>
> you can find the JLCPCB parts on [LCSC](https://lcsc.com/) too (exept the PCB) <br>

---

## Contribute

Want to add something?? Want a real KVM with Video? Found any bugs?? Feel free to open a PR (pull request) or an issue. 
> the libraries are all imported with [easyeda2kicad](https://github.com/uPesy/easyeda2kicad.py)

---

## Thank you

A huge thank you to my brain, who didnt die in this session. Another huge thank you to all the guys teaching me hardware. A last thank you to my laptop and kicad who dont like each other and decides to crash alot. 
