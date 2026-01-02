---
id: woundaissist-telemedicine
slug: woundaissist-telemedicine
entity_type: research
status: published
data_completeness: high
last_researched: 2025-01-27
research_category: academic_institution
researcher: AI Assistant
version: 3.3
name: WoundAIssist Mobile Application
description: A patient-centered mobile application designed to support telemedical wound care with AI assistance, enabling patients to document wounds at home through photographs and questionnaires while physicians monitor progress remotely and conduct video consultations.
mission: To develop a patient-centered mobile application for telemedical wound care that enables patients to document wounds at home through photographs and questionnaires while physicians monitor progress remotely and conduct video consultations. The application integrates on-device AI for wound segmentation, ensuring privacy while enabling continuous monitoring.
entity_data:
  results: Usability study demonstrated excellent usability, good app quality, and favorable perceptions of the AI-driven wound recognition feature. The study validated the user-centered design approach, particularly for elderly patients.
  objectives: Develop patient-centered mobile application for telemedical wound care with AI assistance, enabling patients to document wounds at home while physicians monitor progress remotely
  methodology: Iterative, user-centered design process involving both patients and domain experts, with particular focus on usability for elderly patients. The development followed an agile methodology with multiple iterations based on user feedback.
  publication_date: 2025-06-06
  collaboration_period:
  end: 2025-06
  start: 2024
  status: completed
taxonomy:
  geography: Europe
  ai_technology:
  - Predictive ML/DL
  primary_focus:
  - Diagnostics & Preventive Health
  aging_approach: []
  target_biology:
  - General Aging/Longevity
  development_stage: Research / Preclinical
  organization_type: research
  organization_subtype: academic_institution
  therapeutic_modality: []
organizations:
  -
    name: University Hospital Würzburg
    role: collaborator
    org_type: institution
    website: "https://www.ukw.de"
    status: operational
    role_description: Collaborating institution
    contribution_description: University Hospital Würzburg provided clinical expertise in dermatology and wound care. The Dermatology Department contributed to patient recruitment for usability study and validation of wound care workflows.
  -
    name: University of Würzburg
    role: primary
    org_type: institution
    website: "https://www.uni-wuerzburg.de"
    status: operational
    role_description: Primary research institution
    contribution_description: University of Würzburg was the primary institution where the WoundAIssist mobile application was developed. The Department of Computer Science and Human-Computer Interaction provided research facilities, expertise, and research supervision.
products:
  -
    name: WoundAIssist
    type: platform
    status: Published / Research prototype
    development_stage: Research / Preclinical
  -
    name: WoundAIssist
    type: platform
    status: Published / Research prototype
    development_stage: Research / Preclinical
links:
  -
    url: "https://arxiv.org/abs/1704.04861"
    type: research_publication
    title: "MobileNets: Efficient Convolutional Neural Networks for Mobile Vision Applications"
  -
    url: "https://arxiv.org/abs/2508.17635"
    type: research_publication
    title: "Wound3DAssist: A Practical Framework for 3D Wound Assessment"
  -
    url: "https://arxiv.org/abs/2506.06104"
    type: research_publication
    title: "WoundAIssist: A Patient-Centered Mobile App for AI-Assisted Wound Care With Physicians in the Loop"
  -
    url: "https://www.tensorflow.org/lite"
    type: documentation
    title: "TensorFlow Lite: Machine Learning for Mobile and Edge Devices"
  -
    url: "https://arxiv.org/abs/1807.04355"
    type: research_publication
    title: "Deepwound: Automated Postoperative Wound Assessment"
  -
    url: "https://arxiv.org/abs/2506.03188"
    type: research_publication
    title: Multi-Analyte, Swab-based Automated Wound Monitor with AI
  -
    url: "https://arxiv.org/abs/2009.07133"
    type: research_publication
    title: A Mobile App for Wound Localization using Deep Learning
  -
    url: "https://arxiv.org/abs/1505.04597"
    type: research_publication
    title: "U-Net: Convolutional Networks for Biomedical Image Segmentation"
  -
    url: "https://developer.apple.com/machine-learning/core-ml/"
    type: documentation
    title: "Core ML: Machine Learning Framework for Apple Devices"
