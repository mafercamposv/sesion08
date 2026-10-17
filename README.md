# Práctica 8: BLAST+ local

- Versión de BLAST+: 2.16.0+
- Versión de MAFFT: v7.526 (2024/Apr/26)
- Origen de los datos: /mnt/data/bioinfo1/jmiranda/sesion08

Tabla de resultados ./top5.sh referencias_lgr5.faa proteoma_dlaeve

| qseqid | sseqid | pident | length | evalue | bitscore | qcovs |
|---|---|---|---|---|---|---|
| LGR5\|human\|NP_003658.1 | dlaeveM00000441839 | 33.908 | 870 | 1.11e-143 | 466 | 89 |
| LGR5\|human\|NP_003658.1 | dlaeveM00000727719 | 31.597 | 883 | 9.29e-138 | 434 | 90 |
| LGR5\|human\|NP_003658.1 | dlaeveM00000308285 | 28.094 | 299 | 2.04e-39 | 158 | 33 |
| LGR5\|human\|NP_003658.1 | dlaeveM00000612275 | 29.167 | 432 | 7.98e-33 | 137 | 46 |
| LGR5\|human\|NP_003658.1 | dlaeveM00000132191 | 25.440 | 511 | 2.03e-29 | 126 | 83 |
| LGR5\|mollusc\|Bradybaena_similaris\|BFZ05148.1 | dlaeveM00000727719 | 83.243 | 925 | 0.0 | 1621 | 67 |
| LGR5\|mollusc\|Bradybaena_similaris\|BFZ05148.1 | dlaeveM00000441839 | 56.643 | 1400 | 0.0 | 1444 | 99 |
| LGR5\|mollusc\|Bradybaena_similaris\|BFZ05148.1 | dlaeveM00000308285 | 32.873 | 724 | 5.18e-100 | 346 | 46 |
| LGR5\|mollusc\|Bradybaena_similaris\|BFZ05148.1 | dlaeveM00000132191 | 28.877 | 561 | 7.55e-57 | 216 | 61 |
| LGR5\|mollusc\|Bradybaena_similaris\|BFZ05148.1 | dlaeveM00000351276 | 37.097 | 310 | 1.69e-45 | 178 | 55 |
| LGR5\|mollusc\|Magallana_gigas\|NP_001292277.1 | dlaeveM00000727719 | 50.166 | 903 | 0.0 | 856 | 81 |
| LGR5\|mollusc\|Magallana_gigas\|NP_001292277.1 | dlaeveM00000441839 | 48.394 | 903 | 0.0 | 827 | 81 |
| LGR5\|mollusc\|Magallana_gigas\|NP_001292277.1 | dlaeveM00000308285 | 46.757 | 370 | 1.72e-95 | 328 | 56 |
| LGR5\|mollusc\|Magallana_gigas\|NP_001292277.1 | dlaeveM00000351276 | 29.714 | 525 | 5.53e-41 | 163 | 78 |
| LGR5\|mollusc\|Magallana_gigas\|NP_001292277.1 | dlaeveM00000132191 | 28.269 | 520 | 1.85e-38 | 156 | 74 |
| LGR5\|mollusc\|Pomacea_canaliculata\|XP_025085505.1 | dlaeveM00000727719 | 58.758 | 902 | 0.0 | 1065 | 79 |
| LGR5\|mollusc\|Pomacea_canaliculata\|XP_025085505.1 | dlaeveM00000441839 | 57.556 | 900 | 0.0 | 1031 | 79 |
| LGR5\|mollusc\|Pomacea_canaliculata\|XP_025085505.1 | dlaeveM00000308285 | 32.228 | 754 | 7.16e-106 | 358 | 66 |
| LGR5\|mollusc\|Pomacea_canaliculata\|XP_025085505.1 | dlaeveM00000351276 | 30.989 | 526 | 1.23e-52 | 200 | 76 |
| LGR5\|mollusc\|Pomacea_canaliculata\|XP_025085505.1 | dlaeveM00000132191 | 28.571 | 539 | 4.82e-50 | 193 | 77 |

Después de filtrar los resultados buscando que el parentesco fuera real y que el gen no estuviera incompleto, encontramos que la babosa tiene 6 genes que tienen buen e value y una cobertura mayor al 60%. Revisando el mapa de mRNAs, vi que estos se ubican en los cromosomas: 2, 4, 5, 6 y 10.

Por otro lado, descartamos al gen dlaeveM00000909458. Al principio engaña porque tiene un buen E-value (10⁻¹⁴), lo que significa que un pedazo de él es casi idéntico a LGR5. Sin embargo, su cobertura es muy baja porque está incompleto. Por último al observar los resultados, podemos observar que la babosa solo tiene 2 receptores LGR verdaderos: el 6 y el 10.
