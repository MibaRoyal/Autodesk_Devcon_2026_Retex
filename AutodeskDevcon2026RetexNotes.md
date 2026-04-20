# Autodesk Devcon 2026, event report
The following text presents my experience at the Autodesk Devcon 2026 event.
The Event was organized by Autodesk with participation by a number of collaborating companies.
The event took place on Wednesday 15 and Thursday april 16, 2026, at the Beurs van Berlage in Amsterdam.

## Session 1: Automatic pattern generation for tiling the roof of the Sydney opera house
Two programmers from 4G architect presented their workflow for automatic design of a tiling pattern.
The Revit model is imported in Rhino to generate a parametric mesh. An algorithm called "kangaroo solver" iterated through solutions to find a suitable arrangement of shingles.
The generated arrangement pattern was exported from Rhino back into Revit. A similar approach was employed to generate a pattern and arrays of panels following a radial arrangement.
The workflow was operatied from within Revit with a dedicated tool. Operation of the tool was shown with a screen capture video.
_Remark: This presentation did not document the application of language models; it presented the integration of Revit, Rhino and an algorithmic solver._

## Session 2: Integration of data collections for job site management
The Californian company "Open Space" proposes an imaginary platform for integrating different data collections.
The idea is to integrate point cloud recorded with rayban sunglasses, sensor position data, as well as language model analysis of layout drawings, 360 site photos, norms and requirements.
The hypothetical integrated system would then enable a user to track job process, identify code violations and safety issues, delays in execution, process invoices and payments, and so forth.
No actual projects were presented, only possibilities, a few non-live examples, and many stock-footage like 3D animations.
_Remark: This speaker used the word "imagine" many times; the presentation was heavily speculative and hype-oriented; whether a stable, fast, efficient system, that runs reliably on low-grade hardware, can at all be created, remains to be seen._

## Session 3: Combined language model + cloud system for checking technical room compliance in project "Grand Paris Express"
French engineering / developers team at EGIS was tasked with designing a system for evaluating a large number of technical rooms designs, for the massive Grand Paris Express metro line.
The automation team created a system which could answer user questions on the design of thechnical rooms, specifically about norm compliance or clashes.
The system read and analyzed hundreds of Revit models and hundreds of norm specifications.
1) The human-written French norms are available as tables with admixed text, images, formatting and so on. These were converted to JSON tables of parameters with a language model.
2) The collection of JSON parameters, and the many Revit models, were hosted on the Autodesk Platform Service cloud, which allowed parallel processing of several requests and storing the system code, offering it to the user by session.
3) Depending on the user request, the system could generate isometric or section details, to document compliance to a certain norm parameter, and generate a text report presenting the result.
4) The handling and closure of issue requests was proposed by the language model and final check was done by a human.

_Remark: This presentation showed an actual real-world solution. A similar , within a huge project with repetitive tasks. A similar system would benefit a similarly large project like Pallas._

## Session 4: platform "Viktor" for handling Revit models and other applications.
The Viktor platform allows users to instruct a language model to perform different operations on Revit models.
It can also design workflows including exporting building information to other applications, like a finite element analysis for structural calculations.
The Viktor.ai system can generate simple Python scripts to extract and process information from a Revit model. It is unclear how linked models behave.
The language model is running a Claude engine. A free demo is available but is very limited.
The presentation emo was heavily "sandboxed" and used a very simple model without links.
Practical use of the platform during a personal enquiry of this writer immediately showed a few bugs and the typical shortcomings of language model behaviour: misunderstanding the prompt and beating around the bush.
The Viktor stand showed a video of application to the design of a Hello Fresh warehouse; unfortunately I couldn't check the quality of this evidence.
_Remark: This company also showed clear signs of "wishful thinking", glossing over the difficulties of real-life application to real projects, and had no real projects to document._

## Hand-out leaflet: Fortune article "AI at the frontier: Capability, adoption, and the Road Ahead" by Jeremy Kahn.
A two-page flyer was handed out, containing Kahn's article. The article states that AI is advancing fast and already delivers strong results in some real-world tasks, especially in coding. But its capabilities remain uneven, with clear overall weaknesses; actual use in engineering reamins lower than 20%. Success will depend less on the model quality and more on governance, oversight, and well-designed human-AI workflows.
_Remark: It is unclear how the article measures "theoretical AI coverage" and "strong results". Therefore, the text comes over like wishful thinking and hype-driving._

## Hand-out leaflet documenting the "Open Building Service Reference" by bosch and Autodesk
A leaflet was handed out, pointing to Bosch’s article about their Open Building Service Reference. The article says it wants to turn messy building data into usable digital building models for maintenance and operations. That basic idea is plausible.
_Remark: The rest of the article feels inflated, lots of catchy jargon with little proof. It reads more like a strategy pitch and hype-milking than a serious engineering solution._

# Concluding remarks
Only one of the four presentation I attended were actual solutions to problems using language models; one was an algorithmic solver, the other two were proofs of concept and hypotheses.
Moreover:
1) There is a real need for converting information encoded for humans, such as texts and images in norms and standards, into information searchable by machines. This was discussed by EGIS, Bosch, Open Space; only EGIS presented a field-proven succesful solution.
2) Reading and understanding Revit files was demonstrated by EGIS and Viktor; it seems feasible. Processing and modifying Revit information might be possible with Viktor, after getting used to the buggy workflow. No clear time-saving was demonstrated nor quantified.
3) There is a real need for reading and understanding layout drawings (as in accurately describing in text); OpenSpace says their system "may" do that, but this is little more than fantasizing;
4) The presented "platforms" or "systems"  Viktor and OpenSpace were little more than sandboxes or proofs-of-concept, without field-proven applications to present. This is true of much of the narration and press surrounding language model development.

None of the presentation actually gave quantitative data about saving time using language models; in general terms, developing these systems to actually working automation is costly and time-consuming, and only justified by economies of scale on very large projects. This is true of most automation projects.
The event was clearly commercial in nature, with many logos, free high-quality lunch, dramatic slogans, presentations of barely working hypothetical and experimental systems. Actual engineering solutions, typically more plain and drab, were not prominently visible.




