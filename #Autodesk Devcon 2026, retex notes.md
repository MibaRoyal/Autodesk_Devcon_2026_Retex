#Autodesk Devcon 2026, retex notes

## Session 1: Automatic pattern generation for tiling the spherical roof of the Sydney opera house, by "4G Architecture".

Interestingly, the first slide showd an AI-generated "spacecraft"-like impossible façade, with a wrongly fitting window. The audience took pictures of it; apparently the public still buys this slop.
The Revit model is imported in Rhino to generate a parametric mesh.
To generate the mesh, dimensions and parameters of the shingles were also recorded.
An algorithm called "kangaroo solver" iterated through solutions to find a suitable arrangement of shingles.
The generated arrangement pattern was exported from Rhino back into Revit.
A similar approach was employed to generate a pattern and arrays of panels following a radial arrangement.
The second approach, which was seemingly selected for production, entailed the algorithmic generation of packaging lists for packing the irregular shaped panels.

_Concluding summary: This presentation did not document the application of language models; it presented the integration of Revit, Rhino and an algorithmic solver._
