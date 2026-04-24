# VitaAssist: Interpretable Machine Learning for Pediatric Vitamin A Deficiency Detection

**VitaAssist** is a web-based screening tool designed to identify children at risk of Vitamin A Deficiency (VAD) using opthalmic and demographic data. By utilizing a Random Forest classifier and SHAP (SHapley Additive exPlanations), the system provides transparent risk assessments to healthcare workers in low-resource environments.

# Key Features
 **Non-Invasive Screening:** Predicts risk using ocular symptoms and demographic data instead of invasive blood tests.
 **Explainable AI (XAI):** Integrated SHAP reasoning to visualize exactly which clinical symptoms triggered a "High Risk" classification.
 **Offline Functionality:** Developed as a lightweight Flask-based web application capable of LAN-based deployment for rural areas without internet access.
 **Secure Data Archiving:** MySQL integration to track child demographics and screening history over time.

# Tech Stack
 **Language:** Python 3.7.4+

**Machine Learning:** Random Forest Classifier, SHAP Library

 **Backend:** Flask
 
 **Frontend:** HTML5, CSS3, Bootstrap

 **Database:** MySQL (WampServer)

# VitaAssist Dashboard
[View VitaAssist Dashboard Screenshots](web.pdf)

# System Architecture
The system follows a modular architecture:
1. **Data Pipeline:** Raw clinical data is cleaned and normalized.
2. **Inference Engine:** Features are processed by the pre-trained Random Forest model.
3. **Interpretability Layer:** SHAP calculates feature contributions for every prediction.
4. **UI Dashboard:** Results and dietary recommendations are displayed via a Bootstrap interface.

# Results

Predictive Performance: The Random Forest model successfully categorizes risk levels, providing a reliable risk probability score for early screening.  
**​Diagnostic Efficiency:** The system prioritizes significant clinical attributes, reducing the need for exhaustive data entry and computational overhead.  

**​Visual Interpretability:** SHAP reasoning effectively identifies specific ocular and demographic triggers, generating bar graphs to explain "High Risk" flags to health workers.  

**​System Reliability:** The Flask-based deployment ensures high-speed processing and model stability while maintaining data security via MySQL.

**​Clinical Impact:** By replacing invasive blood tests with non-invasive clinical records, the tool minimizes human error and significantly saves time during mass screenings.  
