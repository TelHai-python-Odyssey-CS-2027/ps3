# PS3 — Edge cases and approximating π

Two short exercises on lists and loops.

## What to change

Edit these two files only:

### 1. `edge_case_exercise.py` — `move(my_list, direction)`

`my_list` is zeros with a single `1`. Move the `1` `"left"` or `"right"`. If the move would leave the list, leave the `1` in place.

```python
move([0, 0, 0, 1, 0], "right")  # [0, 0, 0, 0, 1]
move([1, 0, 0, 0, 0], "left")   # [1, 0, 0, 0, 0]
```

### 2. `leibniz_series_exercise.py` — `approximate_pi(n_terms)`

Approximate π with the first `n_terms` of the Leibniz series:

$$\pi = 4 \sum_{n=0}^{\infty} \frac{(-1)^n}{2n+1}$$

## Practice in Colab (optional)

**From GitHub:** use **Ctrl+click** / **⌘+click** (or middle-click) so Colab opens in a new tab — GitHub ignores `target=_blank` on README links.

- <a href="https://colab.research.google.com/github/TelHai-python-Odyssey-CS-2027/ps3/blob/main/edge_case_exercise.ipynb" target="_blank" rel="noopener noreferrer">Edge cases notebook</a>
- <a href="https://colab.research.google.com/github/TelHai-python-Odyssey-CS-2027/ps3/blob/main/leibniz_series_exercise.ipynb" target="_blank" rel="noopener noreferrer">Leibniz notebook</a>

Notebooks are not graded — only the `.py` files count. Each notebook ends with a **self-check** cell that runs the same cases as the autograder (expected / got / hint) — run it before copying your code into the `.py` file.

## Submit

1. Accept the Classroom 50 assignment.
2. Edit the two `.py` files, then **Commit changes**.
3. Check the latest autograding run for your score.

## Grading — 10 points

Points are split across cases; a failing case shows the exact input, expected value, your value, and a hint in the autograding **Details**.

| Check | Points |
| --- | ---: |
| `move` — 1 in the middle | 1 |
| `move` — 1 at the left edge, move left | 1 |
| `move` — 1 at the right edge, move right | 1 |
| `move` — 1 at an edge, move inward | 1 |
| `move` — single-element list | 1 |
| `approximate_pi` — `n = 1`, `5`, `99`, `999` | 1 each |
| `approximate_pi` — `n = 100000` is close to `math.pi` | 1 |
