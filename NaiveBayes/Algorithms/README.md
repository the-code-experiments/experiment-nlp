# Naive Bayes

Bayes rules:
```
p(y|x) [Posterior] = p(x|y) [Likelihood] p(y) [Prior] / p(x) [Evidence]

Eg:
p(x|y) = probability of seeing word "hello" if spam = 90%
p(y) = probability that any email is spam = 40%
```

How do we calculate these probabilities?
```
p(y=spam) = #spam emails / #total emails
p(y=not spam) = #not spam emails / #total emails
```

Choose a likelihood distribution that's appropriate for the feature vectors:
E.g.
* real-valued / bell-curve -> Gaussian
* counts -> Multinomial
* binary -> Bernoulli

> All are available in sklearn