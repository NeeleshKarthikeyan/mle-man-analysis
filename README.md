# SPC4004 Assessment 3: Use of *man* in the London English Corpus

This repository contains the dataset, classified sample, and supporting materials for my SPC4004 Assessment 3 project: **Analyzing Natural Language Data**.

## Project overview

This project investigates how the word *man* is used in a sample from the London English Corpus. The main research question is:

> To what extent does *man* function pragmatically, as an interactional feature that helps manage emphasis, stance, and conversation flow, rather than referentially, as a reference to a person?

The analysis focuses on whether *man* is mainly used to refer to a person, or whether it functions more broadly as a conversational/pragmatic marker in spoken London English.

## Dataset

The original dataset used for this project is the **man-sentences dataset**, extracted from the London English Corpus and provided via QMPlus for SPC4004 Assessment 3.

A cleaned sample of 100 sentences was constructed from the original dataset. The sample focused on cases where *man* appeared as a separate word, while avoiding duplicate sentences and plural-only examples such as *men*.

## Classification categories

Each sentence was classified according to the function of *man*.

The detailed categories were:

| Category | Description |
|---|---|
| Literal person reference | *man* refers to a specific adult male person |
| Generic person reference | *man* refers to a person or people generally |
| Vocative/address | *man* directly addresses the listener or another person |
| Discourse marker | *man* adds emphasis, stance, agreement, frustration, solidarity, or conversational rhythm |
| Fixed expression/compound | *man* appears as part of a fixed phrase or compound expression |

These were then grouped into broader labels:

| Broad label | Included categories |
|---|---|
| Referential | Literal person reference, generic person reference |
| Pragmatic/interactional | Vocative/address, discourse marker |
| Other | Fixed expression/compound |

## AI use

Two AI tools were used transparently during the project.

ChatGPT was used to assist with constructing the 100-sentence sample by identifying examples where *man* appeared as a separate word and avoiding duplicate sentences.

Gemini 3.5 Flash was used for the initial linguistic classification. Gemini was prompted to classify each sentence by detailed category, broad label, reason, and confidence rating. Each classification was then manually checked, with particular attention to medium-confidence cases.

The exact Gemini prompt is included in the report appendix.

## Results summary

The final classification found:

| Broad label | Count |
|---|---:|
| Pragmatic/interactional | 63 |
| Referential | 33 |
| Other | 4 |

The results suggest that *man* was used more often pragmatically than referentially in this 100-sentence sample. The most common use was as a discourse marker, where *man* helped manage emphasis, stance, or conversational rhythm.

## Limitations

This is an exploratory analysis based on a small sample of 100 sentences. The findings should not be treated as representative of the entire London English Corpus. Some sentences were short or fragmentary, meaning the function of man was sometimes difficult to classify confidently without wider conversational context.

## Repository structure

```text
mle-man-analysis/
│
├── README.md
├── data/
│   ├── man-sentences.csv
│   └── cleaned_man_sentences.csv
