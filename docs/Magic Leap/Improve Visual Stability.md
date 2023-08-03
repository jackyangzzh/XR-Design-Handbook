
# Improve Visual Stability
Original article: [Improve Visual Stability](https://developer-docs.magicleap.cloud/docs/guides/best-practices/improve-visual-stability)

## TL;DR
In augmented and mixed reality, Visual Stability anchors virtual objects in the real world. Optimal realism relies on adjusting Focus Distance and Near/Far Clipping Planes based on user interactions and scene content. However, developer oversights, especially in Unity applications, can disrupt this stability.

## Bullet points

1. **🔍 Visual Stability**: This sensation ensures that virtual objects feel grounded and consistent in the real world, especially as you move your device around. High visual stability means that virtual objects remain steadfast and anchored, enhancing the augmented or mixed reality experience's realism.

2. **📏 Focus Distance**: This is a pivotal measurement indicating the distance between the headset and a chosen virtual plane. When this distance closely matches the primary object the user is looking at, the object appears more stable and realistic. In settings with multiple objects, aligning this distance with the furthest object is usually best unless user interactions indicate otherwise.

3. **🔲 Near/Far Clipping Planes**: Invisible boundaries determining the range at which virtual content appears. Keeping these boundaries tight and adaptive to the content in view ensures clarity and grounded visuals. Dynamic adjustments, based on scene content, offer the user a clear and undistracted view of the virtual elements.

4. **🖼️ World Lock Experience (Pixel Stick Quality)**: A critical aspect of AR and MR applications, this factor dictates how embedded and fixed virtual content feels in the real world. Its effectiveness is closely linked to the correct setting of the focus distance and clipping planes, emphasizing the developer's role in adjusting these parameters accurately.

5. **⚠️ Common Pitfalls**: Some typical mistakes developers make include neglecting to set a focus distance, particularly in Unity-driven applications; defaulting to a large, static focus distance value, which disrupts the stability of near objects; and routinely setting the focus on the closest object in a scene with multiple items, causing distant objects to feel unstable.

6. **🛠️ Dynamic Adjustments**: Rather than sticking to static values, developers are advised to dynamically alter the near/far clipping planes and focus distance based on the scene's content. This approach ensures optimal visual stability as the environment or user's focus changes, leading to a more immersive experience.

7. **👁️ User Interactions as Cues**: When multiple virtual objects are present, user cues such as eye-tracking, controller interactions, or hand gestures can provide invaluable insights. Developers can leverage this information to adjust the focus distance, prioritizing objects that the user is most likely to interact with or focus on.

## Keywords
- **Visual Stability**: The degree to which virtual content remains fixed in position and orientation relative to the real world, especially as the user moves or shifts their gaze.

- **Focus Distance**: A parameter that determines the ideal virtual distance for rendering content to ensure that it appears stable and anchored to the real world.

- **MLGraphicsFrameParamsEx**: Structure that defines the frame parameters for rendering the next frame in ML2.

- **World Lock Experience/Pixel Stick Quality**: The extent to which virtual content feels integrated and stable in the real world when viewed through mixed-reality devices.

- **Near/Far Clipping Planes**: Virtual boundaries that determine the closest and farthest points at which content will be rendered in a mixed-reality scene.