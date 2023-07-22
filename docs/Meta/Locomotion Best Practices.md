---
layout: default
title: Locomotion Best Practices
parent: Meta
---

# Locomotion Best Practices
Original article: [Locomotion Best Practices](https://developer.oculus.com/resources/locomotion-design-techniques-best-practices/)

## TL;DR
The article explores various methods to improve comfort and decrease motion sickness in VR experiences. These include maintaining a steady frame rate and precise head tracking, using Asynchronous Time Warp to reduce judder, and leveraging Independent Visual Backgrounds to lower discomfort, exemplified by a skybox reacting only to head movements. The benefits and implementation challenges of IVBs in VR applications are discussed. Simulated activities, like walking in place or climbing a ladder, are suggested as additional comfort-boosting techniques. Spatial sound effects are recognized for their role in reducing disorientation, especially during teleportation movements.

## Bullet Points
1. **🌄 Minimize Movement on Slopes:** Slopes and stairs increase discomfort in virtual environments due to the vertical accelerations and the induced vection. By limiting movement to flat terrains, users can have a more comfortable experience.

2. **🚶‍♂️ Design for Forward Movement:** People find forward movement most comfortable in VR environments. Strafing, back-stepping, and spinning should be minimized as they increase the likelihood of discomfort.

3. **🏰 Keep Walls at a Distance:** Walls and large structures that are close to the user can increase optic flow, which leads to discomfort. To mitigate this, design environments with open spaces or with barriers that distance users from walls.

4. **🏢 Elevator and Stair Design:** Stairs and elevators are filled with visual cues that can fill the user's field of view, potentially triggering discomfort. When necessary, design them to be less detailed and simple to minimize optic flow.

5. **⛰️ Stair & Slope Teleports:** In certain instances, it might be helpful to provide teleport nodes at the top and bottom of stairways. This offers an option for users who prefer to navigate without dealing with the discomfort that stairs might induce.

6. **🖼️ Consistent Frame Rate and Head Tracking:** Maintaining a consistent frame rate is crucial for VR comfort. Any inconsistencies can lead to "judder", an uncomfortable mismatch between the virtual and physical camera position.

7. **🌌 Independent Visual Backgrounds (IVB):** Using IVBs can help to reduce discomfort by allowing the user's brain to reinterpret the visual motion as the world moving around them, rather than them moving through the world.

8. **🎮 Simulated Activities:** Controlling artificial locomotion through the re-enactment of physical activities (such as walking in place or climbing a ladder) can improve comfort by aligning proprioceptive and vestibular input with visual motion.

9. **🔊 Spatial Sound Effects:** Sound effects can help in reducing disorientation during blink effects or when occluding the environment. It helps in positioning the users in the environment.

10. **⚙️ Asynchronous Time Warp (ATW):** ATW is a re-projection feature that reduces the effect of judder when the application doesn't submit frames fast enough to keep up with the display refresh rate.

## Keywords
- **Vection:** It is the sensation of movement of the body in space produced purely by visual inputs. In the context of this transcript, it refers to the visual perception of motion that causes discomfort in VR.

- **Optic Flow:** The pattern of apparent motion of objects, surfaces, and edges in a visual scene caused by the relative motion between an observer and a scene. High optic flow can cause discomfort in VR due to the perceived motion.

- **Teleportation (VR):** A common form of locomotion in VR that instantly moves the player from one place to another, thus reducing motion sickness.

- **Judder:** A visual artifacting that occurs in VR when the frame rate is inconsistent. It refers to the uncomfortable mismatch between the virtual and physical camera position.

- **Asynchronous Time Warp (ATW):** A reprojection technique used in VR to maintain a high frame rate and prevent judder. It helps in reducing discomfort by making sure the image on the display keeps up with the user's head movement.

- **Independent Visual Background (IVB):** A technique used in VR to reduce discomfort. It uses consistent imagery or geometry in the environment that aligns with the user's vestibular senses to trick the brain into thinking the user is stationary, and it's the world that's moving.

- **Vestibular Senses:** They are the sensory system that contributes to the sense of balance and spatial orientation for coordination of movement. Discrepancies between vestibular senses and visual inputs in VR can cause discomfort.

- **Proprioceptive Input:** This is the sense of the relative position of one's own parts of the body and the strength of effort being employed in movement. In VR, alignment of proprioceptive and vestibular input with visual motion can help improve comfort.

- **Binocular Disparity:** The difference in image location of an object seen by the left and right eyes, resulting from the eyes’ horizontal separation. The brain uses binocular disparity to extract depth information from the two-dimensional retinal images in stereopsis.

- **Occlusion Depth Cues:** In the context of VR and 3D graphics, occlusion refers to the effect of one object in 3D space blocking another object from view. In terms of depth perception, if an object occludes another, it is perceived as being closer.
