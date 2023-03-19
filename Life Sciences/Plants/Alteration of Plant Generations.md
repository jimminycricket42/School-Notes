---
aliases: [ ]
tags: [GR11/Q1]
created: Wed 08/03 2023
---
# Alteration of Plant Generations
Two definitive generations arise within plants: The Gametophyte and the Sporophyte generation. The Gamotophyte is a *sexual* generation that produces *gametes* [^1]. The sporophyte is an *asexual* generation which produces *spores* [^1]. ^blurb

[^1]: [[Reproduction]]

The two generations alternate, with one generation giving rise to the other.

```mermaid
flowchart TB
gam([Gametophyte])
spor([Sporophyte])
mal("Male ♀ Gamete")
fem("Female ♂ Gamete")
zyg{{Zygote}}
spores{{Spores}}

subgraph Haploid 
direction LR
	gam --> mal & fem
	
end


subgraph Diploid
mal & fem --> zyg
spor --> spores
spores --> gam
zyg --> spor
end
```

