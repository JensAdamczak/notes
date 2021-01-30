---
title: "Hugo: posts and terms per taxonomy"
date: 2021-01-30T13:51:05+01:00
snippets: ['Hugo']
draft: false 
---

Counting the number of posts and different terms per taxonomy in Hugo requires looping through all
taxonomies.

```Go
{{ range $taxname, $tax := .Site.Taxonomies }}                                                        
    {{ $nposts := len (where $.Site.RegularPages (print "Params" "." $taxname) "ne" nil) }}
    {{ $nterms := len $tax }}
    {{ $posttext := cond (gt $nposts 1) "posts" "post" }}
    {{ $termtext := cond (gt $nterms 1) "terms" "term" }}
    {{ $taxname }}: {{ $nposts }} {{ $posttext }} and {{ $nterms }} search {{ $termtext }}.
    <br>                                                                                              
{{ end }}
```

