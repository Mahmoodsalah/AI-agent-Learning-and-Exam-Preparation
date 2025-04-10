
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1R5mFGDCU27KA6tMDpr15CwlP8MCpMEJM?usp=sharing)


# AI-Powered Learning and Exam Preparation Notebook

This Google Colab notebook leverages the power of AI to enhance learning and exam preparation through various functionalities:

## Features

1. **Study Partner:** 
   - Uses the `agno` library with the `OpenAIChat` model and tools like `ExaTools` and `YouTubeTools` to create a study partner agent named StudyScout.
   - Assists in finding resources, answering questions, and providing explanations on various topics.
   - Generates personalized study plans, recommends learning resources, and offers tips for effective learning.

2. **Exam Preparation:**
   - Utilizes the `agno` library with the `OpenAIChat` model to create an exam preparation agent named ExamPrepGPT.
   - Processes uploaded PDF study materials using `PyMuPDF`.
   - Generates quizzes, flashcards, and summaries based on the PDF content.
   - Explains difficult concepts and encourages active recall through Q&A.

3. **Handwritten Essay Evaluation:**
   - Employs the `OpenAI` API with the `gpt-4o` model to evaluate handwritten essays.
   - Uploads images of handwritten essays using `google.colab.files`.
   - Provides feedback and a score similar to the IELTS writing test out of 9.

## Usage

1. **Setup:**
   - Install necessary libraries: `agno`, `exa_py`, `youtube_transcript_api`, `python-dotenv`, `pymupdf`, `Pillow`, `openai`.
   - Set up environment variables for API keys (OPENAI_API_KEY, EXA_API_KEY).

2. **Study Partner:**
   - Define the `study_partner` agent with desired instructions.
   - Provide a topic and learning preferences to receive a study plan and resources.

3. **Exam Preparation:**
   - Define the `exam_prep_agent` with desired instructions.
   - Upload a PDF study material using `google.colab.files`.
   - Extract text from the PDF using `PyMuPDF`.
   - Provide the extracted text to the agent to generate quizzes, flashcards, and summaries.

4. **Handwritten Essay Evaluation:**
   - Upload an image of the handwritten essay using `google.colab.files`.
   - Encode the image as base64.
   - Send the encoded image to the `gpt-4o` model using the `OpenAI` API.
   - Receive feedback and a score for the essay.

## Requirements

- Google Colab environment
- Python 3
- Required libraries (listed in the "Usage" section)
- API keys for OpenAI and Exa (optional)

## Disclaimer

- This notebook is for educational and experimental purposes.
- The accuracy and reliability of the AI-generated content may vary.
- Users are responsible for verifying the information and using it responsibly.