---

# WoundAIssist Mobile Application

## Description

A patient-centered mobile application designed to support telemedical wound care with AI assistance, enabling patients to document wounds at home through photographs and questionnaires while physicians monitor progress remotely and conduct video consultations.

## Mission

To develop a patient-centered mobile application for telemedical wound care that enables patients to document wounds at home through photographs and questionnaires while physicians monitor progress remotely and conduct video consultations. The application integrates on-device AI for wound segmentation, ensuring privacy while enabling continuous monitoring.

## Project Information

**Publication Date**: 2025-06-06
**Objectives**: Develop patient-centered mobile application for telemedical wound care with AI assistance, enabling patients to document wounds at home while physicians monitor progress remotely
**Methodology**: Iterative, user-centered design process involving both patients and domain experts, with particular focus on usability for elderly patients. The development followed an agile methodology with multiple iterations based on user feedback.
**Results**: Usability study demonstrated excellent usability, good app quality, and favorable perceptions of the AI-driven wound recognition feature. The study validated the user-centered design approach, particularly for elderly patients.
**Collaboration Period**: [object Object]

## Scientific Background

```yaml
elderly_user_design:
  challenges:
  - Varying levels of technical literacy
  - Visual and motor impairments
  - Cognitive load limitations
  - Trust in technology (especially AI)
  - Privacy concerns
  importance: Elderly patients represent a significant portion of chronic wound patients (diabetic ulcers, pressure sores, venous ulcers). Designing for this demographic requires particular attention to interface simplicity, large text, clear instructions, and minimal cognitive load.
  validation: "WoundAIssist's excellent usability results with elderly patients validate the importance of user-centered design in healthcare applications for this demographic."
  design_principles:
  - User-centered design involving elderly patients in the development process
  - Large, high-contrast text and buttons
  - Simple navigation with minimal steps
  - Clear visual feedback and instructions
  - Error prevention and recovery
  - Minimal reliance on technical knowledge
  - Accessibility features (voice instructions, haptic feedback)
mobile_healthcare_ai:
  trends: Growing trend toward on-device AI in healthcare applications driven by privacy concerns, regulatory requirements, and user demand for offline functionality.
  challenges:
  - Balancing model accuracy with size and speed
  - Device fragmentation (different capabilities across devices)
  - Battery consumption
  - Model update mechanisms without cloud connectivity
  technical_advances:
  - Improved mobile hardware (NPUs, optimized GPUs)
  - Better model compression techniques
  - Federated learning for privacy-preserving model updates
  - Edge computing frameworks (TensorFlow Lite, Core ML, ONNX Runtime)
regulatory_and_privacy:
  data_protection: "On-device processing ensures that sensitive health data (wound images) remain on patient's device, addressing key privacy concerns in telemedicine applications."
  gdpr_compliance: On-device processing significantly simplifies GDPR compliance as patient data never leaves the device. No data transfer to third parties reduces regulatory burden and privacy risks.
  informed_consent: Telemedicine applications require clear informed consent regarding data collection, AI processing, and physician access to information.
  medical_device_regulation: Depending on intended use and claims, mobile health applications may require medical device certification (e.g., CE marking in EU, FDA clearance in US). Research prototypes typically exempt, but commercial deployment requires regulatory review.
ai_in_wound_segmentation:
  application: AI-powered wound segmentation enables automated analysis of wound images, helping track healing progression and identify concerning changes. On-device processing addresses privacy concerns while enabling real-time analysis without network dependency.
  clinical_value: Automated wound segmentation can assist both patients and physicians in tracking healing progress, potentially enabling earlier intervention when complications arise. Quantitative measurements (wound area, perimeter) provide objective metrics for healing assessment.
  evaluation_metrics:
  - "IoU (Intersection over Union): Measures overlap between predicted and ground truth segmentation"
  - "Dice coefficient: Similar to IoU, commonly used in medical segmentation"
  - "Pixel accuracy: Percentage of correctly classified pixels"
  - "Boundary accuracy: Precision of wound boundary detection"
  typical_performance: State-of-the-art wound segmentation models achieve 85-95% IoU on standardized datasets. Mobile-optimized models typically achieve 80-90% IoU with significantly reduced model size and inference time.
  technical_approaches:
  - Encoder-decoder architectures (U-Net, DeepLab) for semantic segmentation
  - Mobile-optimized backbones (MobileNet, EfficientNet) for efficiency
  - Model compression techniques (quantization, pruning, knowledge distillation)
  - Transfer learning from large medical image datasets
  technical_requirements: "Mobile deployment requires lightweight models that can run efficiently on resource-constrained devices while maintaining acceptable accuracy. Typical challenges include: model size constraints (< 20 MB), inference speed (< 1 second), memory limitations, and battery consumption."
telemedicine_in_wound_care:
  context: Telemedicine has emerged as a valuable approach for managing chronic wounds, particularly for elderly patients who may have difficulty accessing healthcare facilities regularly. Remote monitoring enables continuous care while reducing healthcare system burden. The COVID-19 pandemic accelerated adoption of telemedicine solutions across healthcare domains, including wound care.
  challenges:
  - Need for accurate wound documentation at home without clinical training
  - Requirement for physician oversight and consultation
  - Privacy concerns with patient data (especially with cloud-based solutions)
  - Usability for elderly patients with limited technical skills
  - Regulatory compliance (GDPR in EU, HIPAA in US)
  - Variability in image quality (lighting, angles, camera quality)
  - Integration with existing healthcare systems
  current_trends:
  - Shift toward on-device AI processing for privacy
  - Focus on elderly-friendly interfaces
  - Integration of multiple data sources (images, questionnaires, sensors)
  - Real-time monitoring and alerting systems
  historical_development: Telemedicine in wound care has evolved from simple photo sharing via email to sophisticated AI-powered platforms. Early systems relied on cloud-based image analysis, but privacy concerns and connectivity requirements limited adoption, especially for elderly patients.
```

