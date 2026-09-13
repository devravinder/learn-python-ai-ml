# Overfitting and Underfitting

These are two common problems in Machine Learning where the model does not learn properly.

```text
Underfitting  → Model learns too little
Good fit      → Model learns the right amount
Overfitting   → Model learns too much
```

## Underfitting

`Underfitting` → The model is too simple and cannot learn the important patterns in the training data.

Example:

```text
Training data
     ↓
Simple model
     ↓
Doesn't learn enough
     ↓
Poor predictions
```

### Example

Suppose we want to predict house prices.

The actual relationship might be:

```text
House size + location + bedrooms
            ↓
       House price
```

But our model uses only:

```text
House size
    ↓
Price
```

The model is too simple and misses important patterns.

### Signs of Underfitting

Usually:

```text
Training accuracy → Low
Testing accuracy  → Low
```

### Causes

- Model is too simple
- Too few features
- Too little training
- Excessive regularization

### How to fix

- Use a more complex model
- Add useful features
- Reduce excessive regularization
- Train the model better

---

## Overfitting

`Overfitting` → The model learns the training data too closely, including noise and unnecessary patterns.

Example:

```text
Training data
     ↓
Very complex model
     ↓
Memorizes training data
     ↓
Poor performance on new data
```

Suppose we have:

```text
Training data → 95% accuracy
Testing data  → 70% accuracy
```

The model performs very well on training data but poorly on unseen data.

This is a typical sign of `overfitting`.

### Signs of Overfitting

Usually:

```text
Training accuracy → Very high
Testing accuracy  → Much lower
```

### Causes Of Overfitting

- Model is too complex
- Too many unnecessary features
- Too little training data
- Model learns noise
- Training for too long in some models

### How to fix Overfitting

- Use a simpler model
- Remove unnecessary features
- Get more training data
- Use regularization
- Use cross-validation
- Use techniques such as dropout for neural networks

---

## Simple Example

Imagine you are preparing for an exam.

### Underfitting Example

You study only a few topics:

```text
Study very little
      ↓
Don't understand enough
      ↓
Poor performance
```

### Overfitting Example

You memorize the exact questions from previous exams:

```text
Memorize previous questions
          ↓
Previous questions → Excellent
New questions      → Poor
```

### Good Fit

You understand the concepts:

```text
Understand concepts
       ↓
Can solve familiar and new questions
       ↓
Good performance
```

---

## Comparison

```text
                    Underfitting       Good Fit       Overfitting

Model complexity       Low               Right            High

Training accuracy      Low               High             Very High

Testing accuracy       Low               High             Low

Learning               Too little        Appropriate      Too much

Problem                Too simple        Good model       Memorization
```

## Easy way to remember

```text
Underfitting → Model didn't learn enough.

Overfitting  → Model learned too much from training data.

Good fit     → Model learned the important patterns and
               works well on new/unseen data.
```

## Most important point

The goal of Machine Learning is `not` to get the highest training accuracy.

The goal is to build a model that performs well on `unseen data`.

```text
Training Data
     ↓
    Model
     ↓
Unseen/Test Data
     ↓
Good predictions
```
