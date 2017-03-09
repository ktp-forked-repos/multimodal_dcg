# multimodal_dcg
Reduce floundering of DCGs by constraining and narrowing search 

```prolog

 :- pack_install('https://github.com/TeamSPoon/multimodal_dcg.git').

```


```prolog

:- use_module(library(multimodal_dcg)).


predicate_named(Pred) --> dcgAnd(theText(Text),dcgLenBetween(1,5)).

:- must(dcgAnd(dcgLenBetween(5,1),theText(_Text),[a,b,c],[])).
:- must(predicate_named(_P,[proper,-,named],[])).


```



# Some TODOs

Document this pack!
Write tests
Untangle the 'pack' install deps
Still in progress (Moving predicates over here from logicmoo_base)


[BSD 2-Clause License](LICENSE.md)

Copyright (c) 2017, 
Douglas Miles <logicmoo@gmail.com> and TeamSPoon
All rights reserved.

# Dislike having tons of forks that are several commits behind the main git repo?

(Why feel obligated to maintain a git fork just to contribute ?)

Please ask to be added to TeamSPoon !


