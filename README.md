# Minecraft Ore Detection

A YOLOv8 model that detects 7 Minecraft ores: coal, diamond, gold, lapis, redstone, iron and emerald.

## Run it

1. Open `prepare_data.ipynb` in Colab and add your Roboflow key as a secret named `ROBOFLOW_API_KEY`.
2. Run it from top to bottom. Check the class-name printout and the spot-check images before moving on.
3. Open `train.ipynb` in Colab with a GPU on, then run it from top to bottom. It loads the merged dataset from Google Drive and saves results there.

To work outside Colab, set `ROBOFLOW_API_KEY` as an environment variable and start Jupyter from this folder.

## Data

| Name | Roboflow project | Version |
|---|---|---|
| `oblig10` | [oblig10/minecraft-ore-detection-20pzg-xejw6](https://universe.roboflow.com/oblig10/minecraft-ore-detection-20pzg-xejw6) | 2 |
| `blocks` | [main-data/minecraft-blocks](https://universe.roboflow.com/main-data/minecraft-blocks) | 1 |
| `360` | [aasmaa-alibhai/360-3wqmv](https://universe.roboflow.com/aasmaa-alibhai/360-3wqmv) | 1 |

Downloads go in `datasets/raw/` and are never edited. The merged dataset is rebuilt in `datasets/merged/`. Neither folder is committed to git.

## To do

- [ ] Decide whether `360` is train or test data (`DATASETS` in `prepare_data.ipynb`)
- [ ] Add 30 new labelled images per person, as the brief requires
- [ ] Train the baseline and save its results
