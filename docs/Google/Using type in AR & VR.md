---
layout: default
title: Using type in AR & VR
parent: Google
---

# Using type in AR & VR

Original article: [Using type in AR & VR](https://fonts.google.com/knowledge/using_type_in_ar_and_vr)

## TL;DR

In AR/VR environments, traditional typography rules are insufficient, requiring new approaches to ensure text readability and legibility in 3D spaces. Factors like text rendering methods, dimensionality, and intricate font details like counters and apertures are crucial but can be affected by optical distortions like chromatic aberration. Both hardware and software need to innovate to tackle these unique typographic challenges as AR/VR technology continues to evolve.

## Bullet points

1. 📏 **Spatial Classification of Typography**: Text in AR/VR is not just a flat element but exists in a three-dimensional space. Decisions have to be made on whether text will remain stationary in the 3D environment or will move according to the user's point of view. These decisions have immediate implications on legibility and usability. This also affects how text should behave when the user is in motion.

2. 🔠 **Challenges in Text Rendering**: The 3D medium poses challenges like perspective distortion, distance reading, and distortion of letter shapes. These are not entirely new issues but are intensified and nuanced in a 3D context. For example, readability can be compromised if guidelines from traditional mediums, such as highway signs, are directly translated to AR/VR applications.

3. 🚫 **Limitations of 3D Text**: While 3D text might seem like an attractive option for a 3D medium, it hinders readability and legibility. Three-dimensional text adds to the letter shapes and complicates the spaces between them, making them less recognizable and requiring extra effort to read. Flat, 2D text is generally recommended for sentences and paragraphs.

4. 🔡 **Role of Variable Fonts**: Variable fonts offer dynamic customization across various axes like weight, width, and spacing. This adaptability is crucial for optimizing text based on the user's viewpoint, distance, and background contrast. It allows for real-time adjustments to improve legibility and readability in varying conditions.

5. 🔄 **Dynamic Rendering**: Text rendering in AR/VR is dynamic due to constant changes in the point of view. Traditional methods, like bitmap glyphs or FreeType, can result in blurred text when resized. More advanced methods, like Signed-Distance-Field-based (SDF) text rendering, offer better scalability but can still suffer from rounding issues at corners when text size exceeds the generated texture.

6. 🔜 **The Future of AR/VR Typography**: Despite advances in AR/VR technology, typography in this medium is still in its nascent stages. Processing power limitations have led designers to adopt less CPU-intensive text rendering methods, affecting the quality of text. However, as technology evolves, there's a need for designing typefaces and applications optimized for these unique challenges.

7. 🎯**Counters and Apertures**: The design of counters (fully enclosed spaces) and apertures (partially enclosed spaces) in letters like "c," "e," and "o" is crucial, especially in AR/VR contexts. Factors like irradiation and chromatic aberration can fill these spaces, causing misrecognition. For instance, a "c" may appear as an "o." Opt for typefaces with larger counters and open apertures for better legibility.

8. 🏋️‍♂️**Font Weight Matters**: In environments with varying resolutions, the weight of the font plays a critical role in how legible the text is. Lighter weights can flicker and blend into the background, making them hard to read. However, going too bold can also affect legibility by closing up counters and apertures. Medium to semi-bold weights usually offer a good balance and should be tested rigorously.

9. 🖊️**Width and X-Height**: The width of the typeface and its x-height (the height of lowercase letters like "x") are significant for legibility, especially in AR where text can be viewed from different angles and distances. Wider typefaces generally perform better but may require more space. A large x-height enhances legibility but must be balanced to prevent letter misrecognition.

10. ✒️**Visual Nuances **: Fine details such as stroke contrast, the thinning at joints, and stroke endings can be distorted in AR/VR due to factors like halation (glow around letters). Therefore, opt for low-to-moderate contrast typefaces and those that have well-defined stroke endings. Additionally, generous letter spacing is needed to prevent the merging of letters, particularly when viewed at angles.

11. 📑 **Text Classification in AR/VR**: The document outlines six categories for classifying text in augmented and virtual reality environments. These classifications — "Text in HUD," "Text for Long Reading," "Sticky Info Text," "Signage Text," "Responsive Text," and "Ticker Text" — serve different purposes and require specific considerations for rendering. This classification framework aids in the decision-making process for designing and setting text within AR/VR applications.

12. 👁️ **Field of View (FoV) Constraints**: The document highlights the importance of Field of View (FoV) as a critical factor in AR/VR text placement and readability. Human FoV is around 120° when looking straight and extends up to 200°-270° with eye movement. In contrast, most AR/VR devices offer a much more limited FoV, typically between 40° and 100°. This discrepancy imposes a constraint on the amount of text that can be comfortably displayed and emphasizes the need for wider FoV in future AR/VR devices for a more immersive experience.

13. ☀️ **Brightness and Contrast Challenges**: Addressing the brightness and contrast levels in AR/VR environments, especially for optical see-through headsets (OSTs), is essential. The document emphasizes that achieving a high level of brightness is vital for legible text in high ambient light conditions, such as outdoors. It also indicates that contrast ratios affect how easily the text can be read, making it a key factor in designing textual elements in mixed realities.

14. 🖥️ **Resolution and Pixel Density**: The document details the role of resolution and pixels per degree (PPD) in AR/VR text readability. A higher PPD will yield clearer and sharper text. However, the resolution isn't just about the number of pixels; it also depends on how these pixels are magnified by the optics of the device. Therefore, the calculation for PPD takes into account both the number of pixels and the device's field of view. With current technology, achieving a PPD close to the human eye's capability (approximately 60 PPD) remains a challenge.

15. 🎨 **Optical and Graphical Distortions**: Various kinds of optical and graphical distortions, such as halation, chromatic aberration, and the screen door effect, can negatively impact text readability and overall user experience in AR/VR. Halation causes a foggy glow around text, compromising its clarity. Chromatic aberration can produce colored fringes around text and objects, disrupting the immersive experience and possibly causing user discomfort. The screen door effect arises from the visible grid lines between pixels, reducing the perceived quality of the display. Addressing these distortions is crucial for improving the visual quality and readability of text in AR/VR environments.

## Keywords

- **Typography**: The art and technique of arranging type, critical for readability and legibility in AR/VR environments.

- **Legibility**: The clarity of text, influenced by factors such as dimensionality and rendering methods in AR/VR.

- **Readability**: The overall ease with which text can be read, impacted by layout and design.

- **Dimensionality**: Refers to whether text appears flat (2D) or has depth (3D) in AR/VR environments.

- **Spatial Classification**: Organization and behavior of text in 3D space, relevant for typography in AR/VR.

- **Variable Fonts**: Customizable fonts that offer control over multiple design axes like weight, width, and spacing.

- **Extrapolation**: The estimation of text appearance at sizes other than the original, which can cause issues like rounding errors.

- **Atlas (Text Atlas)**: Pre-generated text glyphs used for rendering, optimized for specific conditions in AR/VR.

- **Texture Maps**: Pre-rendered images that add details or depth to 3D models, including text.

- **SDF (Signed-Distance-Field)**: A text rendering method that offers smoothness by measuring the pixel distance from shape boundaries.

- **OTF/TTF (OpenType Font/TrueType Font)**: Font file types that are potentially not used directly in AR/VR due to performance concerns.

- **Counters**: The enclosed or partially enclosed circular or curved negative spaces in characters like "c," "d," and "o." Important for text legibility in AR/VR.

- **Apertures**: The partially enclosed, somewhat rounded negative spaces in some characters such as "n," "C," "S," etc. Important for text legibility.

- **Chromatic Aberration**: A distortion where colors are rendered incorrectly, which can lead to counters and apertures appearing closed, affecting legibility.

- **Irradiation**: A phenomenon where light or color spills over the boundaries of an object, affecting its perceived shape. In fonts, this can make small counters and apertures appear filled.

- **Font Weight**: Refers to the thickness of the character outlines in a font, affecting legibility.

- **Stroke Contrast**: The variation in stroke thickness within a single character, which may be a problem in low-resolution devices like AR/VR headsets.

- **X-Height**: The height of lowercase letters, disregarding ascenders or descenders. Important for determining the legibility of a typeface.

- **Ascenders and Descenders**: Ascenders extend above the x-height, while descenders extend below the baseline. Important for letter recognition.

- **Joints/Intersections**: The points where strokes in a character meet; the glow of pixels (halation) at these points can affect legibility.

- **Halation**: The scattering of light beyond its proper boundaries, often causing a foggy appearance or glow around text, impacting legibility.

- **Terminals**: The end of a stroke in a letter or symbol, which can be distorted in AR/VR environments, affecting legibility.

- **Letter Spacing**: The amount of space between characters in a word or sentence; generous spacing is often needed in AR/VR to maintain legibility.
