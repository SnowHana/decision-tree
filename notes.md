# 1. Gini Index

- Gini Index = Name of the _cost function_ used to evaluate splits in dataset.
- **Split** = 1 input attr. + 1 value for that attr.
- Perfect separation => Gini score of 0
- Worst case => 50/50 , Gini score of 0.5

## Calculating Gini Score

```
proportion = count(class_value) / count(rows)
```

```
gini_index = sum(proportion * (1.0 - proportion))
gini_index = 1.0 - sum(proportion * proportion)
```

- Gini index for each group must then be weighted by the size of the group, relative to all samples that are currently being grouped.

```
gini_index = (1.0 - sum(proportion * proportion)) * (group_size/total_samples)
```
