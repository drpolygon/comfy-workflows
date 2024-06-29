# Comfy Workflows
This repo contains some of my sample workflows and data for how I generate images with comfyUI. I plan on supporting this repo and will develop it by adding more examples over time.

Use them however you like. I will admit there are likely better methods available to achieve what I am doing here, especially considering how fast things are moving!

I like to add notes to explain my thought process, and I am quite open to peer review - please feel free to provide feedback.

## The Workflows
- [**Regional Prompting**] (https://github.com/drpolygon/comfy-workflows/blob/main/regional_prompting.json) - SDXL - This workflow is a single-pass sampler that uses an RGB channel-packed mask for input. Each channel of the mask is used for prompt conditioning and attention-masking with its own ipAdapter. This workflow makes use of Perturbed Attention Guidance, and the AlignYourSteps sampler. You will need to install several additional custom nodes to get this to run - so if you get stuck with any of them, feel free to contact me. It is designed to be used with the dataset below.

## The Data
- [**Regional Prompting Input Data**] (https://github.com/drpolygon/comfy-workflows/tree/main/regional_prompting_input_data) This folder includes an array of channel packed masks, and sample data that gets used by the ipAdapters. Place all of this content in your comfyUI/input folder.
