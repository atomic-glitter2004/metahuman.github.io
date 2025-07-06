# Picture to metahuman workflow
Internship project
1. **Picture to head 3D model using face builder(blender plugin)**
    1. Blender + plugin(face builder) **update 1.0**:: Could use Hunyuan 2.0 made by Tencent for a more personalized model, however not yet known how it could be used for later on mesh to metahuman **update 2.0**: Metahumansdk company offers WEBGL 3D avatars which is optimized for web and generate avatar from a selfie in one click. Could potentially be helpful in terms of mesh to metahuman, or even bypass the process of metahuman as it could still use SDK and thus doesn't need to go through UE5(decrease requirement for use device capacity or cloud capacity)
    2. Require at least two pictures, front, and side views for the model, and at least 3 pictures (Front + two sides) for texture jpg if you want specific character skin textures such as mole, acne,     brows(since metahuman default brows are limited so drawn on/original brow would be helpful), etc. **update 1.0**: Hunyuan could use simply a front image since created metahuman only is for a single-angled use. However if 3D is needed then 3 image(front + 2 side)
    3. Export JPG + FBX file from blender**update 3.0**:JPG need to be processed by removing hair color, and bolding eyebrows if not ovious.
2. **Head model to metahuman**
    1. Import FBX(as mesh) + JPG(as texture)
    2. Use the metahuman plug-in to create a metahuman identity **update 1.0**:potentially needs to calibrate the model if using Hunyuan
    3. Calibrate neutral expression + add body
    4. Export to Quixel bridge
3. **Meta human creation**
    1. Use metahuman creator to create a facial feature
    2. Add body and cloth
4. **Meta human use in-game/level/etc.**
    1. Download the game/file using Quixel bridge
    2. Use previously processed jpg to create facial pattern textures by dragging the texture into the material editor and connecting the texture to the base color node
5. **Use the plugin Metahuman SDK to speak(voice-to-facial movement or text to speech then movent) or as needed**
6. **update4.0**UE5 also could be ran to do deeplearning which could be applied futher when AI movement could be implimented. Moreover, it is possible to use q-learning to train movement directly in UE however not with metahuman(?)