## Lessons Learned

### Achievements

- Successfully developed a patient-centered mobile application for telemedical wound care
- Demonstrated excellent usability with elderly patients
- Integrated on-device AI for wound segmentation, ensuring privacy
- Positive user acceptance of AI-driven wound recognition feature
- User-centered design process involving both patients and domain experts

### Challenges

- Limited information available about technical implementation details
- Clinical efficacy data not publicly available
- Commercial deployment status unclear

### Impact on Field

WoundAIssist demonstrates the potential for AI-assisted telemedicine in wound care, particularly for elderly patients with chronic wounds. The focus on on-device processing addresses privacy concerns while enabling remote monitoring capabilities. The excellent usability results, especially among elderly patients, validate the user-centered design approach and suggest that AI-assisted telemedicine can be effectively deployed for this demographic. The positive perception of AI-driven wound recognition indicates user acceptance of AI assistance in healthcare, which is crucial for adoption. For longevity research, this approach could enable better monitoring of age-related conditions requiring regular assessment, such as diabetic ulcers, pressure sores, and other chronic wounds common in elderly populations. The on-device AI processing model could be adapted for other age-related monitoring applications where privacy and accessibility are critical concerns.

## Organizations

### University Hospital Würzburg
**Role in Project**: collaborator
**Role Description**: Collaborating institution
**Contribution**: University Hospital Würzburg provided clinical expertise in dermatology and wound care. The Dermatology Department contributed to patient recruitment for usability study and validation of wound care workflows.
**Organization Type**: institution
**Status**: operational
**Website**: https://www.ukw.de
**Description**: University Hospital Würzburg is a teaching hospital affiliated with the University of Würzburg. The hospital's Dermatology Department provided clinical expertise and validation for the WoundAIssist project.
**Focus**: Clinical care, medical research, and education in dermatology and wound care

