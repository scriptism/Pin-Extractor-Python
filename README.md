# Scriptism – Simple

# PinExtractor

A tiny utility that turns short poems into numeric secret codes.

## How it works

1. Split each poem into lines.
2. For every line, pick the word whose index matches the line number (0-based).
3. Append the length of that word to the code string; if the line has too few words, append `0`.
4. Return the list of codes for all supplied poems.

## Function

```python
def pin_extractor(poems):
    ...

poem = """Stars and the moon
shine in the sky
white and
until the end of the night"""

print(pin_extractor([poem]))
# -> ['4550']

## How to run the app?

```bash
python main.py
```
