# Autodesk Devcon 2026, retex notes
The following text presents my experience at the Autodesk Devcon 2026 event.
The Event was organized by Autodesk with participation by a number of collaborating companies.
The event took place on wednesday 15 and thursday april 16, 2026, at the Beurs van Berlage in Amsterdam.

## Session 1: Automatic pattern generation for tiling the spherical roof of the Sydney opera house, by "4G Architecture".
The Revit model is imported in Rhino to generate a parametric mesh.
To generate the mesh, dimensions and parameters of the shingles were also recorded.
An algorithm called "kangaroo solver" iterated through solutions to find a suitable arrangement of shingles.
The generated arrangement pattern was exported from Rhino back into Revit.
A similar approach was employed to generate a pattern and arrays of panels following a radial arrangement.
The workflow was operatied from within Revit with a dedicated tool. Operation of the tool was shown with a screen capture video.
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
No actual projects were presented, only hypothetical possibilities and very polished, stock-footage like 3D animations.
_Remark: This speaker used the word "imagine" many times; the presentation was heavily speculative and hype-oriented; whether a stable, fast, efficient system, that runs reliably on low-grade hardware, can at all be created, remains to be seen._

## Session 3: Integrated language model system for checking technical room compliance in project "Grand Paris Express", by EGIS engineering company (FR).
This French engineering team was tasked with designing the technical rooms for the massive Grand Paris Express metro line.
The automation team created a system which could answer user questions on the design of thechnical rooms, specifically about norm compliance or clashes.
The system read and analyzed hundreds of Revit models and hundreds of norm specifications.
1) The human-written French norms are available as tables with admixed text, images, formatting and so on. These were converted to JSON tables of parameters with a language model.
2) The collection of JSON parameters, and the many Revit models, were hosted on the Autodesk Platform Service cloud, which allowed parallel processing of several requests and storing the system code, offering it to the user by session.
3) Depending on the user request, the system could generate isometric or section details, to document compliance to a certain norm parameter, and generate a text report presenting the result.
4) The handling and closure of issue requests was proposed by the language model and final check was done by a human.

_Remark: This presentation showed an actual real-world solution. A similar system would benefit a project like Pallas._

## Lunch was included in the entry ticket; it consisted of mini-portions of warm stews, salads, brownies. Coffee and drinks were free, with servers in uniform. Felt like luxury treatment.

## Session 4: Integrated platform "Viktor" for handling Revit models and other applications.
The Viktor platform allows users to instruct a language model to perform different operations on Revit models.
It can also design workflows including exporting building information to other applications, like a finite element analysis for structural calculations.
The Viktor.ai system can generate simple Python scripts to extract and process information from a Revit model. It is unclear how linked models behave.
The language model is running a Claude engine. A free demo is available but is very limited.
The presentation emo was heavily "sandboxed" and used a very simple model without links.
Practical use of the platform during a personal enquiry of this writer immediately showed a few bugs and the typical shortcomings of language model behaviour: misunderstanding the prompt and beating around the bush.
_Remark: This company also showed clear signs of "wishful thinking", glossing over the difficulties of real-life application to real projects, and had no real projects to document._

## Hand-out leaflet: Fortune article "AI at the frontier: Capability, adoption, and the Road Ahead" by Jeremy Kahn.
A two-page flyer was handed out, containing Kahn's article. The article states that AI is advancing fast and already delivers strong results in some real-world tasks, especially in coding. But its capabilities remain uneven, with clear overall weaknesses; actual use in engineering reamins lower than 20%. Success will depend less on the model quality and more on governance, oversight, and well-designed human-AI workflows.
_Remark: It is unclear how the article measures theoretical AI coverage and "strong results". Again, this feels like wishful thinking and hype-driving._

## Hand-out leaflet documenting the "Open Building Service Reference" by bosch and Autodesk
A leaflet was handed out, pointing to Bosch’s article about their Open Building Service Reference. The article says it wants to turn messy building data into usable digital building models for maintenance and operations. That basic idea is plausible.
_Remark: The rest of the article feels inflated, lots of catchy jargon with little proof. It reads more like a strategy pitch and hype-milking than a serious engineering solution._

# Concluding remarks
Two of the four presentation I attended were actual solutions to problems using AI; the other two were little more than proofs of concept and hypotheses.
Of the presentation I attended:
1) Converting information in human formats, such as norms and standards, into information searchable by machines: this was discussed by EGIS, Bosch, Open Space; only EGIS presented a real-world use of this solution.
2) Reading and understanding Revit files seems possible; processing and modifying the Revit information might be possible with Viktor, to a certain degree, after getting used to the buggy workflow.
3) Reading and understanding layout drawings is a real behoefte; no clearly field-proven solution was presented.
4) The presented "platforms" or "systems"  Viktor and OpenSpace were little more than sandboxes or proofs-of-concept.
The event was clearly commercial in nature, with many logos, free lunch, catchy slogans, presentations of barely working hypothetical and experimental systems.
The first presentation contained slide showing an AI-generated "spacecraft"-like façade, with a wrongly fitting "window". The audience rushed to take photos, betraying ongoing interest in fancy slop. Actual engineering solutions are boring and not eye-catching.