### University of Würzburg
**Role in Project**: primary
**Role Description**: Primary research institution
**Contribution**: University of Würzburg was the primary institution where the WoundAIssist mobile application was developed. The Department of Computer Science and Human-Computer Interaction provided research facilities, expertise, and research supervision.
**Organization Type**: institution
**Status**: operational
**Website**: https://www.uni-wuerzburg.de
**Description**: University of Würzburg is a public research university located in Würzburg, Bavaria, Germany. The university's Department of Computer Science and Human-Computer Interaction was the primary institution for the WoundAIssist research project.
**Focus**: Research and education in computer science, human-computer interaction, and medical applications

## Locations

### University of Würzburg Main Campus
**Type**: institution
**City**: Würzburg
**State/Region**: Bavaria
**Country**: Germany
**Organizations**: University of Würzburg

### University Hospital Würzburg
**Type**: facility
**City**: Würzburg
**State/Region**: Bavaria
**Country**: Germany
**Organizations**: University Hospital Würzburg

## Products

### WoundAIssist
**Type**: platform
**Status**: Published / Research prototype
**Development Stage**: Research / Preclinical
**Role in Project**: primary
**Relationship Description**: WoundAIssist mobile application - the main product of this research project
**Description**: A patient-centered mobile application that integrates a lightweight deep learning model for on-device wound segmentation, enabling patients to document wounds at home through photographs and questionnaires while physicians monitor progress remotely and conduct video consultations.
**Capabilities**:
- Wound segmentation from photographs
- Healing progression tracking
- Automated wound assessment
- Real-time processing on mobile devices
- Photograph wound documentation
- Patient questionnaires
- Remote physician monitoring
- Video consultations with physicians
- On-device AI wound segmentation
- User interface optimized for elderly patients
- Continuous wound healing monitoring
**Applications**:
- Telemedical wound care for patients with chronic wounds
- Remote monitoring for elderly patients
- Wound healing assessment and tracking
**Technical Details**:
```yaml
dataset:
  size: Not fully specified in publication, but includes wound images from patients with clinical annotations
  sources:
  - Wound images from patients with chronic wounds
  - Clinical annotations by dermatologists
  annotation: Clinical annotations by dermatologists providing ground truth for wound segmentation
  data_characteristics:
  - Diverse wound types and stages
  - Various lighting conditions
  - Different camera angles and distances
training:
  note: Specific training parameters not disclosed in publication, focus was on usability study rather than technical training details
  metrics: Segmentation accuracy (IoU, Dice coefficient), inference speed, model size, memory footprint
  approach: Supervised learning on annotated wound images
  hardware: Training likely performed on GPU clusters (NVIDIA GPUs typical), inference on mobile devices (CPU/GPU/NPU depending on device)
  framework: Deep learning framework (likely TensorFlow or PyTorch, converted to mobile format via TensorFlow Lite for Android or Core ML for iOS)
  optimization: Optimized for mobile device deployment through model compression techniques (quantization to INT8/FP16, pruning, knowledge distillation)
  validation_split: "Standard train/validation/test split (exact ratios not specified, typical: 70/15/15 or 80/10/10)"
  training_parameters:
  epochs: "Not specified (typical: 50-200 epochs with early stopping)"
  batch_size: "Not specified (typical: 8-32 for medical image segmentation)"
  learning_rate: "Not specified in publication (typical range: 1e-4 to 1e-3 for segmentation tasks)"
  loss_function: Likely Dice loss or combined Dice + Cross-entropy (common for segmentation)
  data_augmentation: Likely used (rotation, scaling, color jittering typical for wound images)
platforms:
  - iOS
  - Android
deployment:
  privacy: Data processed locally on device, enhancing privacy and reducing data transmission requirements
  platform: Mobile (iOS and Android)
  performance: On-device processing enables real-time wound segmentation without internet connectivity
  optimization: Lightweight model for on-device processing
  offline_capability: Full functionality available offline, with optional cloud sync for physician access
ai_technology:
  privacy: On-device processing ensures data privacy and reduces need for internet connectivity
  framework: On-device deployment (likely TensorFlow Lite for Android or Core ML for iOS)
  deployment: On-device inference
  model_type: Deep Learning / Convolutional Neural Network (CNN)
  architecture: Lightweight deep learning model optimized for mobile deployment. Architecture details not fully disclosed in publication, but designed for on-device inference with minimal computational requirements. Likely uses encoder-decoder architecture (U-Net style) or MobileNet-based segmentation model for efficient mobile processing.
  capabilities:
  - Wound segmentation from photographs
  - Healing progression tracking
  - Automated wound assessment
  - Real-time processing on mobile devices
  optimization_techniques:
  - Model quantization for reduced size
  - Pruning for faster inference
  - Mobile-optimized architecture design
  performance_requirements: Optimized for real-time inference on mobile devices with limited computational resources
model_architecture:
  type: Lightweight deep learning model (CNN-based segmentation)
  inference: Real-time inference on mobile devices without cloud connectivity
  description: Deep learning model optimized for on-device deployment. Architecture designed for mobile devices with limited computational resources. Likely uses encoder-decoder architecture or MobileNet-based segmentation for efficient processing.
  optimization: Model optimized for mobile deployment through quantization (INT8 or FP16), pruning (removing less important connections), and architecture selection
  typical_metrics:
  note: Specific metrics for WoundAIssist model not reported in publication, focus was on usability rather than technical performance metrics
  accuracy_range: 85-95% IoU (Intersection over Union) for wound segmentation (typical range for similar models)
  inference_time: < 1 second per image (typical for mobile CNN segmentation)
  model_size_range: 2-15 MB (quantized, typical for mobile wound segmentation models)
  architecture_selection: Specific architecture not disclosed in publication. Selection likely based on trade-off between accuracy, model size, and inference speed for mobile deployment.
  possible_architectures:
  -
  name: U-Net style encoder-decoder
  advantages:
  - Proven effectiveness in medical imaging
  - Good balance between accuracy and model size
  description: Classical segmentation architecture with encoder (downsampling) and decoder (upsampling) paths. U-Net is commonly used for medical image segmentation tasks including wound segmentation.
  typical_size: 5-15 MB (quantized)
  -
  name: MobileNet-based segmentation
  advantages:
  - Very small model size
  - Fast inference
  - Optimized for mobile hardware
  description: Lightweight architecture using MobileNet as backbone with segmentation head. Designed specifically for mobile deployment.
  typical_size: 2-8 MB (quantized)
  -
  name: DeepLab Mobile
  advantages:
  - Good accuracy
  - Mobile-optimized
  - Efficient memory usage
  description: Mobile-optimized version of DeepLab architecture using depthwise separable convolutions.
  typical_size: 3-10 MB (quantized)
```

