
# Annotation Guidelines

## Goal

For each learner sentence, assign **one primary error label** corresponding to the **most salient learner error** in the sentence.

Only **one label must be assigned per sentence**.

Optional fields:

* `agreement_subtype` (only when the main label is `agreement`)
* `notes` to document secondary errors or ambiguities

---

# Annotation Principles

### 1. Choose one primary error

Each sentence must receive **exactly one label**, corresponding to the **main learner error**.

If multiple errors appear:

* choose the **most linguistically central error**
* record additional issues in `notes`

Example:

```
Je suis content pour études commence
```

Primary label → `agreement`
Secondary issue → tense or lexical problems can be mentioned in `notes`.

---

### 2. Annotate the learner sentence as written

Annotate **the learner sentence itself**.

The correction is used **only to understand the intended meaning**, not to modify the sentence during annotation.

---

# Error Taxonomy (10 Labels)

## agreement

Incorrect **morphosyntactic agreement**.

This includes:

* gender agreement
* number agreement
* subject–verb agreement
* adjective agreement

Examples:

```
les personne arrive
il chantent
```

Additional field:

```
agreement_subtype
```

Possible values:

```
gender
number
subjverb
other
```

---

## verb_form

Incorrect **verb morphology** regardless of tense choice.

Examples:

```
il chantent
j’ai allé
```

Typical errors:

* wrong conjugation
* wrong auxiliary
* incorrect participle form
* incorrect inflection

---

## tense_mood_aspect

Incorrect **choice of tense, mood, or aspect**.

The verb form itself may be grammatically correct, but the **tense choice is inappropriate**.

Examples:

```
Hier je vais au marché
il faut que tu vas
```

---

## determiner_article

Incorrect or missing **determiners or articles**.

This includes:

* definite articles
* indefinite articles
* partitive articles
* possessives
* demonstratives
* quantifiers

Examples:

```
ma école
j’ai acheté pain
```

---

## preposition

Incorrect **preposition choice**, missing preposition, or unnecessary preposition.

Examples:

```
aller à France
émue à une nouvelle
```

These often reflect **selection errors** between verbs and prepositions.

---

## pronoun_clitic

Incorrect **clitic pronoun form** or **placement**.

This includes:

* object pronouns (`le`, `la`, `les`, `lui`, `leur`)
* `y`
* `en`

Examples:

```
je donne lui le livre
je le donne lui
```

---

## lexical_choice

Incorrect **word choice** or **collocation**.

The word is grammatically possible but **lexically inappropriate**.

Examples:

```
aucun doute monétaire
faire une promenade sportive forte
```

These often involve incorrect collocations or literal translations.

---

## word_order

Incorrect **word order** or constituent placement.

Examples:

```
Je ne pense seulement pas
pas avant je suis venu
```

---

## negation

Incorrect **negation structure**.

Examples:

```
je ne pense seulement
je pense pas seulement
```

---

## spelling_orthography

Orthographic or spelling errors.

Examples:

```
quelque choses
interresant
```

This includes:

* spelling mistakes
* missing accents
* incorrect word forms due to orthography

---

# Handling Multiple Errors

Learner sentences often contain **multiple errors**.

Annotation rule:

1. Assign **one primary label**
2. Record other errors in `notes`

Example annotation:

```
label: agreement
agreement_subtype: number
notes: possible determiner error
```

---

# Annotation Philosophy

The goal of the annotation is to capture **the most linguistically informative error type**, even when several issues appear in the sentence.

The taxonomy prioritizes:

* grammatical structure
* lexical selection
* morphosyntactic agreement
* functional word usage


