# Fetal Health Monitoring

Fetal Health Monitoring is imperative to prevent complications during childbirth and ensure a timely medical intervention. Deep learning has revolutionised numerous fields, including medical imaging. This report presents a deep learning model designed to identify fetal intracranial structures during the 11th to 14th weeks of pregnancy using ultrasound imaging, and provide an automated process of standard and non-standard sagittal view classification.

The ability to accurately identify and classify these structures is crucial in obstetric ultrasound examinations. It allows for early detection of potential abnormalities, enabling timely intervention and management. However, manual identification and classification can be time-consuming and dependent on the sonographer's expertise.

By harnessing the power of deep learning, we hope to improve the accuracy and speed of these critical assessments, ultimately contributing to better prenatal care and outcomes.

Our solution consists of 2 models. The first model is called **StructureClassification** that does object localization of the 9 structures in the image. 
The second model is called **SNSClassification** that classifies the image as standard or nonstandard.

# Model 1: StructureClassification (Navigate to [branch](https://github.com/claudyAi/adl/tree/Structure-CLassification)
This model is trained on the dataset of Standard images. The input is standard images, structure name and bounding box coordinates of the structure from ObjectDetection.xlsx.
It trains to recognise the location and identify the 9 structures. 9 class classification Output the image with a bounding box drawn on the identified structure.

# Model 2: SNSClassification branch (Current Branch)
This model is trained on the dataset of Standard and Non-Standard images. The input is a mix of Standard and Non-Standard images with corresponding label. It trains to conduct 2 class classification to identify the image as standard or non-standard. Output is the image with label standard or non-standard.

# Preparing the dataset for training
Please ensure that you download the zip file folders from the [google drive](https://drive.google.com/file/d/1-ppPA9UHw9ZTBxyGmbWEyCgRNKTECC_6/view?usp=drive_link) and add it to the root folder of this directory before running the below code cell.