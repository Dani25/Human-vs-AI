# Human-vs-AI
Dataset and code for analyzing human-written and AI-generated image descriptions in Romanian and English. Includes CLIP similarity scores, lexical metrics, and classification scripts for distinguishing human vs AI captions.
#------------------------------------
dataset.CSV file containing paired human-written and AI-generated image descriptions in Romanian and English.
Columns:
• image_id – file names of images from the publicly available T4SA dataset (accessible online).
• human_english – human-written description in English.
• human_romanian – human-written description in Romanian.
• AI_english – AI-generated description in English (BLIP-2).
• AI_romanian – AI-generated description in Romanian (translated from AI_english using MarianMT).
#------------------------------------
