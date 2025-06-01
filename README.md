# Exno.10-Content Creation (Reports, Articles, Case Studies, etc.) Using Prompt Patterns
## DATE: 28/04/2025
# Aim: 
To perform Content Creation (Reports, Articles, Case Studies, etc.) Using Prompt Patterns

# Algorithm: 
Design and implement Python-based applications that:

1. Accept user input as a prompt.

2. Interact with AI models (ChatGPT for task management and content generation, audio-focused models for sound generation, and video generation models).

3. Receive responses with task suggestions, generated audio, video content, or textual content.

4. Store, organize, and optionally download outputs.

5. Demonstrate progression from simple to advanced prompts.

# Objective:

## Build ChatGPT-powered assistant that:

a. Organizes user-input daily tasks.
b. Evolves with progressively advanced prompt engineering.
c. Outputs categorized, prioritized, and optimized to-do lists.
d. Logs data for reuse and review.

## Build an AI audio content generator that:

a. Accepts user prompts for music, narration, or effects.
b. Interfaces with audio generation APIs.
c. Saves or plays audio.

## Build an AI video generation pipeline that:

a. Accepts textual prompts and creates visual stories or clips.
b. Demonstrates effect of prompt detail on output quality.
c. Interfaces with APIs such as RunwayML or Pika Labs.

## Build a content generation workflow using prompt engineering that:

a. Demonstrates different prompting techniques (query decomposition, semantic structuring).
b. Generates structured outputs like reports, articles, or case studies.
c. Explores creativity by generating comic strips or narratives.
d. Evaluates the impact of prompt precision on coherence and relevance.

## Steps for Content Generation via Prompting Techniques – Using ChatGPT

## Step 1: Simple Content Prompting
```py
simple_prompt = "Write a short article about the importance of daily exercise."
response = ask_chatgpt(simple_prompt)
print("\nSimple Article:\n", response)
```
## Step 2: Query Decomposition Technique
Break the task into sub-prompts for structure:
```py
prompt_intro = "Write an introduction about the significance of daily exercise."
prompt_body = "Explain the physical and mental benefits of exercising regularly."
prompt_conclusion = "Write a conclusion summarizing why one should adopt daily exercise."

response_intro = ask_chatgpt(prompt_intro)
response_body = ask_chatgpt(prompt_body)
response_conclusion = ask_chatgpt(prompt_conclusion)

final_article = f"{response_intro}\n\n{response_body}\n\n{response_conclusion}"
print("\nStructured Article:\n", final_article)
```
## Step 3: Decision-Making & Filtering Prompts
Ask the model to make structured decisions and filter data:
```py
decision_prompt = (
    "You are writing an article about the best exercises for busy people. Choose top 3 based on time efficiency, impact, and accessibility."
)
response = ask_chatgpt(decision_prompt)
print("\nDecision-based Output:\n", response)
```
## Step 4: Creative Work (Comic Storyline Prompt)
```py
creative_prompt = (
    "Create a short comic strip script with 4 panels about a robot who learns to cook pasta."
)
response = ask_chatgpt(creative_prompt)
print("\nComic Strip Script:\n", response)
```
## Step 5: Semantic Filtering and Tone Adjustments
```py
tone_prompt = (
    "Rewrite the following paragraph in a humorous tone: 'Waking up early is good for productivity, but hard to do.'"
)
response = ask_chatgpt(tone_prompt)
print("\nHumorous Version:\n", response)
```
# Result:

The application successfully demonstrates:

Task organization with ChatGPT.

Audio narration generation using advanced prompting.

Video generation showing differences in prompt quality.

Structured and creative content generation using varied prompting techniques.

# Conclusion:
This experiment shows how various prompting techniques can be effectively used to build AI-powered applications. In this case:

ChatGPT helps structure daily life with natural prompts.

Audio APIs bring those prompts to life through narration or sound design.

Video models generate visuals based on the level of descriptive prompting.

Content generation becomes more controlled and creative with prompt decomposition, tone guidance, and filtering.

The approach is scalable to full creative workflows like audiobooks, explainer videos, or task automation.

