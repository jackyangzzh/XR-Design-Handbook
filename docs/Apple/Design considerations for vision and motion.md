---
layout: default
title: Design considerations for vision and motion
parent: Apple
---
# Design considerations for vision and motion
Original video: [Design considerations for vision and motion](https://developer.apple.com/videos/play/wwdc2023/10078/)

## TL;DR 
The video discusses designing immersive experiences with focus on visual and motion comfort. It advises using depth cues and optimizing visual parameters to reduce eye strain. For motion, it recommends ensuring stability, limiting head-locked content, and wisely managing camera movements to prevent discomfort.

## Bullet Points
- 🧠 **Understanding Depth Perception:** Design immersive experiences that align with the brain's interpretation of depth. This requires the use of correct visual depth cues like size, blur, motion, background, light, shadow, occlusion, and texture density. These cues enable the viewer's brain to converge the line of sight correctly, preventing discomforts such as double vision or eye fatigue.
- 🚫 **Avoiding Visual Cue Conflicts:** Ensure there are no conflicting depth cues. Misalignments, like an object appearing larger but positioned behind a smaller one, can cause discomfort due to conflicting information about depth. All depth cues should consistently give the brain correct information, aligning the viewer's eyes to the depth intended.
- 🔄 **Addressing Misleading Visual Cues:** Patterns can mislead depth perception. If each eye locks onto a different object in a repeating pattern, the resulting image may be perceived at a different depth than intended, causing discomfort. To mitigate this, use smaller portions of patterns or break them up with different designs.
- 👓 **Optimizing Content Parameters:** Design visually comfortable content with parameters suited for each specific visual experience. Considerations include content size, contrast, and brightness. High contrast is beneficial for reading text, while lower contrast, transparency, or blur can redirect visual attention.
- 👁️ **Reducing Eye Effort:** Minimize eye effort by placing content in comfortable viewing areas, primarily the center and slightly below the line of sight. Consider natural break points in the experience to allow for rest, and adjust content parameters based on the visual effort demanded from the viewer.
- 🔄 **Maintaining Motion Comfort:** The brain needs to perceive the world as stationary for motion comfort. Conflicts between visual motion information and the motion perceived by the vestibular system can cause discomfort. Ensuring stable and well-designed content helps to avoid this.
- 💠 **Managing Virtual Object Motion:** For large virtual objects that move, making them semi-transparent can avoid giving the viewer a sense of self-motion, ensuring motion comfort. 
- 🚫 **Avoiding Head-Locked Content:** Head-locked content, anchored to the user's head, can cause discomfort. Instead, use world-locked views or lazy-follow animations that move content slowly towards a destination over time.
- 🖼️ **Handling Window Motion:** To provide optimal motion comfort, align the virtual window's horizon with the real horizon and keep camera motion and the focus of expansion slow and predictable.
- 🌊 **Avoiding Sustained Oscillations:** To ensure a comfortable experience, avoid oscillating motions, especially those with frequencies around 0.2 Hz. If such motions are necessary, keep the amplitude low, make the content semi-transparent, and provide an oscillation-free alternative.

## Bullet Points
- **Visual Depth Cues:** Signals given to the brain about the spatial relationships of objects, aiding in perceiving depth. They include size, blur, motion, background, light, shadow, occlusion, and texture density.
- **Converge:** The inward turning of the eyes to fixate on a near object. In this context, it refers to the viewer's eyes aligning to perceive the intended depth of an object in a 3D space.
- **Double Vision:** A condition where an individual sees two images of a single object. It can occur if the viewer's eyes aren't aligning correctly due to inconsistent or misleading visual depth cues.
- **Disparity:** The difference in image location of an object seen by the left and right eyes. Correct disparity is essential for comfortable stereo viewing.
- **Eye Effort:** The amount of effort or strain the eyes undergo to view certain content. Reducing eye effort, by adjusting content location and parameters, enhances comfort.
- **Head-Locked Content:** Content that maintains a fixed position relative to the user's head movement. In immersive experiences, world-locked or lazy-follow content is preferred to enhance comfort.
- **Vestibular System:** The sensory system responsible for motion perception, head position, and spatial orientation. Conflicting visual and vestibular motion information can cause discomfort like dizziness or nausea.
- **Oscillations:** Regular back-and-forth movements. Sustained oscillations, especially at around 0.2 Hz, can be visually uncomfortable and should be minimized or made less perceptible.
- **Focus of Expansion:** The point in a visual scene where all motion vectors originate, towards which all movement seems to head. Slow and predictable motion of this point aids in motion comfort.
- **Reduce Motion Accessibility Setting:** A feature that minimizes certain interface movement effects to provide a simpler visual experience. Designers should offer oscillation-free alternatives when this setting is activated.
