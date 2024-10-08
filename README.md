# CS7641 ML Study Materials 2023
A collection of study materials for OMSCS CS7641 Machine Learning.

## 2024 Update: Check out [_mlrose-ky_](https://github.com/knakamura13/mlrose-ky) now!
_mlrose-ky_ is my fork of _mlrose-hiive_. I'm adding extensive documentation, bugfixes, unit tests, code optimizations, and more! 

New PyPi package now available! Try it out with `pip install mlrose-ky` and use it as a replacement for `mlrose-hiive`. https://pypi.org/project/mlrose-ky/

## Study Materials

### Lecture Transcripts

`./Lecture Transcripts/` includes a complete copy of the course lectures in text format.

**How it was made**

These transcripts were created by downloading the lecture videos from Canvas, converting the subtitle (.srt) files to plain text, using regex to remove the subtitle formatting, then organizing the text files by chapter, module, and lecture title.

### Lecture Summaries

`./Lecture Summaries/` includes three PDFs containing individual summaries of the course lectures.

**How it was made**

I used GPT-4 to recursively summarize the lecture transcripts. See my [Recursive Lecture Summarizer](https://github.com/knakamura13/recursive-lecture-summarizer) project for more information.

### Practice Quizzes

`./Practice Quizzes/` includes 19 multiple-choice practice quizzes, each pertaining to one of the 19 modules from the course.

### Practice Exams

`./Practice Exams/` includes 2 multiple-choice practice exams covering key concepts from modules covered by the midterm and final exams.

**How it was made**

I used GPT-3 and GPT-4 to recursively summarize the lecture transcripts. The transcripts were acquired by converting the video subtitles into plain text, stripping out the subtitle formatting, and combining the hundreds of text files into one. The transcripts were then condensed to 1% of their original size, starting with over 1.5 million characters and ending with around 15,000.
 
This process made it possible to copy all the lectures into a single ChatGPT prompt.

Here is the prompt that I used to create the practice final exam:

> The following text is a summary of the transcripts from the lectures in CS7641 ML. Use the information in the summary to get an idea of what was taught in this course. 
> 
> Then, create a practice exam with 50 questions, following these rules:  
> 1. The questions are multiple-choice, with multiple correct options per question.  
> 2. Each question has at least one correct option but no more than three correct options.  
> 3. Each question has four options.
> 4. The options are labeled A, B, C, D. 
> 5. The exam is difficult but not impossible.
> 6. Try to disambiguate the options and avoid writing questions that rely on a technicality or a "trick" answer. 
> 
> Do not show me the answers. Instead, show me an answer key at the end of your response so that I can test myself. 
>  
> Here is the summary of the transcribed lectures (delimited by triple quotes):
> 
> """
> SUMMARY OF LECTURE TRANSCRIPTS
> """

## Other tools and resources

- [🤗 Dataset Toolkit](https://github.com/knakamura13/huggingface-dataset-toolkit) (by Kyle Nakamura)
    - This repository contains Python code that automates the process of downloading, cleaning, and saving datasets. The code uses Huggingface's datasets library to download the datasets and utilizes pandas and scikit-learn for preprocessing tasks such as one-hot encoding. I created this tool to enable rapid experimenting with different ML models and it should be particularly useful for ML Assignment 1.
- [Recursive Lecture Summarizer](https://github.com/knakamura13/recursive-lecture-summarizer) (by Kyle Nakamura)
    - This project features a GPT-powered text summarizer designed to efficiently condense large documents into concise summaries. It focuses on extracting key information while maintaining the core essence of the original text, and uses a "chunking" methodology to make the summarization task easier for the ML model.
- [LaTeX templates for the 4 assignments](https://github.com/knakamura13/cs7641-ml-study-materials-2023/tree/main/Report%20LaTeX%20Templates) (by Kyle Nakamura)
    - The `/Report LaTex Templates` directory contains 4 templates that can be used for the 4 assignments. To use one, sign in to [Overleaf](https://www.overleaf.com/) with your GATech credentials, click "New Project", and then "Upload Project".
- UPDATE! Check out _mlrose-ky_, my fork of _mlrose-hiive_ where I'm adding extensive documentation, bugfixes, unit tests, code optimizations, and more! New PyPi package now available! Try it out with `pip install mlrose-ky` and use it as a replacement for `mlrose-hiive`. https://pypi.org/project/mlrose-ky/

## License
Licensed under the [Unlicense](https://unlicense.org/).
