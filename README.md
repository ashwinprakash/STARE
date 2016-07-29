# STARE
STructured Analysis of the Retina

What is STARE?

The STARE (STructured Analysis of the Retina) Project was conceived and initiated in 1975 by Michael Goldbaum, M.D., at the University of California, San Diego. It was funded by the U.S. National Institutes of Health . During its history, over thirty people contributed to the project, with backgrounds ranging from medicine to science to engineering. Images and clinical data were provided by the Shiley Eye Center at the University of California, San Diego, and by the Veterans Administration Medical Center in San Diego.
I had the pleasure of working on the project from 1996-2004. The contents of this web page reflect my contributions. Please contact me if you have any questions or requests concerning our data or code. Please contact Dr. Goldbaum if you have any requests concerning the current state of the project.

A brief overview of the project

An ophthalmologist is a medical doctor that specializes in the structure, function, and diseases of the human eye. During a clinical examination, an opthalmologist notes findings that are visible in the eyes of the subject. The ophthalmologist then uses these findings to reason about the health of the subject. For instance, a patient may exhibit discoloration of the optic nerve, or a narrowing of the blood vessels in the retina. An opthalmologist uses this information to diagnose the patient, as having for instance Coats' disease or a central retinal artery occlusion.
A common procedure during an examination is retinal imaging. An optical camera is used to see through the pupil of the eye to the rear inner surface of the eyeball. A picture is taken showing the optic nerve, fovea, surrounding vessels, and the retinal layer. The opthalmologist can then reference this image while considering any observed findings.

This research concerns a system to automatically diagnose diseases of the human eye. The system takes as input information observable in a retinal image. This information is formulated to mimic the findings that an ophthalmologist would note during a clinical examination. The main output of the system is a diagnosis formulated to mimic the conclusion that an ophthalmologist would reach about the health of the subject.

Our approach breaks the problem into two components. The first component concerns automatically processing a retinal image to denote the important findings. The second component concerns automatically reasoning about the findings to determine a diagnosis. Additional outputs include detailed measurements of the anatomical structures and lesions visible in the retinal image. These measurements are useful for tracking disease severity and the evaluation of treatment progress over time. By collecting a database of measurements for a large number of people, the STARE project could support clinical population studies and intern training.

Data

The full set of ~400 raw images in the STARE database can be obtained here. Small versions of all the images can be viewed 100 at a time: 1-100, 101-200, 201-300, 301-400.
List of diagnosis codes and diagnoses for each image.
Expert annotations of the manifestations (features) visible in each image, tabulated here in text files. A total of 44 possible manifestations were queried to the experts during data collection and then reduced to 39 values during encoding. This mapping provides details.
Blood vessel segmentation work including 40 hand labeled images, our results, and a demo.
Artery/vein labelings of 10 images done by expert 1 and expert 2.
Optic nerve detection work including 80 images with ground truth, and our results.
Papers

A lot has been published on this project by many people; these are my two most relevant papers:
A. Hoover, V. Kouznetsova and M. Goldbaum, "Locating Blood Vessels in Retinal Images by Piece-wise Threhsold Probing of a Matched Filter Response", IEEE Transactions on Medical Imaging , vol. 19 no. 3, pp. 203-210, March 2000.
A. Hoover and M. Goldbaum, "Locating the optic nerve in a retinal image using the fuzzy convergence of the blood vessels", IEEE Transactions on Medical Imaging , vol. 22 no. 8, pp. 951-958, August 2003.
Code

Source code for Microsoft Visual C. The image processing portions are separated from the GUI and are coded in plain C.
