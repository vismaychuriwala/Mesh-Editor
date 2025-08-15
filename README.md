# 3D Mesh Editor

This project is a 3D mesh editor built in C++ and OpenGL. It allows users to load, view, and manipulate 3D models. The editor is built around a **half-edge data structure**, which enables efficient traversal and modification of the mesh geometry. The application also supports loading and binding a skeleton to the mesh for basic animation.

## Demonstration

A video demonstration of the editor's features is available on Vimeo:

**[Watch the Demo on Vimeo](https://vimeo.com/1105288119)**

[![Mesh-Editor Demo](images/cow.png)](https://vimeo.com/1105288119)

*A cow mesh loaded in the editor, showcasing the half-edge structure and interactive editing capabilities.*

## Key Features

*   **Half-Edge Mesh Representation:**
    *   Loads 3D models from `.obj` files and converts them into a half-edge data structure.
    *   This structure allows for efficient implementation of mesh operations like face splitting, edge extrusion, and vertex manipulation.
*   **Interactive Mesh Editing:**
    *   **Component Selection:** Users can select individual vertices, edges, and faces of the mesh.
    *   **Coloring:** Selected components can be colored to visually highlight them.
    *   **Extrusion:** Faces can be extruded to create new geometry.
    *   **Vertex Manipulation:** The position of selected vertices can be modified.
*   **Skeletal Animation (Skinning):**
    *   Loads a skeleton from a `.json` file.
    *   Binds the mesh to the skeleton using skinning weights, allowing the mesh to be deformed by the skeleton's joints.
    *   Users can select joints and rotate them to pose the model.
*   **3D Viewer:**
    *   Renders the 3D mesh using OpenGL.
    *   Provides a camera that can be controlled to view the model from different angles.

## Technologies

*   **C++:** The core language for the entire project.
*   **OpenGL:** Used for all 3D rendering.
*   **GLSL (OpenGL Shading Language):** For writing the vertex and fragment shaders.
*   **Qt Framework:** Used for creating the UI, handling user input, and managing the OpenGL context.
