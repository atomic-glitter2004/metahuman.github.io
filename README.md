# Picture to metahuman workflow

1. **Picture to head 3D model using face builder(blender plugin)**
    1. Blender + plugin(face builder)
    2. Require at least two pictures, front, and side views for the model, and at least 3 pictures (Front + two sides) for texture jpg if want specific character skin textures such as mole, acne,     brows(since metahuman default brows are limited so drawn on/original brow would be helpful), etc.
    3. Export JPG + FBX file from blender
2. **Head model to metahuman**
    1. Import FBX(as mesh) + JPG(as texture)
    2. Use the metahuman plug-in to create a metahuman identity
    3. Calibrate neutral expression + add body
    4. Export to quixel bridge
3. **Meta human creation**
    1. Use metahuman creator to create a facial feature
    2. Add body and cloth
4. **Meta human use in-game/level/etc.**
    1. Download to game/file using Quixel bridge
    2. Use previously processed jpg to create facial pattern textures by dragging the texture into the material editor and connecting the texture to the base color node
5. **Use the plugin Metahuman SDK to speak(voice-to-facial movement or text to speech then movent) or as needed**
