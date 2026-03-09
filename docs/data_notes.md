# Data Notes

## Data Construction Overview

The datasets used in this project were constructed from two main sources:

* learner sentences derived from **Lang-8**
* **synthetic learner-like sentences** generated from clean Wikipedia sentences

The goal was to obtain a dataset suitable for **sentence-level classification of learner error types**.

---

## Annotation Workflow

Learner sentences were processed in **annotation batches** and labeled manually according to the taxonomy described in:

```
docs/annotation_guidelines.md
```

For each learner sentence:

* exactly **one primary error label** was assigned
* optional fields such as `agreement_subtype` and `notes` were used to document secondary information
* ambiguous or unusable examples were flagged and removed during later cleaning stages

The annotation process involved **iterative manual inspection and correction**.

---

## Filtering and Data Cleaning

During dataset construction, some sentences were marked with the flag:

```
REPLACE
```

This indicates that the sentence should **not be used in the final dataset**.

Reasons for exclusion included:

* unclear learner intent
* annotation uncertainty
* unusable sentence structure
* noisy or corrupted learner input

These examples were removed during dataset cleaning.

---

## Manual Corrections and Iterative Updates

The annotation process involved several rounds of **manual corrections and patching**.

This included:

* updating previously annotated examples
* correcting inconsistent labels
* refining annotation decisions after reviewing batches of sentences

As a result, the data preparation process was **iterative and partly exploratory**.

---

## Reproducibility

The full data construction pipeline is **not provided as a fully reproducible script**.

Some steps were conducted through **manual annotation and exploratory notebooks**, which are not distributed as a clean pipeline in this repository.

Instead, the repository focuses on providing:

* the **final experimental setup**
* the **annotation guidelines**
* the **modeling and evaluation notebooks**

---

## Data Availability

Due to **licensing and annotation constraints**, the datasets used in this project are **not distributed in this repository**.

The repository therefore documents:

* the **structure of the expected datasets**
* the **annotation scheme**
* the **experimental pipeline**

---