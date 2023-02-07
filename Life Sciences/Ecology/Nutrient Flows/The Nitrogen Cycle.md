---
date: [Tue 20/09 2022]
aliases: [nitrogen cycle,  ]
tags: [GR10/Q3 Ecology/nutrient-cycles Ecology/biosphere ]
modified: Thu 03/11 2022 08:00
---
# The Nitrogen Cycle
Nitrogen is found in [[The Atmosphere]]. Nitrogen is necessary for all organisms – it is one of the essential components of [[Proteins|Amino Acids]]. However, no organism can absorb it directly from the [[The Atmosphere|atmosphere]]. 


```mermaid
flowchart TB

subgraph Earth-Flow
	nitrites -- Nitrification by \nNitrifying Bacteria--> nitrates("Nitrate Salts NO<sub>3</sub>")
	nitrates -- Absorption by Plants --> plants("Plant Protein")
	plants -- digestion by animals --> animals(Animal proteins)
	animals -- excretion --> urea("Urea") --> decomBac
  animals & plants -- death --> decomBac{{Decomposing Bacteria}}
  
  subgraph Ammonia-flow
	  ammonia(Ammonia) -- Nitrification by \nNitrifying Bacteria --> nitrites("Nitrites NO<sub>2</sub>")
        decomBac --> ammonia
	end
end

subgraph Atmosphere-Flow
	direction LR
	atmosphere --> lightning("Rain and Lightning") & nitrogenFix("Fixation by Nitrogen Fixing Bacteria")
	nitrates("Nitrate Salts NO<sub>3</sub>") --> denitrification{{"Denitrifying Bacteria"}} --> atmosphere
	lightning("Rain and Lightning") & nitrogenFix("Fixation by Nitrogen Fixing Bacteria") -- fixation --> nitrates
end
```

## How Nitrogen Is used
The N<sub>2(g)</sub> undergoes *Fixation*, either by rain and lightning or by *Nitrogen Fixing Bacteria*, which turns the N<sub>2(g)</sub> into *Nitrates (NO<sub>3</sub>)*, which can be found in the soil. 

### Nitrogen-Fixing Bacteria
Nitrogen fixing Bacteria are found in the soil as *free-living bacteria*. Some Nitrogen-fixing bacteria are found living mutualistically in the root nodules of leguminous plants (such as peas and beans). These absorb the Nitrogen gas and convert it into *Nitrates*. 

### Usage By Plants
Nitrates can be absorbed by *plants* through their [[Dicotyledonous plants#Dicotyledonous Roots|Roots]] and converted into [[proteins]]. When the plant dies, their organic matter is decomposed by *decomposing Bacteria* into *Ammonia (NH<sub>3</sub>)*

### Usage By Animals
Animals will eat plants, and the proteins will filter through the [[Energy Flow|trophic levels]] to all animals before either being *excreted as urea*, or *released when the animal dies* and is decomposed. The urea is decomposed by *decomposing Bacteria* into *Ammonia (NH<sub>3</sub>)*. When the animals dies, their organic matter is decomposed by *decomposing Bacteria* into *Ammonia (NH<sub>3</sub>)*

#### Ammonia To Nitrates
Ammonia (NH<sub>3</sub>) is broken into Nitrites (NO<sub>2</sub>) by *nitrifying bacteria*. NO<sub>2</sub> is then combined into Nitrites (NO<sub>3</sub>) by the same nitrifying bacteria. 

## Return of Nitrogen to the Atmosphere
*Ammonia (NH<sub>3</sub>)* can be broken into Nitrites (NO<sub>2</sub>), which can be made into Nitrates (NO<sub>3</sub>), which are then broken into N<sub>2(g)</sub> by *denitrifying bacteria* and re-released into the atmosphere. 


> [!info] Eutrophication and Fertilisers
>
>Fertilizers increase soil quality for plant growth, but may cause runoff water that leeches the nutrients from the soil. This water can then escape into waterbodies, which will experience an *algae bloom* due to the excessive nutrients. This is known as eutrophication.
>
>These algae will eventually cover the surface of the waterbody and use all the nutrients, leaving the water without any life or nutrients. This causes decomposition bacteria to increase in the water, using up more oxygen from the water, and killing off any remaining aquatic organisms that require this water. 
>
>This is why the excessive use of fertilisers and the dumping of waste into waterbodies is discouraged, as it can devastate the [[Ecosystems]] involved