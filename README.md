# Smartcity-flood-simulation
## Overview  
This repository demonstrates a full pipeline for generating realistic fluid simulations based on terrain data, starting from height maps and ending with Blender-based flip-fluid visualizations.

## Features  
- Height Map to 3D Terrain: Import grayscale height maps to Unreal Engine and construct 3D terrain meshes.
- Mesh Refinement: Export the terrain mesh to MeshLab for refinement and cleanup.
- Fluid Simulation: Import the refined mesh into Blender and perform Flip Fluids simulation to visualize water or other fluids interacting with the terrain.
- Video Output: The final results are rendered as a video to showcase the complete process.

## Video  
<video src="output.mp4" controls width="800"></video>

## Examples  
Each stage of the pipeline includes step-by-step instructions and sample assets:

- heightmap_to_ue.md – Convert height map image into 3D terrain in Unreal Engine
- ue_to_meshlab.md – Export terrain mesh from Unreal Engine and refine using MeshLab
- meshlab_to_blender.md – Import refined mesh into Blender and set up Flip Fluids simulation
- blender_render.md – Render the simulation results and export as video

## Known Issue  
Mesh simplification during the MeshLab refinement stage may result in small artifacts in the Flip Fluids simulation. Manual mesh verification is recommended.

## Requirements  
- Unreal Engine (tested with UE 5.1+)
- MeshLab
- Blender with Flip Fluids add-on
- Python 3.8+ (for optional automation scripts)

## Getting Started  
Clone this repository:
```bash
git clone https://github.com/yourusername/terrain-flipfluid-pipeline
cd terrain-flipfluid-pipeline
```
Follow the examples in the examples/ directory for each stage of the pipeline.

Launch Unreal Engine and import the provided height maps to begin constructing terrain.

After generating and refining the mesh, open Blender and run the Flip Fluids simulation.

Render the final result as a video using Blender's rendering pipeline.

References

Unreal Engine Documentation: https://docs.unrealengine.com

MeshLab Documentation: https://www.meshlab.net

Blender Flip Fluids Add-on: https://blendermarket.com/products/flipfluids

Blender Documentation: https://docs.blender.org
