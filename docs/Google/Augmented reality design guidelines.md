---
layout: default
title: Augmented reality design guidelines
parent: Google
---

# Augmented reality design guidelines
Original article: [Augmented reality design guidelines](https://developers.google.com/ar/design) 

## TL;DR
Google's AR design guidelines recommend creating immersive, user-friendly AR experiences with intuitive object interactions, smooth transitions, and well-defined object movement boundaries. To boost user engagement, visual and audio cues should encourage exploration, and clear error messages should assist users in rectifying errors. The interface should be visually clean, with a simple onboarding process. For multiplayer AR experiences, a seamless and intuitive shared virtual environment is crucial. The guidelines also advise on permissions and privacy, highlighting the importance of transparently communicating the need for specific app permissions.

## Bullet Points
1. 🎯 **Selection of virtual objects**: Enable users to select and interact with virtual objects seamlessly. This can be achieved through the use of highlighting techniques such as color differences, glowing outlines, or other distinct visual cues. The key is to ensure that these objects, despite their interactive potential, continue to behave like standard elements within the Augmented Reality (AR) environment. This reinforces the blended nature of the virtual and real world in AR.

2. 📦 **Translation of objects**: This refers to moving a virtual object along a surface or between different surfaces in the AR space. It is vital that this process is intuitive, either involving a simple on-screen dragging motion of the object or the physical movement of the device in the desired direction. The smoother the translation process, the more immersive the AR experience becomes.

3. 🌐 **Multiple surfaces**: Actively promote and facilitate the transition of virtual objects between various surfaces in the user's environment. This encourages the user to engage more dynamically with the AR world, thus enhancing the blend of virtual and real-world elements. However, be careful to avoid abrupt transitions or sudden changes in object scale as these can be jarring and disrupt the immersive experience.

4. 🛑 **Translation limits**: There should be clear and discernable boundaries that indicate the limits of an object's movement. This prevents situations where an object is moved beyond the field of view or to a distance that makes further interaction challenging. These boundaries can be indicated through visual cues such as grids, shadows, or changes in object color or opacity.

5. 🔄 **Rotation**: The AR design should allow users to rotate virtual objects freely in any direction. This can be manually controlled through touch gestures or can occur automatically through programmed animations. The design should be capable of supporting both single and multi-finger rotation gestures, offering a more interactive and flexible user experience.

6. 🔍 **Scaling**: Users should have the ability to alter the size of an object within the AR environment through gestures such as pinching or spreading fingers. However, to prevent an object from becoming either too small to see or too large for the AR space, designers should set minimum and maximum scaling limits.

7. ✋ **Gestures & Proximity**: When virtual objects are close together or overlap, it can be challenging for the user to select or interact with an individual object. To alleviate this, design should accommodate various two-finger gestures, such as pinching or a two-finger tap, to aid in distinguishing between close-proximity objects.

8. 🌈 **AR Initialization**: The transition from a 2D interface to the AR experience should be clear and smooth. Using visual cues such as a dimming display or a blurring effect can signal the impending transition to the user. Giving the user control over when the transition happens, such as through an 'Enter AR' button, can make the change less jarring.

9. 👥 **Multiplayer experience**: Aim to create a shared AR space where different users can interact with the same virtual objects. This can involve synchronizing surface detection across devices and providing visual or audio cues to guide users towards a shared space. Remember that multiplayer experiences can be complex, so aim to make the process of joining, connecting, and interacting as straightforward and user-friendly as possible.

10. 🎨 **UI Elements**: The User Interface (UI) should enhance, not detract from, the immersive AR experience. Avoid sudden pop-ups, full-screen takeovers, and persistent 2D overlays that constantly remind the user of the artificial nature of the AR world. The UI should be easy to navigate, employing familiar interaction models and supporting both landscape and portrait modes. This reduces the learning curve and allows users to focus more on the AR experience itself.

## Keywords
- **AR (Augmented Reality)**: This is a technology that superimposes a computer-generated image on a user's view of the real world, providing a composite view.
   
- **Translation**: In the context of AR, translation refers to moving a virtual object along a surface or from one surface to another.

- **Rotation**: This is the process of turning an object around in any direction in the AR environment.

- **Scaling**: In AR, scaling refers to the process of increasing or decreasing the size of a virtual object.

- **Gestures**: These are specific physical actions, like pinching or dragging, that a user performs to interact with their device in the AR environment.

- **Proximity**: In AR, proximity can refer to the relative distance or orientation of a user or object to other entities in the digital space.

- **Multiplayer Experience**: In AR, this refers to an experience where different users can interact with the same virtual environment.

- **UI (User Interface)**: This term refers to the graphical layout of an application. In AR, it includes the buttons users click on, the text they read, the images, sliders, and all the rest of the items the user interacts with.

- **Onboarding**: This is a term for the mechanism through which new users are introduced to an application. In AR, it can involve explaining how to interact with the virtual environment.

- **Error State**: This refers to a condition where the AR program or application encounters an unexpected situation or doesn't function as intended.
