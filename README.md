### Summary:
This repository contains preliminary data for the usage of photogrammetry to measure breast volume as an approach to quantify post-radiation breast volume reduction for prediction purposes. Use of photogrammetry may represent an alternative to CT imaging which exposes patients to unnecessary radiation.

### Methodology:
Two breastform models (Breastform1.stl - large, Breastform2.stl - small) were 3D printed and post-processed (e.g., spraypainted, marked) for subsequent scanning using commerical (Polycam) and open-source (Meshroom) photogrammetry software. Re-constructed breastform meshes from the photogrammetry software were post-processed and analyzed using Meshmixer to quantify their volume. The volumes of the reconstructed meshes were then compared to the original model to obtain % errors in volume for reconstruction.

### Results:
| Model | Software | Volume (mm<sup>3</sup>) | Reference Volume (mm<sup>3</sup>) | Error (%) |
| -- | -- | -- | -- | -- |
| Breastform1 | Polycam | 431119 | 463845 | 7.1 |
| Breastform1 | Meshroom | 483873 | 463845 | 4.2 |
| Breastform2 | Polycam | 264015 | 274992 | 4.0 |
| Breastform2 | Meshroom | 257176 | 274992 | 6.5 |

*Of note, these error rates incorporate error from both the 3D printing and photogrammetry process

### File patterns:
- Breastform.stl - original breastform shell model
- Breastform_filled_scaled.stl - filled breastform model scaled to printer bed. The volume of this model was used as the reference point
- Breastform_meshroom_post_meshmixer.stl - breastform model re-constructed using Meshroom after being post-processed by Meshmixer
- Breastform_poly_post_meshmixer.stl - breastform model re-constructed using Polycam after being post-processed by Meshmixer