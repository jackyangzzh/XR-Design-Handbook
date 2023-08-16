---
layout: default
title: The Design & Implementation of Hand-tracking in ‘Myst’
parent: Road to VR
---

# The Design & Implementation of Hand-tracking in ‘Myst’
Original article: [The Design & Implementation of Hand-tracking in ‘Myst’](https://www.roadtovr.com/design-implementation-of-hand-tracking-in-myst-oculus-quest/)

## TL;DR
The article details hand tracking development for the VR game Myst using Unreal Engine. Custom solutions were implemented for gesture recognition, movement control, and multi-platform compatibility. The process highlights the complexity of creating a seamless hand tracking experience in VR.

## Bullet points
1. **👉 Pointing Mechanism for Movement**: The game adopts a natural pointing gesture for movement, allowing the player to teleport or move smoothly by pointing with their free-movement-dominant hand. To deal with inconsistencies in finger tracking when occluded, some adjustments were made to the code to ensure stable movement execution. This design leverages intuitive human gestures to enable seamless navigation within the game, incorporating extensive playtesting to find the perfect balance.
2. **👍 Thumbs-up Gesture for Turning**: Turning introduced complications with the pointing method, so a thumbs-up gesture was utilized instead. By giving a thumbs-up and rotating the wrist left or right, the player can turn smoothly or with snap turns. This solution, while not initially intuitive, was found to be the most comfortable and consistent way to enable turning within the game, showcasing the willingness to explore unconventional but effective design solutions.
3. **🚫 Handling Conflicts with Object Interaction**: Pointing is also a common interaction gesture, so the team had to distinguish between navigation pointing and interaction pointing. A range of 25 cm from the fingertip to the interactable object was established as the sweet spot to prevent unintended movement during interaction. This demonstrates the meticulous attention to real-world scenarios and user behaviors, enabling a more engaging and less frustrating player experience.
4. **✋ Designing Object Interactions with Hand Tracking**: Grabbable interactions were built to work with hand tracking by assessing when the fingers were curled enough to grab something, mimicking the behavior with Touch controllers. For buttons, capsule colliders between finger joints were used, allowing for diverse interaction methods. This multi-layered approach to hand interactions in Myst reflects a comprehensive understanding of both the technical possibilities and the intuitive user behaviors within a virtual environment.
5. **🖐️ Menu/UI Interactions**: To ensure consistency with existing user expectations, the two-finger pinch interaction paradigm from Meta's Quest Platform was used for menu interactions. This wise reuse of established interaction patterns demonstrates a user-centric approach to design, minimizing learning curves and allowing players to dive into the experience without the need to relearn basic interactions.
6. **📢 Communicating the Hand Tracking Experience**: Recognizing that hand tracking may be unfamiliar to some players, the team included specialized notifications and reminders for how to optimize hand tracking, such as proper lighting and keeping hands within the field of view. This emphasizes the team's commitment to user education and support, ensuring that players are set up for success and enjoyment within the game.
7. **🛠️ System Gesture Spam Fix & Multi-Platform Build Stability**: The Oculus left-hand system gesture was triggering prematurely during the pinch motion. The team resolved this by modifying the Oculus Input library to confirm the pinch completion before initiating the notify event. This ensures that the system gesture's confirmation circle is filled in before activating the associated event. A challenge was encountered with the Oculus Hand Component breaking builds for non-Windows and non-Android platforms like Xbox during nativization. The solution was to manage the Oculus Hand Component in C++, spawning and destroying it depending on hand tracking detection, and restricting this functionality to Android builds specifically for Quest.
8. **🎮 Custom Whole-Hand Gesture Recognition**: Unreal Engine lacked built-in functionality for recognizing specific whole-hand gestures like thumbs-up or finger-pointing. The team designed their own bone rotation detection within the Oculus Hand Component to recognize various hand gestures such as finger pointing, grabbing, and thumbs-up. These were then transformed into input events accessible in C++, enabling more intuitive and versatile player interactions.
9. **🤏 Gesture & Tracking Stability Adjustments**: The document outlines quirks in tracking stability for particular hand gestures, such as grabbing with fingers facing away or pointing the index finger directly away. Tracking inaccuracies were noted in these scenarios, sometimes misinterpreting the hand's pose. The solution was to implement individual finger thresholds to control how relaxed a finger could be before it was considered 'not grabbing' or 'not pointing.' This enabled more precise and consistent gesture interpretation.
10. **🧰 Other Handy Utilities for Oculus Hand Component**: The team introduced additional modifications and utility functions to the Oculus Hand Component. One example is a utility to find the closest point on the hand's collision from another point in world space, returning the name of the closest bone. This allowed for enhanced input verification across interactions. A consistent tracking point, such as the wrist bone, was frequently used for reliability across different hand depths.

## Keywords
- **Gesture Detection**: Technology recognizing human gestures through algorithms.
- **System Gesture Spam Fix**: Specific solution to a problem with early triggering of gestures.
- **Multi-Platform Build Stability**: Development of software for multiple platforms.
- **Nativization**: Converting Blueprint scripts into C++ in Unreal Engine.
- **Blueprint**: Visual scripting system in Unreal Engine.
- **Bone Rotation Detection**: Detecting positions and movements of virtual hands.
- **Pointing Mechanism**: Method using a pointing gesture for game control.
- **Teleport Mode**: Instantly moving to a pointed destination in the game.
- **Smooth Movement Mode**: Continuous movement in a directed path by hand pointing.
- **Occluded**: An object hidden from view, interfering with tracking.
- **Fudge Factor**: Tweak or adjustment made to code for stable movement.
- **Turning**: Action of rotating player's view in the game.
- **Wrist Rotation**: Turning of the wrist, related to game gesture.
- **Snap Turning**: Instant turning to a new direction in the game.
- **Interactable Object**: Object that player can engage with in the game.
- **World Space Location**: Coordinate system defining 3D object locations.
- **Colliders**: Used to detect collisions between objects in games.
- **OS-level Menus**: Operating system menus for configuring settings.
