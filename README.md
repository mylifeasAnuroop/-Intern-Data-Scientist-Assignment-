# Project: Subtheme Sentiment Analysis Task 
### Author : Anuroop Arya

[Click here to view the code file](https://github.com/mylifeasAnuroop/-Intern-Data-Scientist-Assignment-/blob/main/Oriserve_Intern_Assignment_.ipynb)
Subtheme Sentiment Analysis Task
Take the following example:
“One tyre went missing, so there was a delay to get the two tyres fitted. The way garage dealt
with it was fantastic.”
In this review there are numerous insights, insights we call “subtheme sentiments”. A Subtheme
sentiment is generally a sentiment towards an aspect or a problem.
If we look at the subtheme sentiments of the above review we will get a clearer sense what these
generally are.
incorrect tyres sent negative garage service positive wait time negative
The main difference between these subthemes is that Garage Service and Wait Time are aspects
of the service that can be positive or negative while
Incorrect Tyres Sent denotes a problem, something inherently negative.
Task
The task is to develop an approach that given a sample will identify the subthemes along with
their respective sentiments.

 
## Overview
The goal of this project is to create text in response to prompts, conduct sentiment analysis on subthemes that have been derived from text data, and format the output in Markdown.



## Approach
### Step-by-Step Approach

1. **Load and Prepare the Dataset**
   - **Library Imports:** Import necessary libraries such as pandas, transformers, textwrap, Markdown, and google.generativeai.
   - **Load Dataset:** Load the dataset containing text data from which subthemes will be extracted.
  

2. **Initialize Sentiment Analysis Pipeline**
   - **Sentiment Analysis:** Use the Hugging Face `pipeline` for sentiment analysis to categorize text into positive and negative sentiments.
   ```python
   mood_detector = pipeline("sentiment-analysis")
   ```

3. **Configure Generative AI API**
   - **Generative AI API:** Configure the Google Generative AI API with your API key for content generation.
   ```python
   genai.configure(api_key="YOUR_GENERATIVE_AI_API_KEY")
   ```

4. **Select Generative Model for Content Generation**
   - **List and Select Models:** List available generative models and select one for content generation. Example:


5. **Convert Text to Markdown Format**
   - **Markdown Conversion:** Define a function to convert generated text into Markdown format for easy readability and presentation.


6. **System Prompt Definition**
   - **Define System Prompt:** Define a system prompt that will be used to generate content.

 
7. **Format Response into Pros and Cons**
   - **Pros and Cons Analysis:** Define a function to format the generated text into pros and cons based on sentiment analysis results.
   - 

8. **Generate Content and Display**
   - **Content Generation:** Use the generative model to respond to the system prompt and the dataset.
   - **Display Formatted Response:** Format the response into pros and cons and display it in Markdown format.

### Improvements
There are drawbacks to the current strategy in:
- **Accuracy of Sentiment Analysis:** Sentiment analysis might occasionally misclassify complex feelings.
- **material Coherence:** Because of the generative model's limitations, the generated material may not be coherent.

The following are the improvements: **Advanced Sentiment Analysis:** Use aspect-based sentiment analysis to classify sentiment more precisely.
- **Enhanced work Generation:** Try out more complex generative models to raise the caliber and coherence of your work.

## Final Thoughts 
Using cutting-edge AI models, this project offers a straightforward but creative solution for sentiment analysis and content creation for subthemes. The provided insights' accuracy and usability can be improved further.
