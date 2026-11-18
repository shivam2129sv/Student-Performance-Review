# Student Performance Analysis: Working Notes

## 1. Data exploration and cleaning
- Shape: 1,000 rows x 8 columns. No null values, no duplicate rows, so no cleaning was needed.
- Types: 5 categorical text columns (gender, race/ethnicity, parental level of education, lunch, test preparation course) and 3 integer score columns (math, reading, writing), all 0-100.
- Added columns: `total` (sum of three scores, max 300) and `avg`.

**5-line summary**
1. 1,000 students: 518 female, 482 male; five ethnicity groups (A-E, group C largest at 319).
2. Parental education runs from some high school (179) to master's degree (59); most parents have some college or an associate's degree.
3. 64.5% have standard lunch, 35.5% free/reduced; 35.8% completed test prep.
4. Mean scores: math 66.1, reading 69.2, writing 68.1; total mean 203.3 (median 205, SD 42.8).
5. Lowest scores are 0 (math), 17 (reading) and 10 (writing), so the bottom tail needs attention. The data is complete and consistent.

## 2. Factor analysis
1. **Parental education:** Yes. Average score rises from 63.1 (high school) to 73.6 (master's). ANOVA p < 0.001. The pattern is not perfectly steady: "some high school" (65.1) is slightly above "high school" (63.1).
2. **Test prep:** Yes. Completers score higher in all subjects: math +5.6, reading +7.4, writing +9.9 (all p < 0.001).
3. **Correlations:** reading-writing 0.955; math-reading 0.818; math-writing 0.803. All strongly positive.
4. **Gender:** Female higher in reading (72.6 vs 65.5) and writing (72.5 vs 63.3); male higher in math (68.7 vs 63.6). All differences p < 0.001.
5. **Total score distribution:** Roughly bell-shaped with a longer tail to the left (skew -0.30). Mean 203, median 205, quartiles 175 to 233. 109 students scored 150 or below (average of 50 or less).

## 4. At-risk definition and results
**At-risk = below 50 in any one subject.** 188 students (18.8%) are at risk: 92 in one subject, 41 in two, 55 in all three. Failures by subject: math 135, writing 114, reading 90.

| Group | At-risk % |
|---|---|
| Free/reduced lunch | 31.3 (vs 11.9 standard) |
| No test prep | 23.7 (vs 10.1 completed) |
| Parents some high school / high school | 25.7 / 25.0 |
| Master's degree parents | 10.2 |
| Ethnicity group A / E | 33.7 / 10.0 (group A is only 89 students) |
| Male / Female | 20.5 / 17.2 (not significant, p = 0.20) |

Combined: free/reduced lunch with no prep 37.5%; standard lunch with prep 4.0%.
Chi-square tests: lunch, prep, parental education and ethnicity group are significantly associated with risk (p < 0.01); gender is not.

**Why:** The dataset has no causal information, but the pattern is consistent with fewer home resources and less academic support, with test prep acting as a partial buffer. Risk adds up: students with several disadvantages are far more likely to fall below 50.
