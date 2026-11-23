# RAG vs ERIE Demo

One chat input sent to both RAG and ERIE, with an inspection terminal to compare their outputs.

The corpus is Mary Shelley's Frankenstein (1818, Project Gutenberg 41445), held in the record as 27 entries, KIDs 1 to 27, each at trust 8.

- **RAG** shows the soup: similarity-ranked novel chunks with scores, the raw soup prompt it builds, and its answer with a soup-check warning.
- **ERIE** shows the ingredients and the recipe: record entries with KID, birth stamp, source chapter, and trust 8/MATURE, the ingredients-plus-recipe prompt, and a cited answer.
- **The inspection terminal** logs both pipelines step by step.
- **The record browser** shows all 27 record entries.

Preset questions cover who created the creature, the wedding night, Justine Moritz, and the creature's demand. There is a trap question, the name of Victor's dog: the novel has no dog and the record has no entry for one. ERIE says it does not know. RAG confabulates a dog from noise.

## Run it

Open `index.html` in a browser. It is a single self-contained file, no build step, no server needed.

## The paper

This demo accompanies the RAG vs ERIE paper: RAG gives the model soup and asks it to make a sandwich; ERIE gives the model the ingredients and the recipe. The paper draft is being written alongside the demo.

## Live demo

https://muse.ai/s/rag-vs-erie-demo-xao6yxixdrx0zjxa/BEPuqfOLbz1dJlx-w4dIEyua0nC1sBNOX_K4P--HSeM
