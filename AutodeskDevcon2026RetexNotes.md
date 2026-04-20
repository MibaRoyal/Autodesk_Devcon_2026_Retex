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

## Session 3: Integrated language model system for checking technical room compliance in project "Grand Paris Express", by EGIS engineering company (FR).
This French engineering team was tasked with designing the technical rooms for the massive Grand Paris Express metro line.
The automation team created a system which could answer user questions on the design of thechnical rooms, specifically about norm compliance or clashes.
The system read and analyzed hundreds of Revit models and hundreds of norm specifications.
1) The human-written French norms are available as tables with admixed text, images, formatting and so on. These were converted to JSON tables of parameters with a language model.
2) The collection of JSON parameters, and the many Revit models, were hosted on the Autodesk Platform Service cloud, which allowed parallel processing of several requests and storing the system code, offering it to the user by session.
3) Depending on the user request, the system could generate isometric or section details, to document compliance to a certain norm parameter, and generate a text report presenting the result.
4) The handling and closure of issue requests was proposed by the language model and final check was done by a human.

_Remark: This presentation showed an actual project, and the complexity of integrating different data sources in different formats. A similar system would benefit a project like Pallas._




