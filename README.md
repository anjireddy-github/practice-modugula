# Anji Reddy Modugula

## My Favorite Television Show: Breaking Bad

I love **Breaking Bad** because of its **intense storytelling** and complex characters. The show masterfully blends suspense, drama, and moral dilemmas, making every episode captivating. The transformation of Walter White from a humble teacher to a notorious figure is both shocking and fascinating.

---

### Favorite Actors (Most Favorite to Least in This List)
1. Bryan Cranston
2. Aaron Paul
3. Giancarlo Esposito
4. Anna Gunn (honorable mention)

Other Shows I Enjoy:
- Better Call Saul
- Stranger Things
- The Crown
- Dark

---

Explore more: Read about my favorite outdoor activity: [Hiking Activity & Why I Love It](./MyActivity.md)

---

## People I'd Like to Meet

Throughout history (and across disciplines), a few remarkable individuals stand out for their vision, resilience, creativity, and impact on humanity. Below is a curated list of four such people I’d love to have a conversation with—whether to explore scientific curiosity, leadership through adversity, or the birth of entirely new fields of thought.

| Name | Reason | Birth Date | Date of Death |
|------|--------|------------|---------------|
| Marie Curie | Trailblazing physicist and chemist; perseverance in advancing science under adversity; only person to win Nobel Prizes in two scientific fields. | Nov 7, 1867 | Jul 4, 1934 |
| Leonardo da Vinci | Quintessential polymath whose curiosity spanned art, anatomy, engineering, and invention—embodies boundless interdisciplinary creativity. | Apr 15, 1452 | May 2, 1519 |
| Nelson Mandela | Symbol of reconciliation and moral leadership; insights on justice, forgiveness, and building inclusive societies. | Jul 18, 1918 | Dec 5, 2013 |
| Ada Lovelace | Early visionary of computing; foresaw machines doing more than calculation—foundation for modern computer science imagination. | Dec 10, 1815 | Nov 27, 1852 |

---

## Favorite Quotes

> "Somewhere, something incredible is waiting to be known."  
> *Carl Sagan*

> "Imagination is more important than knowledge. For knowledge is limited, whereas imagination embraces the entire world."  
> *Albert Einstein*

---

## Code Fencing

Below is a short Python utility function that returns the 10 most common words in a text file. It demonstrates clean use of a context manager for safe file handling and the `Counter` collection for efficient frequency counting.

```python
from collections import Counter

def top_word_frequencies(path: str, top_n: int = 10):
	"""Return a list of (word, count) tuples for the most common words in the file.

	Words are normalized to lowercase and split on whitespace. Punctuation handling
	is minimal for simplicity; extend with regex tokenization if needed.
	"""
	counts = Counter()
	with open(path, 'r', encoding='utf-8') as f:  # context manager ensures file closes
		for line in f:
			for token in line.strip().split():
				counts[token.lower()] += 1
	return counts.most_common(top_n)

if __name__ == "__main__":
	# Example usage (uncomment and adjust the filename to test):
	# print(top_word_frequencies("example.txt"))
	pass
```

Quick links: [with statement docs](https://docs.python.org/3/reference/compound_stmts.html#the-with-statement) | [collections.Counter](https://docs.python.org/3/library/collections.html#collections.Counter)