### WoundAIssist
**Type**: platform
**Status**: Published / Research prototype
**Development Stage**: Research / Preclinical
**Role in Project**: primary
**Relationship Description**: WoundAIssist mobile application - the main product of this research project
**Description**: A patient-centered mobile application that integrates a lightweight deep learning model for on-device wound segmentation, enabling patients to document wounds at home through photographs and questionnaires while physicians monitor progress remotely and conduct video consultations.
**Capabilities**:
- Wound segmentation from photographs
- Healing progression tracking
- Automated wound assessment
- Real-time processing on mobile devices
- Photograph wound documentation
- Patient questionnaires
- Remote physician monitoring
- Video consultations with physicians
- On-device AI wound segmentation
- User interface optimized for elderly patients
- Continuous wound healing monitoring
**Applications**:
- Telemedical wound care for patients with chronic wounds
- Remote monitoring for elderly patients
- Wound healing assessment and tracking
**Technical Details**:
```yaml
dataset:
  size: Not fully specified in publication, but includes wound images from patients with clinical annotations
  sources:
  - Wound images from patients with chronic wounds
  - Clinical annotations by dermatologists
  annotation: Clinical annotations by dermatologists providing ground truth for wound segmentation
  data_characteristics:
  - Diverse wound types and stages
  - Various lighting conditions
  - Different camera angles and distances
training:
  note: Specific training parameters not disclosed in publication, focus was on usability study rather than technical training details
  metrics: Segmentation accuracy (IoU, Dice coefficient), inference speed, model size, memory footprint
  approach: Supervised learning on annotated wound images
  hardware: Training likely performed on GPU clusters (NVIDIA GPUs typical), inference on mobile devices (CPU/GPU/NPU depending on device)
  framework: Deep learning framework (likely TensorFlow or PyTorch, converted to mobile format via TensorFlow Lite for Android or Core ML for iOS)
  optimization: Optimized for mobile device deployment through model compression techniques (quantization to INT8/FP16, pruning, knowledge distillation)
  validation_split: "Standard train/validation/test split (exact ratios not specified, typical: 70/15/15 or 80/10/10)"
  training_parameters:
  epochs: "Not specified (typical: 50-200 epochs with early stopping)"
  batch_size: "Not specified (typical: 8-32 for medical image segmentation)"
  learning_rate: "Not specified in publication (typical range: 1e-4 to 1e-3 for segmentation tasks)"
  loss_function: Likely Dice loss or combined Dice + Cross-entropy (common for segmentation)
  data_augmentation: Likely used (rotation, scaling, color jittering typical for wound images)
platforms:
  - iOS
  - Android
deployment:
  privacy: Data processed locally on device, enhancing privacy and reducing data transmission requirements
  platform: Mobile (iOS and Android)
  performance: On-device processing enables real-time wound segmentation without internet connectivity
  optimization: Lightweight model for on-device processing
  offline_capability: Full functionality available offline, with optional cloud sync for physician access
ai_technology:
  privacy: On-device processing ensures data privacy and reduces need for internet connectivity
  framework: On-device deployment (likely TensorFlow Lite for Android or Core ML for iOS)
  deployment: On-device inference
  model_type: Deep Learning / Convolutional Neural Network (CNN)
  architecture: Lightweight deep learning model optimized for mobile deployment. Architecture details not fully disclosed in publication, but designed for on-device inference with minimal computational requirements. Likely uses encoder-decoder architecture (U-Net style) or MobileNet-based segmentation model for efficient mobile processing.
  capabilities:
  - Wound segmentation from photographs
  - Healing progression tracking
  - Automated wound assessment
  - Real-time processing on mobile devices
  optimization_techniques:
  - Model quantization for reduced size
  - Pruning for faster inference
  - Mobile-optimized architecture design
  performance_requirements: Optimized for real-time inference on mobile devices with limited computational resources
model_architecture:
  type: Lightweight deep learning model (CNN-based segmentation)
  inference: Real-time inference on mobile devices without cloud connectivity
  description: Deep learning model optimized for on-device deployment. Architecture designed for mobile devices with limited computational resources. Likely uses encoder-decoder architecture or MobileNet-based segmentation for efficient processing.
  optimization: Model optimized for mobile deployment through quantization (INT8 or FP16), pruning (removing less important connections), and architecture selection
  typical_metrics:
  note: Specific metrics for WoundAIssist model not reported in publication, focus was on usability rather than technical performance metrics
  accuracy_range: 85-95% IoU (Intersection over Union) for wound segmentation (typical range for similar models)
  inference_time: < 1 second per image (typical for mobile CNN segmentation)
  model_size_range: 2-15 MB (quantized, typical for mobile wound segmentation models)
  architecture_selection: Specific architecture not disclosed in publication. Selection likely based on trade-off between accuracy, model size, and inference speed for mobile deployment.
  possible_architectures:
  -
  name: U-Net style encoder-decoder
  advantages:
  - Proven effectiveness in medical imaging
  - Good balance between accuracy and model size
  description: Classical segmentation architecture with encoder (downsampling) and decoder (upsampling) paths. U-Net is commonly used for medical image segmentation tasks including wound segmentation.
  typical_size: 5-15 MB (quantized)
  -
  name: MobileNet-based segmentation
  advantages:
  - Very small model size
  - Fast inference
  - Optimized for mobile hardware
  description: Lightweight architecture using MobileNet as backbone with segmentation head. Designed specifically for mobile deployment.
  typical_size: 2-8 MB (quantized)
  -
  name: DeepLab Mobile
  advantages:
  - Good accuracy
  - Mobile-optimized
  - Efficient memory usage
  description: Mobile-optimized version of DeepLab architecture using depthwise separable convolutions.
  typical_size: 3-10 MB (quantized)
```

