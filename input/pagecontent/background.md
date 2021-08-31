This chapter describes the scope of this guide, provides background information about the DICOM SR to FHIR Observaton Mapping IG, key concepts,
and describes the use cases supported by this implementation guide.

1. [Problem Statement](#problem) - Description of the problem statement
2. [Scope](#scope) - Scope of the IG
3. [Use cases](#usecases) - Key use cases covered by the IG
4. [DICOM SR Mapping to FHIR Observation](#DICOMSR) - Description of data mapped through this IG
5. [Glossary](#glossary) - Glossary of terms used in this IG
5. [References](#references) - Useful references


### Problem
Problem Statement:

DICOM Structured Report (DICOM SR) is a standard for recording clinical imaging observations made regarding an diagnostic or interventional imaging procedure.  Imaging Observations are made by humans, such as a sonographer making measurements on recently acquired ultrasound image, a Radiologist recording observations on an suspected legion, or by a machine, such as an automated AI Algorithm providing qualitative and quantitative observations.

DICOM SR is widely adopted by Imaging-based devices and IT systems. Non-imaging based Healthcare IT Systems, generally, do not support DICOM SR. Non-imaging healthcare systems support HL7 standards, such as FHIR. HL7 has defined Observations as the standardized methor for recoring clinical obesrvations.  Bridging the two standards for clinical imaging observations is necessary for interoperability between these type of systems.

### scope

Scope:

The standards for recording clinical observations, DICOM SR and HL7 FHIR Observation resource are bridged by this IG by the transformation of the DICOM SR attributes to the HL7 FHIR Observation Resource.    

DICOM SR defines a multitude of templates for capturing Diagnostic imaging Observations.  The input for this IG is limited to the DICOM SR template TID-1500 (Measurement Report).

The transformation described is one direction.  Reconstruction of a complete DICOM SR is not expected to be re-constructed from a set of FHIR resources using this IG.

DICOM SR mapping is limited to the Observation Resource.  The resultant mapping is provided, as a minimum, a composition or bundle of Observations.  Depending on the use case, the observations may be a Diagnostic Report. Usecase-specific requirements to construct a diagnostic report(e.g. Mammography) may require the transformation described by this IG.  However the specification of those use cases is not in scope for this IG.  This IG is limited to the Observation Resource.

### usecases

#### Use case 1: AI Results created by AI-based Software Analysis Platform 


#### Use case 2: Image Measurements created by Sonographer on Ultrasound Device

### DICOMSR

### glossary

### References



