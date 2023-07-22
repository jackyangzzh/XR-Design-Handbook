---
layout: default
title: User Input 
parent: Meta
---

# User Input 
Original Article: [User Input](https://developer.oculus.com/resources/bp-userinput/)

## TL;DR
The article discusses best practices for designing user interfaces for VR devices, particularly with 3DOF and 6DOF controllers. Recommendations include maintaining a 1:1 movement ratio, standard button mapping, and accommodating left and right-handed users. It also covers the complexities of hand registration, interaction with the virtual world, and using haptics to improve user experience. The challenge of replicating real-world physics in VR is noted, with a strong emphasis on designing believable and comfortable object interactions.

## Bullet Points
1. 🕹️ **VR Controller Types:** The two main types of VR controllers are 3DOF and 6DOF. 3DOF controllers, common in mobile VR devices, allow for orientation tracking but not spatial tracking. 6DOF controllers, on the other hand, can track both orientation and position in space, making them more suitable for advanced VR systems like the Rift.

2. 👍 **User Input Recommendations:** For a successful VR experience, it's crucial to maintain a 1:1 movement ratio between the real-world controller and its virtual representation. Using standard button mappings and touch/controller-based menus can also make your VR application feel more intuitive and familiar to users.

3. 👥 **Accommodating User Preferences:** VR systems should be designed to accommodate users of all kinds, including left-handed and right-handed individuals. If two controllers are used, allow interactions with both hands; if only one is available, respect the user's default hand setting.

4. 📱 **3DOF Best Practices:** 3DOF controllers work well as pointing devices for interacting with UI elements. They shouldn't be represented as hands in-app due to their limited capabilities. Use the controller touchpad for navigating through menus and aim at objects in VR with the ray-cast pointer, which should be on at all times for clarity.

5. 👐 **6DOF Best Practices:** For 6DOF controllers, the representation of hands in VR is crucial for immersion. Poorly implemented hand registration can lead to discomfort, so it's essential to ensure that the virtual hand's position and orientation match the user's actual hand. Allowing customization of hand appearance can also improve user comfort.

6. 📐 **Implementing Hand Registration:** Testing for hand registration can be done using the "back of the hand" test, and to get the best results, the controller model should be placed in the scene accurately. Getting the registration right can avoid the "uncanny hand valley" effect.

7. 💫 **Interactions with Virtual Objects:** Virtual objects should be designed with consideration of their perceived weight to maintain believability, as controllers can't simulate resistance or torque. Using physical and ethereal hand models simultaneously can help manage hand-object intersections.

8. 💡 **Lightweight Interactions:** Since VR can't simulate the physical resistance of real-world interactions, stick to lightweight interactions for believability. Lifting a light switch, for example, is more believable than lifting a heavy rock in VR.

9. 🤲 **Two-Handed Interactions:** Designing interactions requiring two hands can be challenging in VR due to the lack of physical constraints. Be cautious when implementing these types of interactions.

10. 🔊 **Use of Haptics:** Using haptics (tactile feedback) can significantly improve the VR experience. They can be used to simulate the feeling of throwing and catching virtual objects, which increases user immersion.

## Keywords
1. **3DOF (3 Degrees of Freedom)**: This refers to a controller that allows for orientation tracking but does not track the controller's position in space.
2. **6DOF (6 Degrees of Freedom)**: This term describes a controller that supports both orientation and positional tracking. These controllers are usually used in pairs, allowing users to have "virtual hands" in the VR environment.
3. **Proprioceptive Mismatch**: This is a mismatch between the perceived location or movement of a virtual limb and the actual location or movement of the real limb. Such a mismatch can cause discomfort in the VR user.
4. **Hand Registration**: This refers to the process of aligning the virtual hand model with the user's actual hand, making it feel like the virtual hands are their own. Good hand registration is critical for a comfortable and immersive VR experience.
5. **Haptics**: This involves the use of tactile sensations to provide feedback to the user in a virtual environment. This could be in the form of vibrations or resistances.
6. **Occlusion**: In the context of VR, occlusion refers to the obstruction of a sensor's view of the controller or headset, which can affect tracking accuracy. This term is mentioned in the context of avoiding the need for users to pick up objects off the floor, where sensors may not track accurately.
7. **IK Arm**: IK or Inverse Kinematics is a technique used in 3D animations to make movements appear more realistic. An "IK Arm" would be a digital arm that is animated using inverse kinematics. In this case, it's suggested not to use this technique as it can lead to proprioceptive mismatch.