## Key People

### Astrid Schmieder
**Participation Type**: researcher
**Role in Project**: Co-author
**Affiliations**: University Hospital Würzburg
**Contribution**: Clinical expertise and validation
**Expertise**: Dermatology, Wound care, Clinical validation
**Biography**: Dermatologist at University Hospital Würzburg, Department of Dermatology

### Anna Riedmann
**Participation Type**: researcher
**Role in Project**: Co-author
**Affiliations**: University of Würzburg
**Contribution**: Research and development
**Expertise**: Computer Science, Human-Computer Interaction, Mobile application development
**Biography**: Researcher at University of Würzburg, Department of Computer Science / Human-Computer Interaction

### Samuel Kounev
**Participation Type**: pi
**Role in Project**: Corresponding Author / Principal Investigator
**Affiliations**: University of Würzburg
**Contribution**: Principal investigator, research supervision
**Expertise**: Computer Science, Research supervision, Human-Computer Interaction
**Biography**: Professor at University of Würzburg, Department of Computer Science. Principal Investigator for the WoundAIssist project.

### Konstantin Müller
**Participation Type**: researcher
**Role in Project**: Co-author
**Affiliations**: University of Würzburg
**Contribution**: Research and development
**Expertise**: Computer Science, Human-Computer Interaction, Mobile application development
**Biography**: Researcher at University of Würzburg, Department of Computer Science / Human-Computer Interaction

