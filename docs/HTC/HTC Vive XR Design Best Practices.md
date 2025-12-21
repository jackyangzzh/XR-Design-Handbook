---
layout: default
title: HTC Vive XR Design Best Practices
parent: HTC
---

# HTC Vive XR Design Best Practices
Original sources: [HTC Vive Developer Resources](https://developer.vive.com/resources/), [Unity XR Guidelines](https://learn.unity.com/tutorial/best-practices-for-user-interfaces-ui-in-vr-with-the-xr-interaction-toolkit), [XRgonomics Research](https://dl.acm.org/doi/fullHtml/10.1145/3411764.3445349)

## TL;DR
HTC Vive XR design emphasizes world-space UI placement over head-locked interfaces, spatial interactions using gaze and gestures, ergonomic positioning to minimize fatigue, multi-modal accessibility, and real-time feedback. Developers should anchor UI elements to the virtual environment, design for comfortable reach zones, support diverse input methods, and continuously test across different user profiles to create immersive, comfortable experiences.

## Bullet points

1. 🌍 **World-Space UI Design**: Place UI elements in world space anchored to surfaces or objects in the virtual environment rather than attaching them to the user's view. This "in-world" approach maintains immersion by making interfaces feel organic to the scene, avoiding the uncomfortable "sticky note on face" effect that head-locked UI creates, and reducing user fatigue from constant visual adjustment.

2. 🤲 **Spatial Interaction Modalities**: Design for intuitive spatial interactions using gaze direction, hand gestures, and controller input. Ensure interactions feel natural by making buttons and switches exist as graspable 3D objects users can reach for and manipulate. Provide clear affordances so users immediately understand what actions are possible, reducing cognitive load and confusion during interactions.

3. ⚡ **Minimize Physical Fatigue**: Arm and hand fatigue is a critical concern in mid-air XR interaction. Use ergonomic modeling tools like XRgonomics to visualize interaction costs and identify fatigue hotspots. Place UI elements within comfortable reach zones—typically between waist and shoulder height, 40-60cm from the user—and avoid requiring extended or repetitive gestures that strain muscles.

4. 📐 **Ergonomic Positioning and Reach**: Design interactive elements considering the envelope of comfortable movement. Keep frequently used controls near the user's rest position and within natural arm extension. Avoid placing UI too close (causing neck strain or eye fatigue) or too far (requiring stretching or excessive motion). Dynamic adjustment based on user height and arm length enhances comfort across diverse demographics.

5. ♿ **Multi-Modal Accessibility**: Integrate multiple input methods including voice commands, gaze-based selection, gesture controls, and motion-agnostic alternatives for users with mobility or cognitive impairments. Following WCAG and WebXR API guidelines ensures experiences are customizable and inclusive, allowing all users to interact comfortably regardless of physical capabilities or preferences.

6. 🎯 **Clear Affordances and Feedback**: Provide immediate visual, haptic, and auditory feedback for every user action. Design interface elements with obvious interaction cues so users intuitively understand what's clickable, draggable, or manipulable. Consistent feedback reinforces engagement, makes interfaces feel responsive and alive, and helps users confidently navigate the virtual environment.

7. 🔄 **Adaptive Interface Design**: UI should dynamically adapt to different user heights, arm lengths, and physical constraints using real-time tracking data. This personalization ensures comfort and accessibility across populations with varying physical attributes. Interfaces that respond to individual user characteristics provide better experiences than one-size-fits-all approaches.

8. 📱 **Context-Aware UI Behavior**: Evaluate the form factor capabilities—whether room-scale, seated, or standing XR—and design context-specific interactions. Target appropriate interaction ranges and UI sizing based on the expected use case. Room-scale experiences require different considerations than seated experiences, affecting optimal placement and interaction distance.

9. 🎨 **Consistent Spatial Metaphors**: Adapt familiar interface patterns like buttons and icons to 3D space while respecting spatial affordances. Don't blindly port 2D design practices; instead, leverage depth, scale, and spatial relationships. Design for the unique capabilities of 3D interaction while maintaining intuitive patterns users understand from previous experiences.

10. 🔍 **Continuous User Testing**: Arm and hand fatigue, interaction confusion, and accessibility barriers are often only revealed through real user testing. Regularly prototype and test designs with diverse user profiles including different physical abilities, experience levels, and body types. Iterate based on feedback to continuously improve comfort, usability, and inclusivity of XR experiences.

## Keywords

- **World-Space UI**: User interface elements positioned and anchored within the 3D virtual environment rather than locked to the user's view or head position.

- **Affordance**: Visual or physical characteristic of an interface element that suggests how it should be used without requiring explicit instructions.

- **Ergonomics**: Study of designing equipment and interfaces that fit human body capabilities and limitations, minimizing fatigue and maximizing comfort.

- **XRgonomics**: Specialized toolkit and methodology for evaluating and optimizing ergonomic factors in XR interface design, measuring interaction costs and fatigue.

- **Multi-Modal Interaction**: Supporting multiple simultaneous or alternative input methods (voice, gaze, gesture, controller) to accommodate different user preferences and abilities.

- **WCAG (Web Content Accessibility Guidelines)**: International standards for making digital content accessible to people with disabilities, applicable to XR experiences.

- **WebXR API**: JavaScript API for creating immersive VR and AR experiences in web browsers with built-in accessibility considerations.

- **Haptic Feedback**: Tactile sensations and vibrations that provide physical responses to user actions in virtual environments.

- **Reach Envelope**: The 3D volume of space a user can comfortably access with their arms without straining or excessive movement.

- **Gaze-Based Selection**: Interaction method where users select objects or UI elements by looking at them, often combined with a dwell time or confirmation action.

- **Room-Scale VR**: VR experience designed for users to physically walk around a designated play area, requiring tracking of full body movement.

- **Head-Locked UI**: Interface elements that maintain fixed position relative to user's head, moving with every head movement (generally discouraged).

- **OpenXR**: Open standard for XR platform APIs, enabling cross-platform development across different VR/AR hardware.