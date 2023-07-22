---
layout: default
title: Comfort and Content Placement
parent: Magic Leap
---

# Comfort and Content Placement
Original article: [Comfort and Content Placement](https://developer-docs.magicleap.cloud/docs/guides/best-practices/comfort-content-placement)

## TL;DR
When creating immersive experiences for headsets, ensure custom fit, place important content within a 30°x30° area, use visual effects sparingly, and adapt the interface to user movements to avoid discomfort and disorientation.

## Bullet points
1. 🖥️ **Device Fit Quality**: Users should use the Custom Fit application for optimal performance and comfort in the headset. This improves the visual comfort experience by tailoring the device to the individual's physical needs.

2. 🎯 **Content Placement**: The location and proximity of content to the user is crucial for maintaining comfort. If content is too close (less than 0.37m), it may lead to discomfort. However, with a Custom Fit, content further than 0.37m will be comfortable for most people.

3. 🚅 **Moving Content**: Content in motion, especially in the Z-axis (i.e., forward/backward), can cause visual discomfort. Designing content to limit the need for extended periods of viewing movement can help minimize discomfort.

4. 🕺 **User Movement**: Consider the natural tendencies of users to move their head or body while using the device. Creating flexible UI behaviors that can adapt to these movements can help improve user comfort and usability.

5. ✨ **Visual Effects**: Certain visual effects such as lense-distortion, chromatic aberration, and depth of field may disorient users. They should be used judiciously to avoid inducing a sense of distorted vision.

6. 📏 **Clipping Plane**: The default near clipping plane is set at 0.37m to prevent discomfort caused by content appearing too close to the user. Viewing content any closer than this is not advisable as it can cause nausea. 

7. 📐 **Optimal Content Placement Area (OCPA)**: The OCPA is a 30°x30° boundary within which content is visible to users at all times, without moving their head. Essential content should be placed within the OCPA to ensure that it's always visible to the user.

8. 👀 **Field of View (FOV)**: Due to facial size and shape variance, every individual will not have a similar virtual FOV visible. Designers should account for this variation when designing content placement.

9. 🤲 **Interaction Ergonomics**: The placement of content relative to the user should be considered in the context of the expected user experience (controller or gesture). For direct inputs, content should be within arms' reach (0.4-0.6m). For indirect inputs, content should be beyond 0.6m.

10. 🕹️ **UI Behavior**: UI behavior should be designed taking into account how and where the user may move. Various UI behaviors include head-relative, body-relative, world-relative, and input-relative. Each behavior has its own use-cases and limitations and should be chosen accordingly.

## Keywords
- **Custom Fit**: An application designed to optimize the fit and performance of a device.
- **Focal Plane**: The distance at which the eye is comfortably focused.
- **Clipping Plane**: Invisible boundary in 3D rendering which limits the rendering of objects, set at 0.37m (near) and 10m (far).
- **Z Axis**: Depth axis in 3D space, indicating forward/backward motion.
- **Lense-Distortion, Chromatic Aberration, Depth of Field**: Visual effects which may cause discomfort, disorientation or sense of distorted vision.
- **Optimal Content Placement Area (OCPA)**: A 30°x30° boundary for optimal visibility of content without moving the head.
- **Direct/Indirect Inputs**: Types of user interaction, with content placed within arm's reach (direct) or beyond (indirect).
- **Head-Relative, Body-Relative, World-Relative, Input-Relative**: Strategies for designing UI behavior, each attached to different user positions or movements.
- **Micro-Movements, Macro-Movements**: Smaller and larger user movements to be considered in UI design, such as swaying or walking across a room.
- **System Overlays**: Elements like system notifications, voice command UI, and privacy indicator UI that may appear within an application.