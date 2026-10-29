# LLM-Guided-GA
![LLM_GA(3)](https://user-images.githubusercontent.com/81431282/233686394-0a5158af-6733-494d-812a-abe9bc607ab2.png)

Project made by Benjamin Weiser, Jérôme Genzling, Nicolas Gastellu, Sylvester Zhang, Tao Liu and Alexander Alexander Al-Feghali, Department of Chemistry, McGill University, Montreal, Quebec; Canada

Part of McGill ChemAI submission to the first LLM Hackaton for Chemistry.

The goal of this work was to investigate the ability for a Language Learning Model (LLM) to work in parallel with genetic algorithms (GA) for molecular property optimization

This work explores the potential of LLMs to improve molecular fragmentation, mutation, variation, and reproduction processes and the ability of a LLM to gather information from a SMILES string and an associated score to produce new SMILES strings

We used GPT-3.5-Turbo as our Main LLM model for this work. To try our model, you can use our Jupyter Notebook LLM-Guided-GA.ipynb attached in this GitHub project. To make it work, you will need your own OpenAI API key (see below). **No key is included in this repository.**

## Setting up your OpenAI API key

You can create a key from your [OpenAI account](https://platform.openai.com/api-keys).
**Running locally**

1. Install the dependency that loads the key: `pip install python-dotenv`
2. Copy the template and add your key:
   ```bash
   cp .env.example .env
   ```
   then edit `.env` so that it reads `OPENAI_API_KEY=<your key>`.
3. Launch the notebook from the repository folder. The first cell reads the key from `.env` (or from an `OPENAI_API_KEY` environment variable if you prefer to set it in your shell).

`.env` is listed in `.gitignore`, so your key won't be committed. Never share it or paste it into the notebook source.

**Running on Google Colab**

There is no `.env` file on Colab: just run the first cell and paste your key when prompted. It is not stored in the notebook. Clear cell outputs before saving or sharing a copy of the notebook.


The LLM model used can be changed in the genLLM_ functions (more precisely in the OpenAi functions) accordingly to the OpenAI API documentation. 

You can learn more about this project in our related paper : https://pubs.rsc.org/dd/article/2/5/1233/804912/14-examples-of-how-LLMs-can-transform-materials

ipynb file in files. Contains GA as well as LLM implementation.

Link to collab: https://colab.research.google.com/drive/1CRTSHzjja-GZ21v_0l-pWCHyZwgzspDj?usp=sharing
