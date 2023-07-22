---
layout: default
title: Mixed Reality Design Guidelines
parent: Meta
---

# Mixed Reality Design Guidelines
Original article: [Mixed Reality Design Guidelines](https://developer.oculus.com/resources/mr-design-guideline/)

## TL;DR
This article discusses how Passthrough technology in VR/AR applications can improve user experiences by increasing real-world awareness. It covers the use of Passthrough as a background, reducing onboarding friction, creating selective windows, and providing tips on stylization, occlusions, and shadows. The Insight SDK is mentioned as a tool for developers to control blending and lighting effects, enhancing user immersion and engagement in virtual and augmented reality environments.

## Bullet points
1. 👀 **Passthrough as a Background:** When used as a background, Passthrough technology allows users to see and interact with the real world while also experiencing virtual elements. This feature not only boosts real-world awareness but can also enhance user engagement by providing AR-like experiences in VR applications.
2. 🌐 **Reducing VR Onboarding Friction:** To ease new users into the VR experience, Passthrough can be utilized to guide users from their actual environment to a fully immersive virtual realm and back. This gradual transition could potentially foster higher adoption rates of VR applications.
3. 🪟 **Selective Passthrough:** Developers have the ability to create "windows" into the real world within the VR environment. These "windows" can provide partial views of the user's physical surroundings and facilitate transitions between real and virtual realities.
4. 🔄 **Transitioning between Realities:** When presenting users with multiple realities, it's essential to clearly define the transitions. Unless there's a direct correspondence or 1:1 match between the virtual and physical spaces, mixing realities can confuse users. 
5. 🎨 **Stylizing Passthrough:** The camera sensors on Quest and Quest 2 are black and white. Developers can choose to show Passthrough as-is or stylize it to achieve an artistic look. Use of color can draw attention towards virtual elements and heighten user experience.
6. ⚡ **Highlighting Moments with Stylization:** Animation and stylization effects can be employed to emphasize certain moments for the user, such as transitioning from the real world to a virtual one or accomplishing an achievement.
7. 🕳️ **Realistic Virtual Content with Occlusions and Shadows:** Using occlusion and shadow effects can make virtual content appear more realistic within the physical world, thus enhancing Mixed Reality experiences. Without proper occlusion, VR objects can seem like they're floating in the Passthrough view.
8. 👓 **Blending Passthrough over Virtual Content:** Developers can blend Passthrough over virtual content, employing stylistic effects like outlines for more appealing and less distracting visuals. Outlines are particularly effective as they can contrast with the virtual background.
9. 💡 **Naive Lighting:** By adjusting the transparency of a black background, applications can create an illusion of lighting and dimming in the environment. This technique can enhance the user's immersion by suggesting that the environment is dynamically responding to their actions.
10. 🎮 **Insight SDK for Blending Control:** The Insight SDK provides developers with the tools to control the blending of Passthrough and their applications. This allows for creative utilization of lighting and transitions, enhancing user immersion and experience.


## Keywords
1. **Passthrough:** In the context of virtual or augmented reality, Passthrough refers to a feature that allows users to see the real world around them while wearing a VR/AR headset.
2. **Spatial Anchor:** A spatial anchor is a point of reference used in augmented and mixed reality experiences to keep virtual objects correctly positioned in the real world as viewed through a device.
3. **Scene:** In the context of VR/AR, a scene is the virtual environment or space that the user can interact with.
4. **Onboarding:** The process of integrating a new user into a system, service, or product, teaching them how to use it.
5. **Selective Passthrough:** A feature where only certain parts of the real-world view are shown in a VR environment.
6. **1:1 Match:** A perfect correspondence between two sets of things; in this context, it refers to the matching between virtual and physical spaces.
7. **Stylization:** The process of designing or presenting in accordance with a style or stylistic pattern.
8.  **Occlusions:** In the context of VR/AR, occlusion refers to the effect where an object appears to be blocked by another, adding to the realism of the scene.
9.  **Insight SDK:** A Software Development Kit provided by Oculus that provides features to help developers create VR experiences.
10. **Naive Lighting:** A method of manipulating lighting in VR experiences by adjusting the transparency of elements, creating an illusion of the real environment being lit or dimmed.
