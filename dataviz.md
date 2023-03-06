I use tools such as [Mermaid.js](https://mermaid.js.org/), [Lucidchart](https://www.lucidchart.com/), and [Biorender](https://www.biorender.com/) to create insightful, vizually appealing process maps and scientific illustrations.

-----------
[College Python programming assignment, flowchart, Mermaid.js](flow.md)    
```mermaid
---
title: n_grams.py
---
flowchart LR
    subgraph "n_grams()"
    classDef default stroke-width:4px
    classDef str stroke:#ff0000
    classDef int stroke:#ffe100
    classDef list stroke:#30b500
    classDef tuple stroke:#022b9c
    classDef dict stroke:#de05f2

    %% This is a comment

    text:::str
    n_gram_len:::int
    min_count:::int
    text -- ".split()" --> word_list:::list
    word_list -- ".lower().strip()" --> word_tup:::tuple
    n_gram_len --> tup_list:::list
    word_tup --> tup_list
    tup_list --> dict_full:::dict
    min_count --> dict_full
    tup_list --> ngram_counts:::list
    min_count --> ngram_counts
    ngram_counts --> list_dict:::dict
    dict_full -- ".append(tup)" --> list_dict
    dict_full -- ".sort()" --> list_dict
    list_dict --> return
    end

    subgraph "most_frequent_n_grams()"
    %%text_mf:::str -- "n_grams()" --> n_grams_dict:::dict
    text_mf:::str --> text
    min_len:::int -- "loop min" --> for-loop(("for-loop"))
    max_len:::int -- "loop max" --> for-loop
    limit:::int
    return --> for-loop
    for-loop --> n_grams_dict:::dict
    %%for-loop <--> text_mf
    %%return --> text_mf
    end
    
    subgraph Legend
    str:::str
    int:::int
    list:::list
    tuple:::tuple
    dict:::dict
    end
```
