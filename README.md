# Framing the End of the World. Analysis of the screenplay of "Don't Look Up"


### A computational linguistic analysis of language structures

This project analyzes the screenplay of Adam McKay's film *Don't Look Up* using **Natural Language Processing (NLP)** methods. The objective is to empirically demonstrate that the communicative failure depicted in the film is not merely a plot device, but a structural inevitability.

By operationalizing sociological theories (Schütz, Lakoff) into measurable data vectors, the analysis proves that the catastrophe is caused not by a lack of knowledge, but by disjointed "finite provinces of meaning" and a lack of semantic intersection.

---

## Theoretical Framework

The data analysis relies on two theoretical pillars:

1. **Alfred Schütz (Phenomenological Sociology):** The theory of *Finite Provinces of Meaning*. The characters inhabit separated realities (Science vs. Media/Politics) between which no translation is possible.
2. **George Lakoff (Cognitive Linguistics):** Theories of *Framing* and *Hypocognition*. The study investigates how threats ("Comet") are linguistically reframed into market opportunities ("Assets") and why society lacks the cognitive frames to grasp "The End" (Hypocognition).

---

## Methodology & Tech Stack

The approach follows the principle of **"Computational Distant Reading"**.

* **Language:** Python 3.x
* **Libraries:** `spaCy`, `scikit-learn`, `pandas`, `matplotlib`, `seaborn`, `nltk`, `wordcloud`
* **Model:** `en_core_web_md` (utilizing 300-dimensional Word Embeddings)

### Pipeline

1. **Parsing:** Extraction of dialogue from the raw screenplay & cleaning (removal of stage directions).
2. **Clustering:** Aggregation of characters into 4 sociological archetypes:
* 1. **SCIENCE** (Dr. Mindy, Dr. Oglethorpe)
* 2. **ACTIVISM** (Kate Dibiasky)
* 3. **POPULISM** (President Orlean)
* 4. **CAPITALISM** (Peter Isherwell)


3. **Analysis:**
* *Vector Space Analysis:* Calculation of **Cosine Similarity** between worldviews.
* *Frequency Analysis:* Deterministic evaluation of keywords (Dictionary Approach).
* *Framing Analysis:* Visualization of semantic orientation via Radar Charts.



---

## Key Findings

### 1. The Semantic Rift (Heatmap)

Vector space analysis reveals that **Science** and **Activism**—though natural allies—share a semantic similarity of only **0.40**. They utilize incompatible codes (Rationality vs. Morality). Simultaneously, Science exhibits a dangerous proximity to Capitalism (**0.63**), explaining its vulnerability to technocratic co-optation.


### 2. The Geometry of Reframing (Radar Chart)

Peter Isherwell (Capitalism) displays extreme "semantic monomania." His vocabulary almost entirely ignores the dimensions of "Panic" and "Politics," maximizing the "Profit" vector instead. This visually demonstrates the successful reframing of the catastrophe into a resource.


### 3. Divergent Relevance Structures (Bar Charts)

While scientists focus on the **Object** (Comet), politicians fixate on the **Subject** (Voters/Crowd). There is no intersection in their relevance structures. Furthermore, the analysis shows that terms like "Death" appear in the Capitalist cluster but are technocratically redefined (as "Evolution" or "Algorithm").

---

## Installation & Usage

1. **Clone Repository:**
```bash
git clone https://github.com/peter2b/dont_look_up

```



```bash
pip install spacy pandas matplotlib seaborn nltk scikit-learn wordcloud

```


3. **Download SpaCy Model:**
The medium-sized model is required for vector calculations:
```bash
python -m spacy download en_core_web_md

```


4. **Run Analysis:**
Execute the Jupyter Notebook or the script:
```bash
jupyter notebook Frame_Analysis_DONT_LOOK_UP_fin.ipynb

```



---

## License & Credits

Based on the original screenplay by Adam McKay.
Analysis created for the seminar Inter-American Environmental Studies 25W 975.036  at University of Graz.

**Author:** Peter Bauer
**Date:** 15.2.2026