### Birgit Lugrin
**Participation Type**: researcher
**Role in Project**: Co-author
**Affiliations**: University of Würzburg
**Contribution**: Research and development
**Expertise**: Computer Science, Human-Computer Interaction, Mobile application development
**Biography**: Researcher at University of Würzburg, Department of Computer Science / Human-Computer Interaction

### Vanessa Borst
**Participation Type**: researcher
**Role in Project**: Co-author
**Affiliations**: University of Würzburg
**Contribution**: Research and development
**Expertise**: Computer Science, Human-Computer Interaction, Mobile application development
**Biography**: Researcher at University of Würzburg, Department of Computer Science / Human-Computer Interaction

### Tassilo Dege
**Participation Type**: researcher
**Role in Project**: Co-author
**Affiliations**: University of Würzburg
**Contribution**: Research and development
**Expertise**: Computer Science, Human-Computer Interaction, Mobile application development
**Biography**: Researcher at University of Würzburg, Department of Computer Science / Human-Computer Interaction

## Links

### [MobileNets: Efficient Convolutional Neural Networks for Mobile Vision Applications](https://arxiv.org/abs/1704.04861)
**Type**: research_publication
**Relevance**: secondary
**Category**: reference
**Relationship Description**: Foundation paper on MobileNet architecture for mobile AI
**Publisher**: arXiv
**Publication Date**: 2017-04-01
**Description**: Foundation paper on MobileNet architecture, commonly used for mobile AI applications. Provides technical background for mobile-optimized models.

