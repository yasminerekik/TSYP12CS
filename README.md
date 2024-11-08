# ENIGUARD 
# "Empowering Real-Time Defense with AI"
SMARTSHIELD:  AI-Driven Cybersecurity Incident Response Automation

The SMARTSHIELD project introduces an AI-driven solution to detect and mitigate Distributed Denial of Service (DDoS) attacks automatically. 
Using the CatBoost classification model, this solution integrates effectively within an existing cybersecurity infrastructure to enhance resilience, detection accuracy, and operational efficiency.

# Problem Description
DDoS attacks pose a rising threat to service availability, causing major financial losses for organizations. Current defenses are limited: on-premise solutions can’t handle large-scale attacks, and automated detection is costly and resource-intensive, struggling with prolonged attacks. ENIGUARD overcomes these issues with a powerful, automated response system for effective DDoS detection and mitigation.

# Problem Implementation 
This solution uses a supervised machine learning framework with the CatBoost algorithm to improve DDoS detection. Trained as a classification model, CatBoost distinguishes between normal traffic and malicious activity, making it well-suited for identifying DDoS attack patterns.
The model configuration is tuned to maximize detection accuracy and F1 score.

# Methodology for Each Step 
### Step 1: Model Preparation
1. **Data Loading and Exploration**: The dataset is imported with Pandas, and exploratory analysis is conducted to understand the structure and identify any anomalies.
2. **Preprocessing**: Numerical data is normalized, and categorical variables are encoded for compatibility.
3. **Model Creation**: CatBoost is selected for its accuracy and effective handling of categorical data. Parameters are optimized for DDoS detection.
4. **Training and Validation**: The model is trained and fine-tuned to maximize precision and recall.
5. **Evaluation**: Metrics like Accuracy and F1 Score confirm CatBoost’s effectiveness.

![image](https://github.com/user-attachments/assets/dac98226-a21a-4677-9e90-819d8dbf9813)


### Step 2: Model Dockerization
- **Deployment**: A Docker setup with a Python script and requirements file enables easy deployment. The model is hosted on Hugging Face, and API functionality is verified with Postman.

### Step 3: Network Architecture
- **Infrastructure**: The setup includes ELK for log centralization, a pfSense firewall, an IDS/IPS, and a SOAR system for automated response.

### Step 4: Model Integration and Visualization
- **Kibana Integration**: The model’s DDoS detection is visualized in Kibana, allowing real-time monitoring and response demonstration.


