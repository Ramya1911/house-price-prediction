<h1 align="center">🏠 House Price Prediction Project</h1>

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.10-blue?logo=python">
  <img src="https://img.shields.io/badge/Flask-Web%20Framework-black?logo=flask">
  <img src="https://img.shields.io/badge/Scikit--Learn-ML-orange?logo=scikitlearn">
  <img src="https://img.shields.io/badge/Deployment-Render-purple?logo=render">
  <img src="https://img.shields.io/badge/Status-Live-success">
  <img src="https://img.shields.io/badge/License-Educational-green">
</p>

<hr>

<h2>📑 Table of Contents</h2>
<ol>
<li>Acknowledgements</li>
<li>Project Overview</li>
<li>Dataset Description</li>
<li>Project Structure</li>
<li>Technology Stack</li>
<li>Implementation Steps</li>
<li>Code Explanation</li>
<li>Model Development</li>
<li>Deployment Process</li>
<li>Results and Output</li>
<li>Challenges and Solutions</li>
<li>Future Enhancements</li>
<li>Conclusion</li>
<li>References</li>
</ol>

<hr>

<h2>1️⃣ Acknowledgements</h2>

<h3>Dataset Source</h3>
<ul>
<li><strong>Dataset Name:</strong> House Sales in King County, USA</li>
<li><strong>Source:</strong> Kaggle - House Data dataset</li>
<li><strong>Contributor:</strong> Shreya Chaudhary</li>
<li><strong>Original Context:</strong> Contains house sale prices for King County including Seattle (May 2014 – May 2015).</li>
</ul>

<h3>Tools and Libraries</h3>
<ul>
<li>Flask</li>
<li>Scikit-learn</li>
<li>NumPy</li>
<li>Pickle</li>
<li>Pandas</li>
<li>HTML/CSS</li>
<li>Render</li>
<li>Git/GitHub</li>
</ul>

<h3>Special Thanks</h3>
<ul>
<li>Kaggle Community</li>
<li>Open-source contributors</li>
<li>Render hosting platform</li>
</ul>

<hr>

<h2>2️⃣ Project Overview</h2>

<h3>🎯 Objective</h3>
<p>
Develop a machine learning web application to predict house prices based on multiple property and temporal features.
</p>

<h3>📌 Problem Statement</h3>
<ul>
<li>Create predictive model using historical data</li>
<li>Build intuitive web interface</li>
<li>Deploy publicly</li>
<li>Provide accurate estimations</li>
</ul>

<h3>✨ Key Features</h3>
<ul>
<li>Responsive UI</li>
<li>Real-time predictions</li>
<li>17 input features</li>
<li>Live deployed application</li>
</ul>

<hr>

<h2>3️⃣ Dataset Description</h2>

<h3>Dataset Specifications</h3>
<ul>
<li><strong>Total Records:</strong> 21,613 houses</li>
<li><strong>Features:</strong> 18 columns</li>
<li><strong>Time Period:</strong> May 2014 – May 2015</li>
<li><strong>Location:</strong> King County, Washington, USA</li>
</ul>

<h3>Data Preprocessing Steps</h3>
<ol>
<li>Handling missing values</li>
<li>Feature Engineering
    <ul>
        <li>Extracted year, month, day</li>
        <li>Encoded city and country</li>
    </ul>
</li>
<li>Feature selection (17 features)</li>
<li>Normalization (if required)</li>
</ol>

<hr>

<h2>4️⃣ Project Structure</h2>

<pre>
House-Price-Prediction/
│
├── app.py
├── MINI_PROJECT.pkl
├── requirements.txt
├── Procfile
├── templates/
│   └── index.html
├── static/
│   ├── style.css
│   └── images/
└── dataset.csv
</pre>

<hr>

<h2>5️⃣ Technology Stack</h2>

<h3>Backend</h3>
<ul>
<li>Python</li>
<li>Flask</li>
<li>Scikit-learn</li>
<li>Pandas</li>
<li>NumPy</li>
<li>Pickle</li>
</ul>

<h3>Frontend</h3>
<ul>
<li>HTML5</li>
<li>CSS3</li>
</ul>

<h3>Development Tools</h3>
<ul>
<li>PyCharm</li>
<li>Git</li>
<li>GitHub</li>
<li>Jupyter Notebook</li>
</ul>

<h3>Deployment</h3>
<ul>
<li>Render</li>
<li>Pip</li>
</ul>

<hr>

<h2>6️⃣ Implementation Steps</h2>

<h3>Step 1: Environment Setup</h3>
<pre>
python -m venv venv
venv\Scripts\activate
pip install flask numpy pandas scikit-learn gunicorn
</pre>

<h3>Step 2: Data Analysis and Model Training</h3>
<ul>
<li>Load dataset</li>
<li>EDA</li>
<li>Preprocessing</li>
<li>Train-test split (80/20)</li>
<li>Train Linear Regression</li>
<li>Evaluate</li>
<li>Save model (pickle)</li>
</ul>

