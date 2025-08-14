# Human-vs-AI
Dataset and code for analyzing human-written and AI-generated image descriptions in Romanian and English. Includes CLIP similarity scores, lexical metrics, and classification scripts for distinguishing human vs AI captions.


**dataset.csv** file containing paired human-written and AI-generated image descriptions in Romanian and English.
	Columns:
 
	• image_id – file names of images from the publicly available T4SA dataset (accessible online).
 
	• human_english – human-written description in English.
 
	• human_romanian – human-written description in Romanian.
 
	• AI_english – AI-generated description in English (BLIP-2).
 
	• AI_romanian – AI-generated description in Romanian (translated from AI_english using MarianMT).

**clip_scores.py** computes semantic similarity scores between images and captions using the OpenAI CLIP model.

	• Loads captions from dataset.csv (human/AI, English/Romanian).

	• Searches for corresponding images (by image_id) in a local directory.

	• Computes raw CLIP scores, applies min–max normalization, and labels each pair as matching or not_matching (threshold = 0.5).

	• Saves results and logs missing images for review.
