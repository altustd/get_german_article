# German Article Determiner (der, die, das)

A simple Python function to predict the German definite article (`der`, `die`, or `das`) for a given noun using common linguistic patterns and suffix rules.

## Why?
German noun genders are notoriously difficult for learners because they often seem arbitrary. However, there are strong statistical patterns based on word endings that allow correct prediction in ~80-90% of cases for common nouns. This script implements many of those reliable rules.

**Note**: This is not a dictionary lookup and will never be 100% accurate. For production or full accuracy, consider using a dictionary-based library like [`german-nouns`](https://pypi.org/project/german-nouns/) which contains ~100,000 nouns with exact genders.

This rule-based version is lightweight, has no dependencies, and works offline.

## Installation
No installation needed! Just copy the `get_german_article` function into your project.

## Usage 

```python

print(get_german_article('Haus'))        # Output: das
print(get_german_article('Frau'))        # Output: die
print(get_german_article('Computer'))    # Output: der
print(get_german_article('Mädchen'))     # Output: das
