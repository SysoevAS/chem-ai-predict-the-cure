# История экспериментов

| Submission | Описание | Score | Статус |
|---|---|---:|---|
| `baseline_submission.csv` | Первый baseline | 305.78271 | complete |
| `advanced_submission.csv` | Первый advanced pipeline | 300.32095 | complete |
| `tree_no_overlay_submission.csv` | Tree baseline без overlay | 293.01010 | complete |
| `v2_tree_no_overlay.csv` | Усиленная tree-версия | 288.39467 | complete |
| `v7_si_overlay_100.csv` | Полная замена SI на модель | 279.10178 | complete |
| `v9_si_model_formula_050.csv` | SI model + formula 0.50 | 271.39276 | complete |
| `Edit17.csv` | Сильная промежуточная SI-версия | 270.57525 | complete |
| `v30_edit17_stack_ic50cc50_005_keep_si.csv` | 5% stack для IC50/CC50, SI оставлен | 270.33545 | complete |
| `v31_adv_weighted_ic50cc50_keep_si.csv` | Первый adversarial weighted overlay | 269.81436 | complete |
| `v32_adv_weighted_ic50_012_cc50_018_keep_si.csv` | Adv overlay IC50 0.012 / CC50 0.018 | 269.56671 | complete |
| `v33_adv_weighted_ic50_016_cc50_024_keep_si.csv` | Adv overlay IC50 0.016 / CC50 0.024 | 269.44732 | complete |
| `v34_adv_weighted_ic50_020_cc50_030_keep_si.csv` | Финальный официальный кандидат | 269.39668 | complete |
| `v35_adv_ic50_020_cc50_038_keep_si.csv` | Больше вес CC50 overlay | 269.49952 | complete |
| `v36_domain_subset_ic50cc50_keep_si.csv` | Domain subset вариант | 269.45322 | complete |
| `v34_adv_weighted_ic50_020_cc50_030_keep_si (1).csv` | Post-deadline проверка | 268.87677 | after deadline |

## Краткий вывод

Работа шла от простых baseline к более аккуратным target-wise решениям.

Основной прогресс:

```text
305.78 -> 293.01 -> 288.39 -> 279.10 -> 271.39 -> 270.57 -> 270.33 -> 269.39
```

Главный скачок качества произошёл после отдельной работы с `SI` и использования связи:

```text
SI = CC50 / IC50
```

Финальный официальный submission:

```text
v34_adv_weighted_ic50_020_cc50_030_keep_si.csv
```

Score:

```text
269.39668
```
