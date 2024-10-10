
# United Airlines Call Center Optimization - Hackathon Project

## Project Overview

This project was developed during SKYHACK 2.0 Hackathon with the goal of optimizing United Airlines' call center metrics. We analyzed call center data to identify inefficiencies in **Average Handle Time (AHT)** and **Average Speed to Answer (AST)**, proposed solutions to reduce these times, and recommended strategies for improving customer satisfaction and operational efficiency.

### Team Members
- Gautam Pubreja
- Arsh Sharma

## Problem Statement

Call centers are a vital part of customer service for United Airlines. However, challenges in long AHT and AST were identified, which negatively impacted customer satisfaction. Our task was to:
- Analyze existing call center data to identify drivers of long AHT and AST.
- Suggest strategies to reduce call resolution times and enhance customer satisfaction.

## To run the project:

1. Clone the repository or download the project files.
2. Ensure you have Python 3.x installed.
3. Create a virtual environment (optional but recommended):
```
python -m venv env
```
```
source env/bin/activate #(for Linux/Mac)
.\env\Scripts\activate #(for Windows)
```
4. Install the dependencies:
```
pip install -r requirements.txt
```
## Objectives

1. **AHT and AST Reduction**: 
   - Identify factors driving long call handling times.
   - Analyze agent performance, call types, and customer sentiment.
   - Recommend solutions to reduce average handle times, focusing on both agent and customer-side analysis.

2. **IVR System Enhancement**:
   - Explore self-solvable issues.
   - Suggest improvements to the Interactive Voice Response (IVR) system to reduce agent workload by enabling faster resolutions through self-service options.

3. **Machine Learning Model**:
   - Classify primary call reasons to streamline processes and direct customers to the appropriate resource or service.

## Dataset Overview

The project used several datasets including:

- **calls.csv**: Contains details like start and end times of calls and agent information.
- **customers.csv**: Contains data about customers involved in the calls.
- **reason.csv**: Lists reasons for each customer service call.
- **sentiment.csv**: Analyzes the sentiment of both agents and customers during calls.

## Key Insights & Findings

1. **Agent Performance**:
   - Agents with a neutral tone exhibited the longest handle times.
   - Agents using a polite tone had shorter handle times.

2. **Customer Sentiment**:
   - Customer sentiment had little effect on the handle time.

3. **Call Reasons**:
   - Most frequent call reason: **Irregular Operations (IRROPS)**, with an average handle time of 13.08 minutes.
   - Least frequent call reason: **Unaccompanied Minor**, with an average handle time of 8.65 minutes.
   - Percentage difference in handle times between the most frequent and least frequent call reasons: **51.2%**.

## Recommendations

1. **Agent Training**:
   - Focus on improving the performance of neutral-toned agents.
   - Prioritize frequent call reasons like IRROPS with better support systems to enhance call handling efficiency.

2. **Sentiment Analysis**:
   - Integrate real-time sentiment analysis to improve agent-customer dynamics and improve response times.

3. **IVR System Enhancements**:
   - Dynamic routing based on real-time analysis of customer tone and call reason.
   - Implement NLP to enable customers to voice their needs naturally for faster resolution.
   - Offer simplified menu structures with real-time updates on services like flight status to reduce unnecessary agent escalations.

4. **Machine Learning for Call Categorization**:
   - Train and deploy a model to classify call reasons based on transcripts, improving call routing and reducing manual tagging.

## Technologies Used

- **Python**: For data analysis, preprocessing, and building machine learning models.
- **Pandas**: Used for dataset cleaning and merging.
- **Scikit-learn**: Used for feature extraction and building the classification model (Random Forest).
- **NLP techniques**: Text cleaning, TF-IDF vectorization for call transcript analysis.

## Future Improvements

- **Model Refinement**: Improve classification model accuracy by handling imbalanced data and better preprocessing of noisy text data.
- **Enhanced IVR Pathways**: Implement AI-based self-service systems to reduce the burden on human agents further.
- **Feedback Loop**: Continuously analyze agent feedback and customer success rates to improve IVR and call classification systems.

