---
layout: default
title: VR Locomotion Design Guide
parent: Meta
---

# VR Locomotion Design Guide
Original article: [VR Locomotion Design Guide](https://developer.oculus.com/resources/bp-locomotion/)

## TL;DR
In VR, user comfort is paramount. Different platforms offer varying mobility and fidelity. Achieving motion in VR can be physical or artificial, with potential for disorientation. Vection can cause discomfort when our eyes disagree with our balance sensors. Developers need to account for space limits, fatigue, accessibility, and predictability in movement to optimize user experience.

## Bullet points
1. 🖥 **VR Types**
VR devices can be grouped mainly into:
   - **PC-Tethered VR**: These are connected to computers and offer high-quality, graphic-intensive experiences, providing the most immersive experience.
   - **Standalone VR**: These are wireless devices offering flexibility and mobility, but they might trade-off a bit in terms of graphic quality.

1. 🌍 **World-Scale Tracking**
Using cutting-edge technology, modern VR devices capture a user's movement across a room. This real-time tracking of the user's full body movement accentuates the realism and immersiveness of the VR experience.

1. 🔄 **Locomotion in VR**
Movement in VR can be approached in multiple ways:
   - **Physical Locomotion**: Users move in real space, translated to VR.
   - **Artificial Locomotion**: Users remain stationary, but use controllers to move.
   - **Teleportation**: Users instantly move from one point to another.
   - **World Pulling**: Users "pull" or "drag" the virtual world around them.

1. ⚖ **Comfort & Usability**
To keep the VR experience engaging, it's vital to minimize sensory mismatches. The more the VR experience aligns with our real-world expectations, the more comfortable and intuitive it becomes.

1. 🧠 **Vection & Disorientation**
   - **Vection**: The illusion of self-movement based on visual cues. When visuals suggest movement, but the body remains still, this can lead to discomfort.
   - **Disorientation**: This occurs when there's a sudden change in camera perspective or location, making users lose their spatial bearings in the virtual world.

2. 🚶 **Physical Limitations & Fatigue**
Continuous physical activity in VR, like moving or turning, can lead to exhaustion. Designers must balance between physical interactivity and user comfort, taking into account varying user stamina and space limitations.

1. ♿ **Accessibility**
A well-designed VR experience is inclusive. It caters to everyone, regardless of their physical capabilities. This means ensuring that VR is usable for those seated, those with limited mobility, and those with other physical constraints.

1. 🧘 **Proprioception & Visual-Vestibular Mismatches**
   - **Proprioception**: The innate awareness of body position and movement. In VR, when our virtual representation doesn't align with our actual physical body, it can feel off.
   - **Visual-Vestibular Mismatch**: A prime cause of motion sickness in VR. When visuals indicate movement but the body doesn't feel it (or vice versa), it can result in discomfort.

2. 📖 **Consistency & Predictability**
In VR, the unexpected can be jarring. Ensuring that movement patterns, controls, and reactions are consistent helps users to predict actions in VR. This makes the environment feel more controlled and thus, more comfortable.

## Keywords
- **PC-Tethered VR**: VR devices connected to computers, generally offering high-quality, graphic-intensive experiences.

- **Standalone VR**: Wireless VR devices offering flexibility and mobility without the need for external computers or wires.

- **World-Scale Tracking**: Technology in VR devices that captures a user's movement across a room in real-time.

- **Physical Locomotion**: Movement in VR where users physically move in real space, and this movement gets translated to the virtual environment.

- **Artificial Locomotion**: Movement in VR where users remain stationary but use controllers or other input methods to simulate movement.

- **Teleportation**: A type of movement in VR where users instantly move from one point to another within the virtual environment.

- **Vection**: The illusory perception of self-motion based on visual input consistent with such movements, leading to a feeling of moving even when stationary.

- **Visual-Vestibular Mismatch**: Discrepancy between what the eyes perceive (vision) and what the inner ear senses (vestibular sense) regarding motion.

- **Proprioception**: The perception or awareness of body position and movement based on sensory information from muscles, joints, and skin.
