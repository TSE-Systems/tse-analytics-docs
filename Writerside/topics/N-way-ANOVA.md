 # N-way ANOVA

N-way ANOVA can be used to determine the effects of two or more (between-subject) factors and their interactions on a (dependent) variable. 

![Figure: N-way ANOVA](N-way ANOVA.png)

To perform N-way ANOVA (Two-way ANOVA, Three-way ANOVA, Four-way ANOVA, …) in TSE Analytics, select the respective data set from the *Add widget* and choose **N-way ANOVA** as the analysis **Mode** in the AN(C)OVA control panel.
Select two or more factors from the **Factors** list and choose a variable from the **Dependent Variable** list.
If needed, select a **P-values adjustment** method or adjust the **Effect size type** via the dropdown menu.
Click **Update** to calculate results and apply changes in the analysis settings.

Analysis result tables for N-way ANOVA include:

![Figure: Two-way ANOVA analysis results table](Two-way ANOVA analysis results table.png)

**N-way ANOVA** (Two-way ANOVA, Three-way ANOVA, …):

- Source: Factor names or interactions
- SS: Sums of squares
- DF: Degrees of freedom
- MS: Mean squares
- F: F-values
- p-unc: uncorrected p-values
- np2: Partial eta-square effect sizes

![Figure: Pairwise post-hoc tests table](Pairwise post-hoc tests table.png)

**Pairwise post-hoc tests** (only for two-way ANOVA):

- Contrast: Factor (= independent variable) or interaction
- A: Name of first measurement
- B: Name of second measurement
- mean(A): Mean of the first measurement
- std(A): Standard deviation of the first measurement
- mean(B): Mean of the second measurement
- std(B): Standard deviation of the second factor group
- Paired: Indicates whether the two measurements are paired or independent
- Parametric: Indicates if parametric tests were used
- T: T statistic
- dof: Degrees of freedom (only if parametric=True)
- alternative: Tail of the test
- p-unc: Uncorrected p-values
- p-corr: Corrected p-values
- p-adjust: p-values correction method
- BF10: Bayes Factor
- effect size type: Effect size as defined in “Effect size type” dropdown menu

> **Note**: N-way ANOVA is only performed if at least one animal is assigned to each possible combination of groups.
>
> Pairwise comparisons for N-way ANOVA are only performed for two factors (Two-way ANOVA).
> The pairwise comparisons table is not displayed for N-way ANOVA with more than two factors (Three-way ANOVA, Four-way ANOVA, …)
>
> Pairwise comparisons for two-way ANOVA are only performed within the factor which is listed first in the Factors list.
> The order of factors can be reversed by clicking on ‘Name’ in the header of the factors list.
{style='note'}

## Example Interpretation

In this example, RER was selected as the dependent variable and analyzed using a Two-way ANOVA with the following two factors:

- Genotype: WT / KO

- Treatment: Control / Treated

![Figure: Example of Two-way ANOVA](Example of N-way ANOVA.png)

**1.** The first table summarizes the **Two-way ANOVA**table includes the F-values and corresponding p-values for each effect:

- **Genotype main effect**: not significant (**p = 0.725**): WT and KO animals show no meaningful difference in RER.

- **Treatment main effect**: not significant (**p = 0.808**): Control and Treated groups have similar RER values.

- **Genotype × Treatment interaction**: not significant (**p = 0.228**):The treatment effect does not differ between WT and KO animals.

All p-values are well above the 0.05 threshold, indicating that **neither factor nor their interaction has a significant impact on RER**. Effect sizes (partial eta-square, np2) are also small, supporting the same conclusion.

**2.** The second table shows pairwise **post-hoc tests**, which further compare the means of the individual groups. This allows checking whether any specific pair of conditions differs from another.

- Mean differences between groups are very small

- All p-values are **> 0.05**

- **Effect sizes (Hedges' g)** are low

- **Bayes Factors (BF10)** do not support evidence for group differences

So,the post-hoc comparisons confirm the ANOVA results:
RER values are similar across all four groups , with no significant differences detected.

Together, in this example, both the Two-way ANOVA and post-hoc tests indicate that RER does not differ significantly across genotypes or treatment conditions, and there is no significant interaction between these two factors.