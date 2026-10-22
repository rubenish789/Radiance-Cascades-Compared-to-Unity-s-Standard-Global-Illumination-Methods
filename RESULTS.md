# Results

Frame time results for every scene and GI method. The values are taken from the `SUMMARY` block at the end of each CSV file in `Measured Data/`. All values are in milliseconds per frame; **lower is better**.

Methods: `NoGI` — no global illumination (baseline), `RC` — Radiance Cascades, `SSGI` — Screen Space Global Illumination, `RTLM`.

## 95th percentile frame time (`p95_ms`)

| Method | Isometric | Realistic FPS | Stylized Fps |
|--------|----------:|--------------:|-------------:|
| NoGI   | 3.335 | 3.025 | 2.911 |
| RC     | 4.651 | 5.024 | 4.145 |
| RTLM   | 5.262 | 5.359 | 4.137 |
| SSGI   | 9.770 | 7.957 | 8.030 |

## Average frame time (`avg_ms`)

| Method | Isometric | Realistic FPS | Stylized Fps |
|--------|----------:|--------------:|-------------:|
| NoGI   | 3.149  | 2.698 | 2.544 |
| RC     | 4.747  | 4.705 | 3.981 |
| RTLM   | 4.995  | 5.151 | 3.730 |
| SSGI   | 10.251 | 7.473 | 7.364 |

In two Isometric runs (RC and SSGI) `avg_ms` is higher than `p95_ms`. This means the average is pulled up by a small number of very slow frames, so `p95_ms` is the more reliable value for comparing the methods.