<h3>Step 3: Flask Application</h3>
<ul>
<li>Create routes</li>
<li>Load model</li>
<li>Prediction endpoint</li>
<li>Form handling</li>
</ul>

<h3>Step 4: Frontend Development</h3>
<ul>
<li>Design form</li>
<li>CSS styling</li>
<li>Responsive layout</li>
</ul>

<h3>Step 5: Local Testing</h3>
<pre>
python app.py
http://127.0.0.1:5000
</pre>

<h3>Step 6: GitHub Upload</h3>
<ul>
<li>Create repository</li>
<li>Upload files</li>
<li>Copy repo URL</li>
</ul>

<h3>Step 7: Render Deployment</h3>
<ul>
<li>Create Web Service</li>
<li>Select Python</li>
<li>Install dependencies</li>
<li>Start with gunicorn</li>
<li>Live URL generated</li>
</ul>

<hr>

<h2>7️⃣ Code Explanation</h2>

<h3>Custom Linear Regression Implementation</h3>

<h4>Imports</h4>
<pre>
import numpy as np
import pandas as pd
import sklearn
import sys
</pre>

<h4>Class: MINIPROJECT</h4>
<ul>
<li>Data Loading</li>
<li>Preprocessing</li>
<li>Training</li>
<li>Testing</li>
</ul>

<h4>Feature Engineering</h4>
<ul>
<li>Date extraction</li>
<li>City frequency encoding</li>
<li>Country mapping</li>
</ul>

<h4>Training</h4>
<ul>
<li>Matrix operations</li>
<li>Normal equation</li>
<li>MSE, RMSE</li>
<li>R² Score</li>
</ul>

<h4>Testing</h4>
<ul>
<li>Test predictions</li>
<li>Test RMSE</li>
<li>Test R²</li>
</ul>

<h4>Flask Routes</h4>
<ul>
<li>/ (Home)</li>
<li>/predict</li>
</ul>

<h4>17 Input Features</h4>
<ul>
<li>bedrooms</li>
<li>bathrooms</li>
<li>sqft_living</li>
<li>sqft_lot</li>
<li>floors</li>
<li>waterfront</li>
<li>view</li>
<li>condition</li>
<li>sqft_above</li>
<li>sqft_basement</li>
<li>yr_built</li>
<li>yr_renovated</li>
<li>city</li>
<li>country</li>
<li>year</li>
<li>month</li>
<li>day</li>
</ul>

<hr>

<h2>8️⃣ Model Development</h2>

<h3>Model: Linear Regression</h3>
<ul>
<li>Interpretable</li>
<li>Efficient</li>
<li>Baseline regression model</li>
</ul>

<h3>Metrics</h3>
<ul>
<li>R² Score</li>
<li>MSE</li>
<li>RMSE</li>
</ul>

<hr>

<h2>9️⃣ Deployment Process</h2>

<ul>
<li>Create GitHub repo</li>
<li>Connect to Render</li>
<li>Build: pip install -r requirements.txt</li>
<li>Start: gunicorn app:app</li>
<li>Live URL generated</li>
</ul>

<hr>

<h2>🔟 Results and Output</h2>

<h3>Application Interface</h3>
<ul>
<li>User-friendly form</li>
<li>Styled prediction result</li>
<li>Interactive UI</li>
</ul>

<h3>Sample Output</h3>
<p><strong>Estimated House Price:</strong> 1201490.48966</p>

<h3>Performance</h3>
<ul>
<li>Response Time: &lt; 2 seconds</li>
<li>24/7 availability</li>
</ul>

<hr>

<h2>1️⃣1️⃣ Challenges and Solutions</h2>
<ul>
<li>Encoding categorical features</li>
<li>Model persistence using pickle</li>
<li>String-to-float conversion</li>
<li>Deployment dependency issues</li>
</ul>

<hr>

<h2>1️⃣2️⃣ Future Enhancements</h2>
<ul>
<li>Random Forest</li>
<li>Gradient Boosting</li>
<li>Neural Networks</li>
<li>Docker</li>
<li>Monitoring & Logging</li>
</ul>

<hr>

<h2>1️⃣3️⃣ Conclusion</h2>

<p>
Complete end-to-end ML pipeline including preprocessing, model training, Flask integration, and cloud deployment.
</p>

<ul>
<li>Full-stack ML application</li>
<li>Production deployment</li>
<li>Cloud integration</li>
</ul>

<hr>

<h2>1️⃣4️⃣ References</h2>
<ul>
<li>Flask Documentation</li>
<li>Scikit-learn Documentation</li>
<li>Render Documentation</li>
<li>Bootstrap Documentation</li>
</ul>

<hr>

<h3 align="center">👩‍💻 Project By: K. RAMYA</h3>
<p align="center">📅 Last Updated: 10-02-2026</p>
<p align="center">🌐 Live Application: Project link</p>
<p align="center">📂 GitHub Repository: github repo</p>
