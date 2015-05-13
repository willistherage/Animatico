# Animatico
A node script that combines the animation data of every ThreeJS FBX converted JSON file in a directory. The script assumes that your folder only has similar JS files that all have animation data (i.e. The exact same model and rig with different animations). It will go through and pull the animation from each file and store it in one array. It then duplicates all the other information (UVS, Vertex, Normals, Materials) from the first file in the directory and then adds all the other animations to it's animation array.

#Parameters
Directory Path - Path to the directory containing files you wish to combine.
New File Name - The name of the new file that will contain your combined animations.

#Usage:
node animatico path/to/directory path/to/newfile.js
