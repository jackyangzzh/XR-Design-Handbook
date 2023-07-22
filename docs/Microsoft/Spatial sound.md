---
layout: default
title: Spatial sound
parent: Microsoft
---

# Spatial sound
Original article: [Spatial sound](https://learn.microsoft.com/en-us/windows/mixed-reality/design/spatial-sound)

## TL;DR
Spatial sound in mixed-reality environments, using head-related transfer function (HRTF), augments user experiences by providing auditory cues that inform about application states, reinforce interactions, and simulate real-world sound propagation. While enriching the immersive quality, developers are advised to exercise restraint in sound use to maintain usability and avoid cognitive overload.

## Bullet Points
1. 🔈 **In low-light situations, our sense of hearing keeps us safe**: This capability evolved as a survival mechanism, allowing humans to react to unseen threats and obstacles, even in the dark. In technology, this concept is used to create more immersive and intuitive experiences.

2. 🎧 **HoloLens utilizes spatial audio to enhance mixed reality experiences**: Spatial audio creates a more realistic soundscape by simulating sounds from various directions and distances, increasing immersion and aiding user orientation within the virtual environment.

3. 👓 **The field of view in HoloLens devices is directly in front of the viewer**: Due to this limitation, only objects directly in front of the user are visible, making peripheral vision less informative in these mixed reality environments.

4. 🔊 **Speakers on HoloLens use HRTF audio to simulate sound from various distances and directions**: By employing Head-Related Transfer Function audio, HoloLens is able to create an audio environment that realistically represents how we would perceive sound in the real world, augmenting the immersion in mixed reality.

5. 👂 **Our ears help us determine the distance and direction of a sound**: We naturally process small differences in the time and intensity of sounds reaching each ear, allowing us to locate their sources in the space around us.

6. 🎼 **HRTF audio simulates this experience through timing differences and spectral changes**: HRTF audio uses mathematical models to recreate these auditory cues, simulating the intricacies of how sound waves interact with our heads and ears.

7. 🔄 **HoloLens speakers mimic this experience by simulating sound arrival at different times**: By carefully controlling when sounds reach the user's ears, the system can create the impression of sound sources located at different positions in the space around the user.

8. 💻 **HoloLens spatial audio offers extensive functionality for developers**: It allows the placement and movement of sound sources in 3D space, enabling developers to create highly immersive and interactive audio environments.

9. 🎛️ **Developers can manipulate the source of the audio on a frame-by-frame basis**: This feature allows developers to precisely control where a sound appears to originate from, creating a highly dynamic and interactive audio experience.

10. 🎚️ **Play, stop, pause, resume, loop, and fire-and-forget sound assets can be controlled by developers**: These functions provide developers with granular control over audio playback, allowing them to finely tune the audio experience to match visual or interactive elements in the mixed reality environment.

## Keywords
1. **Spatial audio**: A technique for creating a three-dimensional sound field, giving the illusion of sound coming from various directions and distances.
2. **HoloLens**: A pair of mixed reality smart glasses developed and manufactured by Microsoft.
3. **Field of view**: The observable area that can be seen at a particular moment.
4. **HRTF (Head-Related Transfer Function) audio**: A response that characterizes how an ear receives a sound from a point in space, used in sound synthesis and spatial audio to simulate directionality.
5. **Spectral changes**: Modifications in the frequency content of a signal.
6. **Pinna**: The visible part of the ear that resides outside the head.
7. **Frame-by-frame basis**: In this context, it refers to the ability to change audio sources for each frame in a sequence, allowing for very detailed control over sound localization.
8. **Fire-and-forget sound assets**: This refers to playing a sound asset and not needing to control it further once it's started.