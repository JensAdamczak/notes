---
title: "R: rank2score"
date: 2022-02-02T21:49:04-08:00
snippets: ['R']
draft: false 
---

Converting a ranking into a set of normally distributed scores.

```R
rank2score <- function(rank, n_total, mn = 0, std = 1, n_tied = 1) {
  # following the equal area method
  # http://node101.psych.cornell.edu/Darlington/transfrm.htm
  
  mean_rank <- rank / n_tied
  qnorm(mean_rank / (n_total + 1), mean = mn, sd = std)
}
```

