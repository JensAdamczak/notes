---
title: "Old post about R"
date: 2019-01-17T11:27:56+01:00
draft: false 
snippets: ['R']
---

Let's write some code snippet here for future reference.

``` R
calc_conf_interval <- function(p, n) {
  ci_var <- p * (1 - p)
  ci_high <- p + 1.96 * sqrt(ci_var / n)
  ci_low  <- p - 1.96 * sqrt(ci_var / n)
  
  list(ci_low = ci_low, ci_high = ci_high)
}

ctr_high = calc_conf_interval(ctr, n)$ci_high
```
