---
title: My Collection
---

# My Collection

This is my collection of art objects.

## Artists

- Vincent van Gogh
- Pablo Picasso
- Rembrandt van Rijn

## Query Examples

### Query 1: Paintings by Vincent van Gogh

```sparql
SELECT ?painting ?title
WHERE {
  ?painting wdt:P31 wd:Q3305213.
  ?painting wdt:P170 wd:Q5582.
  ?painting rdfs:label ?title.
  FILTER (lang(?title) = "en").
}
SELECT ?sculpture ?title
WHERE {
  ?sculpture wdt:P31 wd:Q860861.
  ?sculpture wdt:P170 wd:Q134307.
  ?sculpture rdfs:label ?title.
  FILTER (lang(?title) = "en").
}
SELECT ?etching ?title
WHERE {
  ?etching wdt:P31 wd:Q15304597.
  ?etching wdt:P170 wd:Q5599.
  ?etching rdfs:label ?title.
  FILTER (lang(?title) = "en").
}
