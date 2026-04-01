
# Epistemic (Model) Uncertainty via Ensemble Models

- resource : https://youtu.be/Osju20L6Z3I

## Ensemble Approach

- Train multiple versions (e.g., five) of the same architecture with different random weight initializations.
- Each model learns the same classes but memorizes features differently.

## Measuring Uncertainty

- Pass a new image through all models and observe the **Softmax variance** across predictions.
- **Low variance** = models agree = low epistemic uncertainty.
- **High variance** = models disagree = high epistemic uncertainty (model does not know this input).

## Visualizing with a Probability Simplex

- A triangle where each **vertex** = 100% confidence in one class (e.g., Red, Green, Blue).
- **High-confidence** predictions plot near a vertex.
- **Uncertain** predictions move toward the center (equal probability across all classes).
- Plotting each ensemble member's prediction as a dot shows **model disagreement visually** — greater spread means greater uncertainty.
