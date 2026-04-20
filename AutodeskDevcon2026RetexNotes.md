# Autodesk Devcon 2026, retex notes
## Session 1: Automatic pattern generation for tiling the spherical roof of the Sydney opera house, by "4G Architecture".
Interestingly, the first slide showd an AI-generated "spacecraft"-like impossible façade, with a wrongly fitting window. The audience took pictures of it; apparently the public still buys this slop.
The Revit model is imported in Rhino to generate a parametric mesh.
To generate the mesh, dimensions and parameters of the shingles were also recorded.
An algorithm called "kangaroo solver" iterated through solutions to find a suitable arrangement of shingles.
The generated arrangement pattern was exported from Rhino back into Revit.
A similar approach was employed to generate a pattern and arrays of panels following a radial arrangement.
The second approach, which was seemingly selected for production, entailed the algorithmic generation of packaging lists for packing the irregular shaped panels.
_Remark: This presentation did not document the application of language models; it presented the integration of Revit, Rhino and an algorithmic solver._

## Session 2: Integration of data collections for job site management, by "Open Space".
This Californian company proposes a concept platform for integrating different data collections.
The idea is to integrate the following data collections:
1) point cloud, captured with lidar glasses
2) position encoding of the walkthrough route with sensor data, for example bluetooth
3) language model analysis of layout drawings,
4) language model analysis of site photos, normal and 360deg
5) language model absorption of norms, documentation, requirements.

The hypothetical integrated system would then enable a user to track job process, identify code violations and safety issues, delays in execution, process invoices and payments, and so forth.
No actual projects were presented, only hypothetical possibilities and a few sandbox examples.
_Remark: This speaker used the word "imagine" many times; the presentation was heavily speculative and hype-oriented; whether a stable, fast, efficient system, that runs reliably on low-grade hardware, can at all be created, remains to be seen._

