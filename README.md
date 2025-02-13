# Picture to metahuman workflow

1. **Picture to head 3D model using face builder(blender plugin)**
    1. Blender + plugin(face builder) *update 1.0:: Could possibly use Hunyuan 2.0 made by Tencent for a more personalized model, however not yet known how it could be used for later on mesh to metahuman
    2. Require at least two pictures, front, and side views for the model, and at least 3 pictures (Front + two sides) for texture jpg if you want specific character skin textures such as mole, acne,     brows(since metahuman default brows are limited so drawn on/original brow would be helpful), etc. *update 1.0: Hunyuan could use simply a front image since created metahuman only is for a single-angled use. However if 3D is needed then 3 image(front + 2 side)
    3. Export JPG + FBX file from blender
2. **Head model to metahuman**
    1. Import FBX(as mesh) + JPG(as texture)
    2. Use the metahuman plug-in to create a metahuman identity *update 1.0:potentially needs to calibrate model if use Hunyuan
    3. Calibrate neutral expression + add body
    4. Export to Quixel bridge
3. **Meta human creation**
    1. Use metahuman creator to create a facial feature
    2. Add body and cloth
4. **Meta human use in-game/level/etc.**
    1. Download the game/file using Quixel bridge
    2. Use previously processed jpg to create facial pattern textures by dragging the texture into the material editor and connecting the texture to the base color node
5. **Use the plugin Metahuman SDK to speak(voice-to-facial movement or text to speech then movent) or as needed**
