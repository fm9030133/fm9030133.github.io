# Translative Synthetic Biology
I am synthetic biologist intending to bring emerging technologies to market. I specialize in modeling the flow of information in living tissue. This repository documents my project-based journey in developing such an expertise. I welcome inquiries for work and collaboration.  
  
# Bioelectricity
Living tissue realiably self-assemble into complex structures. Key goal-states of this massively parallel behavior are encoded by intercellular communication as patterned gradients of charge carriers. Growing understanding of this phenomenon is yielding an emerging layer of control to guide large-scale development of animals.  
I'm developing my expertise in this domain by reading and discussing academic publications and experimenting with computational simulations used in such resarch. I'm learning to use BETSE (BioElectric Tissue Simulation Engine), a Python-based ["simulator for 2D computational multiphysics problems in the life sciences – including electrodiffusion, electro-osmosis, galvanotaxis, voltage-gated ion channels, gene regulatory networks, and biochemical reaction networks \(e.g., metabolism\)."] (https://github.com/betsee/betse)  
  
# Process Visualization
Along with subject matter knowledge I am also refining key upstream skills such as planning and communication of complex processes. I use ["Mermaid, the JavaScript based diagramming and charting tool"](https://mermaid.js.org/) to create insightful process maps for projects. Below is the [process map for a recent college programming assignment.](flow.md)  
  
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
```
  
```mermaid
    flowchart LR
    subgraph Legend
    classDef default stroke-width:4px
    classDef str stroke:#ff0000
    classDef int stroke:#ffe100
    classDef list stroke:#30b500
    classDef tuple stroke:#022b9c
    classDef dict stroke:#de05f2

    str:::str
    int:::int
    list:::list
    tuple:::tuple
    dict:::dict
    end
```
  
# Medically Relevant Unconventional Computing
Neural and non-neural electrical activity. Immunology.

# Inspiration: Leaders and Ventures
Although I am grateful to the countless contributors to this field there are a handful of individuals whos work I follow closely. Similarly, there are a few startups that I am particularly interested in. Such focus allows for deeper expertise.  

# Professional Training