### [Wound3DAssist: A Practical Framework for 3D Wound Assessment](https://arxiv.org/abs/2508.17635)
**Type**: research_publication
**Relevance**: secondary
**Category**: research
**Relationship Description**: Related research on 3D wound assessment for comparison
**Publisher**: arXiv
**Publication Date**: 2025-08-01
**Description**: Related research on 3D wound assessment using smartphone video. Provides comparison point for 2D vs 3D approaches in wound segmentation.

### [WoundAIssist: A Patient-Centered Mobile App for AI-Assisted Wound Care With Physicians in the Loop](https://arxiv.org/abs/2506.06104)
**Type**: research_publication
**Relevance**: primary
**Category**: source
**Relationship Description**: Primary research publication describing the WoundAIssist mobile application
**Publisher**: arXiv
**Publication Date**: 2025-06-06
**Description**: Primary research publication describing the WoundAIssist mobile application, its development, methodology, and usability study results. Published on arXiv in June 2025. DOI: 10.48550/arXiv.2506.06104

### [TensorFlow Lite: Machine Learning for Mobile and Edge Devices](https://www.tensorflow.org/lite)
**Type**: documentation
**Relevance**: secondary
**Category**: documentation
**Relationship Description**: TensorFlow Lite documentation for mobile deployment
**Publisher**: TensorFlow
**Description**: Official documentation for TensorFlow Lite, framework for edge AI deployment

### [Deepwound: Automated Postoperative Wound Assessment](https://arxiv.org/abs/1807.04355)
**Type**: research_publication
**Relevance**: secondary
**Category**: research
**Relationship Description**: Early work on automated wound assessment for historical context
**Publisher**: arXiv
**Publication Date**: 2018-07-01
**Description**: Early work on automated wound assessment using CNNs. Focuses on surgical wounds and provides historical context for wound segmentation research.

### [Multi-Analyte, Swab-based Automated Wound Monitor with AI](https://arxiv.org/abs/2506.03188)
**Type**: research_publication
**Relevance**: secondary
**Category**: research
**Relationship Description**: Alternative sensor-based approach for comparison
**Publisher**: arXiv
**Publication Date**: 2025-06-01
**Description**: Alternative approach to wound monitoring using physical sensors. Provides comparison for image-based vs sensor-based wound assessment.

### [A Mobile App for Wound Localization using Deep Learning](https://arxiv.org/abs/2009.07133)
**Type**: research_publication
**Relevance**: secondary
**Category**: research
**Relationship Description**: Related research on mobile wound localization
**Publisher**: arXiv
**Publication Date**: 2020-09-01
**Description**: Related research on mobile wound localization. Provides context for mobile deep learning applications in wound care.

### [U-Net: Convolutional Networks for Biomedical Image Segmentation](https://arxiv.org/abs/1505.04597)
**Type**: research_publication
**Relevance**: secondary
**Category**: reference
**Relationship Description**: Seminal paper on U-Net architecture for medical image segmentation
**Publisher**: arXiv
**Publication Date**: 2015-05-01
**Description**: Seminal paper on U-Net architecture, commonly used for medical image segmentation including wound segmentation. Provides technical background for likely architecture used in WoundAIssist.

### [Core ML: Machine Learning Framework for Apple Devices](https://developer.apple.com/machine-learning/core-ml/)
**Type**: documentation
**Relevance**: secondary
**Category**: documentation
**Relationship Description**: Core ML documentation for iOS deployment
**Publisher**: Apple
**Description**: Official documentation for Core ML, framework for edge AI on iOS devices
