# Autodesk Devcon 2026, event report
The following text presents my experience at the Autodesk Devcon 2026 event.
The Event was organized by Autodesk with participation by a number of collaborating companies.
The event took place on Wednesday 15 and Thursday April 16, 2026, at the Beurs van Berlage in Amsterdam.

## Session 1: Automatic pattern generation for tiling the roof of the Sydney opera house
Two programmers from 4G architect presented their workflow for automatic design of a tiling pattern.
The Revit model is imported into Rhino to generate a parametric mesh. An algorithm called "kangaroo solver" iterated through solutions to find a suitable arrangement of shingles.
The generated arrangement pattern was exported from Rhino back into Revit. A similar approach was employed to generate a pattern and arrays of panels following a radial arrangement.
The workflow was operated from within Revit with a dedicated tool. Operation of the tool was shown with a screen capture video.
_Remark: This presentation did not document the application of language models; it presented the integration of Revit, Rhino and an algorithmic solver._

## Session 2: Integration of data collections for job site management
The Californian company "Open Space" proposes a concept platform for integrating different data collections.
The idea is to integrate point cloud recorded with Ray-Ban sunglasses, sensor position data, as well as language model analysis of layout drawings, 360 site photos, norms and requirements.
The hypothetical integrated system would then enable a user to track job process, identify code violations and safety issues, delays in execution, process invoices and payments, and so forth.
No actual projects were presented, only possibilities, a few non-live examples, and many stock-footage like 3D animations.
_Remark: This speaker used the word "imagine" many times; the presentation focuses on technical possibilities rather than demonstrated real-world performance. Whether the proposed system can be built efficiently for practical deployment remains unproven._

## Session 3: Combined language model + cloud system for checking technical room compliance in project "Grand Paris Express"
French engineering/developer team at EGIS was tasked with designing a system for evaluating a large number of technical room designs for the massive Grand Paris Express metro line.
The automation team created a system that could answer user questions on the design of technical rooms, specifically about norm compliance or clashes.
The system read and analyzed hundreds of Revit models and hundreds of norm specifications.
1) The human-written French norms are available as tables with admixed text, images, formatting and so on. These were converted to JSON tables of parameters with a language model.
2) The collection of JSON parameters and the many Revit models were hosted on the Autodesk Platform Service cloud, which allowed parallel processing of several requests and storing the system code, offering session-based access to users.
3) Depending on the user request, the system could generate isometric or section details, to document compliance to a certain norm parameter, and generate a text report presenting the result.
4) The handling and closure of issue requests was proposed by the language model and final check was done by a human.

_Remark: This presentation showed an actual real-world solution. A similar system would benefit a similarly large project with repetitive tasks, such as Pallas._

## Session 4: platform "Viktor" for handling Revit models and other applications.
The Viktor platform allows users to instruct a language model to perform different operations on Revit models.
It can also design workflows including exporting building information to other applications, like a finite element analysis for structural calculations.
The Viktor.ai system can generate simple Python scripts to extract and process information from a Revit model. It is unclear how linked models behave.
The language model is running on a Claude engine. A free demo is available but is very limited.
The presentation demo was heavily "sandboxed" and used a very simple model without links.
Practical use of the platform during a personal enquiry of this writer immediately showed a few bugs and the typical shortcomings of language model behaviour: misunderstanding the prompt and beating around the bush.
The Viktor stand showed a video of application to the design of a Hello Fresh warehouse; unfortunately I couldn't check the quality of this evidence.
_Remark: This company demonstrated a technically interesting approach but offered limited evidence of practical deployment. Field testing on real projects remains incomplete._

## Hand-out leaflet: Fortune article "AI at the frontier: Capability, adoption, and the Road Ahead" by Jeremy Kahn.
A two-page flyer was handed out, containing Kahn's article. The article states that AI is advancing fast and already delivers strong results in some real-world tasks, especially in coding. But its capabilities remain uneven, with clear overall weaknesses; actual use in engineering remains lower than 20%. Success will depend less on the model quality and more on governance, oversight, and well-designed human-AI workflows.
_Remark: It is unclear how the article measures "theoretical AI coverage" and "strong results". Key claims lack clear substantiation or supporting data._

## Hand-out leaflet documenting the "Open Building Service Reference" by bosch and Autodesk
A leaflet was handed out, pointing to Bosch’s article about their Open Building Service Reference. The article says it wants to turn messy building data into usable digital building models for maintenance and operations. That basic idea is plausible.
_Remark: The rest of the article contains lots of catchy jargon, but key claims lack substantiating evidence. The value propositions are not demonstrated or quantified._

# Concluding remarks
Only one of the four presentations I attended were actual solutions to problems using language models; one was an algorithmic solver, the other two were proofs of concept and early-stage concepts.
Moreover:
1) There is a real need for converting information encoded for humans, such as texts and images in norms and standards, into information searchable by machines. This was discussed by EGIS, Bosch, and Open Space; only EGIS presented a field-proven successful solution.
2) Reading and understanding Revit files was demonstrated by EGIS and Viktor; this appears technically feasible. Processing and modifying Revit information may be possible with Viktor, pending further refinement. Practical time-saving benefits remain unquantified.
3) There is a real need for reading and understanding layout drawings (accurately describing them in text); Open Space says their system "may" do that, but this capability appears technically promising yet remains unvalidated in practice.
4) The presented "platforms" or "systems" – Viktor and Open Space – are at early stages of development, demonstrating technical feasibility rather than production-ready solutions. This reflects the general maturity level of much of the current language model tooling.

None of the presentations actually gave quantitative data about saving time using language models. In general terms, developing these systems into working automation is costly and time-consuming, and is only justified by economies of scale on very large projects. This is true of most automation projects.
The event was clearly commercial in nature, with many logos, free high-quality lunch, and dramatic slogans. Presentations showcased systems at various stages of maturity, from early-stage technical demonstrations to near-production solutions. Fully mature, field-proven engineering solutions were not prominently featured.




