# 𝑻𝒐𝒘𝒂𝒓𝒅𝒔 𝑬𝒗𝒆𝒏𝒕-𝑹𝒐𝒃𝒖𝒔𝒕 𝑨𝒄𝒐𝒖𝒔𝒕𝒊𝒄 𝑺𝒄𝒆𝒏𝒆 𝑪𝒍𝒂𝒔𝒔𝒊𝒇𝒊𝒄𝒂𝒕𝒊𝒐𝒏
<p align="center">
  <!-- 会议状态与许可证 -->
  <img src="https://img.shields.io/badge/Conference-Interspeech_2026-purple" alt="Conference">
  <img src="https://img.shields.io/badge/Status-Accepted-success" alt="Status">
  <img src="https://img.shields.io/badge/License-Appache-2.0-green" alt="License">
  <br>
  <!-- 数据集与 DOI -->
  <img src="https://img.shields.io/badge/Dataset-ESAS-blue" alt="Dataset">
  <img src="https://img.shields.io/badge/DOI-10.5281/zenodo.20623264-blue" alt="DOI">
  <br>

🔥 𝙽𝚎𝚠𝚜: 𝙾𝚞𝚛 𝚙𝚊𝚙𝚎𝚛 𝚑𝚊𝚜 𝚋𝚎𝚎𝚗 𝚊𝚌𝚌𝚎𝚙𝚝𝚎𝚍 𝚋𝚢 𝙸𝚗𝚝𝚎𝚛𝚜𝚙𝚎𝚎𝚌𝚑 𝟸𝟶𝟸𝟼!

💭 𝚃𝚑𝚒𝚜 𝚛𝚎𝚙𝚘𝚜𝚒𝚝𝚘𝚛𝚢 𝚙𝚛𝚘𝚟𝚒𝚍𝚎𝚜 𝚊𝚗 𝚎𝚊𝚜𝚢 𝚠𝚊𝚢 𝚝𝚘 𝚝𝚛𝚊𝚒𝚗 𝚢𝚘𝚞𝚛 𝚖𝚘𝚍𝚎𝚕𝚜 𝚘𝚗 𝚝𝚑𝚎 𝙴𝚂𝙰𝚂 𝚍𝚊𝚝𝚊𝚜𝚎𝚝. 𝙸𝚗 𝚊𝚍𝚍𝚒𝚝𝚒𝚘𝚗 𝚝𝚘 𝚍𝚘𝚠𝚗𝚕𝚘𝚊𝚍𝚒𝚗𝚐 𝚝𝚑𝚎 𝚙𝚛𝚎-𝚐𝚎𝚗𝚎𝚛𝚊𝚝𝚎𝚍 𝙴𝚂𝙰𝚂 𝚍𝚊𝚝𝚊𝚜𝚎𝚝, 𝚢𝚘𝚞 𝚌𝚊𝚗 𝚊𝚕𝚜𝚘 𝚋𝚞𝚒𝚕𝚍 𝚒𝚝 𝚏𝚛𝚘𝚖 𝚜𝚌𝚛𝚊𝚝𝚌𝚑 𝚞𝚜𝚒𝚗𝚐 𝚝𝚑𝚎 𝚙𝚛𝚘𝚟𝚒𝚍𝚎𝚍 𝚙𝚒𝚙𝚎𝚕𝚒𝚗𝚎 𝚝𝚘 𝚢𝚘𝚞𝚛 𝚗𝚎𝚎𝚍𝚜.  

📑 **[𝚁𝚎𝚊𝚍 𝚝𝚑𝚎 𝚙𝚊𝚙𝚎𝚛 𝚘𝚗 𝚊𝚛𝚡𝚒𝚟.](https://arxiv.org/abs/2606.06921)**

👉 **[𝙳𝚘𝚠𝚗𝚕𝚘𝚊𝚍 𝚝𝚑𝚎 𝙴𝚂𝙰𝚂 𝙳𝚊𝚝𝚊𝚜𝚎𝚝 𝚘𝚗 𝚉𝚎𝚗𝚘𝚍𝚘.](https://doi.org/10.5281/zenodo.21317541)**

## 𝑰𝒏𝒕𝒓𝒐𝒅𝒖𝒄𝒕𝒊𝒐𝒏
Existing ASC datasets typically contain recordings of clean and consistent audio, while real-world environments often include diverse and unexpected sound events. To bridge this gap, ESAS simulates real-world acoustic variability by injecting foreground sound events into background scenes with the assistance of large language models.
In this work, we present the construction methodology, dataset statistics, and evaluation protocols. A comprehensive evaluation of ASC systems on ESAS reveals that existing models suffer significant performance degradation when facing the **event-shift** challenge.


## 𝑬𝑺𝑨𝑺 𝑫𝒂𝒕𝒂𝒔𝒆𝒕
The Event-Shifted Acoustic Scene (ESAS) dataset is designed to evaluate the robustness of ASC systems against unknown sound events. It combines **CochlScene** (13 scene classes) as background and **FSD50K** (96 event classes) as foreground.

| Split | Background Only | Known Events | Unknown Events | Total |
| :--- | :--- | :--- | :--- | :--- |
| **Train** | 54,799 | 6,056 | — | 60,855 |
| **Validation** | 3,856 | 3,716 | — | 7,572 |
| **Test** | 2,623 | 2,499 | 2,532 | 7,654 |
| **Total** | 61,312 | 12,271 | 2,532 | **76,081** |

- **Audio format:** 10-second mono clips, 44.1 kHz WAV
- **Total duration:** 211 hours
- **Metadata:** Includes filename, scene label, mix type, num event types, clip snr level
- **Note:** The ESAS dataset contains **only the mixed samples** (Known + Unknown Events). The background-only samples are **not included** and must be downloaded separately from [CochlScene](https://zenodo.org/records/7080122).

## 𝑺𝒚𝒔𝒕𝒆𝒎 𝑫𝒆𝒔𝒄𝒓𝒊𝒑𝒕𝒊𝒐𝒏

- All configurations of model, dataset and training can be done via a simple YAML file.
- Entire system is implemented using [PyTorch Lightning](https://lightning.ai/).
- Logging is implemented using [TensorBoard](https://lightning.ai/docs/pytorch/stable/extensions/generated/lightning.pytorch.loggers.TensorBoardLogger.html#tensorboardlogger). ([Wandb API](https://lightning.ai/docs/pytorch/stable/extensions/generated/lightning.pytorch.loggers.WandbLogger.html) is also supported.)
- Various task-related techniques have been included.
   * 4 Spectrogram Extractor: Cnn3Mel, CpMel, BEATsMel, PaSSTMel.
   * 6 High-performing Backbones: BEATs, PASST, TF-SepNet, BC-ResNet, CP-Mobile, GRU-CNN.
   * 5 Plug-and-played Data Augmentation Techniques: MixUp, MixUpMultiLabels, FreqMixStyle, SpecAugmentation, Device Impulse Response Augmentation.


## 𝑮𝒆𝒕𝒕𝒊𝒏𝒈 𝑺𝒕𝒂𝒓𝒕𝒆𝒅

1. Clone this repository.
2. Create and activate a [conda](https://docs.anaconda.com/free/miniconda/index.html) environment:

```
conda create -n ESAS
conda activate ESAS
```

3. Install [PyTorch](https://pytorch.org/get-started/previous-versions/) version that suits your system. For example:

```
pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu118
# or for cuda >= 12.1
pip install torch torchvision torchaudio
```

4. Install requirements:

```
pip install -r requirements.txt
```

5. Download and extract the Event-Shifted Acoustic Scene (ESAS) dataset according to your needs. The directory should be placed in the **parent path** of code directory. You should end up with a directory that contains, among other files, the following: `..data/ESAS/` - A directory containing audio files in *wav* format.

6. Several default configuration yaml files are provided in config/. The training procedure can be started by running the following command:
```
python -m main fit --config config/cpmobile/cpmobile_train.yaml
```

7. Test model:
```
python -m main test --config config/cpmobile/cpmobile_test.yaml --ckpt_path path/to/ckpt
```

8. View results:
```
tensorboard --logdir log/cpmobile_train  # Check training results
tensorboard --logdir log/cpmobile_test  # Check testing results
```
Then results will be available at [localhost port 6006](http://127.0.0.1:6006/).

## 𝑫𝒂𝒕𝒂𝒔𝒆𝒕 𝑮𝒆𝒏𝒆𝒓𝒂𝒕𝒊𝒐𝒏 𝒕𝒐 𝒚𝒐𝒖𝒓 𝒏𝒆𝒆𝒅𝒔
In addition to downloading the pre-generated ESAS dataset, you can also build it from scratch using the provided pipeline to your needs. The generation process consists of three main stages:

- **Audio Event Tagging** – Use the BEATs model to predict event probabilities for each CochlScene recording.
- **Metadata Generation** – Create the ESAS metadata, identify “real-unknown” recordings, and define known/unknown event splits.
- **Audio Mixing** – Synthesise the final dataset by mixing background scenes with foreground events according to the ESAS protocol.
All scripts are located in the root directory of the repository.


**Requirements:**
- CochlScene dataset placed in a known directory (e.g.,  `../CochlScene`).
- BEATs model checkpoint (e.g.,  `BEATs_iter3_plus_AS2M_finetuned_on_AS2M_cpt2.pt`) downloaded and placed in an accessible location.
- FSD50K metadata (for label mapping) available in  `.../FSD50K/FSD50K.ground_truth`.


***Script 1:*** `audio_tagging.py`

Before running, open the script and adjust the following variables to match your local paths:
```python
audio_dir = ".../CochlScene"   # Path to CochlScene root
ckpt_event_model = ".../BEATs_iter3_plus_AS2M_finetuned_on_AS2M_cpt2.pt"   # BEATs checkpoint
fsd50k_meta_dir = ".../FSD50K/FSD50K.ground_truth"   # FSD50K metadata directory
```

The script processes all audio files in `audio_dir` and saves a CSV file named `CochlScene_event_tags_with_BEATs.csv` in the same directory. 
This file contains one row per CochlScene recording, with columns for each BEATs class MID storing the predicted probability.


***Script 2:*** `generate_metadata.py`

Edit the paths in the main() function if necessary (the defaults are shown below):

```python
generator = ESASMetadataGenerator(
    scene_dir = ".../CochlScene",
    event_mapping_path = "docs/event_scene_grouping.json",
    fsd50k_meta_dir = ".../FSD50K/FSD50K.ground_truth"
)
```

Output files are created in the following locations:

`data/metadata/metadata_template.csv` – empty template with the correct columns.
`data/metadata/real_unknown_metadata.csv` – list of real‑unknown recordings.
`docs/event_splits.json` – known/unknown event lists and statistics.
`docs/metadata_schema.json` – field descriptions for the metadata.
`docs/scene_event_coverage.json` – per‑scene event counts.
`docs/real_unknown_statistics.json` – distribution of real‑unknown recordings.


***Script 3:***: `mix_audio.py`

The mixer supports three mix types:
**background** – only the original scene audio.
**known** – scene mixed with known events (from the training split of FSD50K).
**unknown** – scene mixed with unknown events (from the evaluation split of FSD50K).
Events are placed with allowed overlap, and each event’s audio may be time‑stretched and pitch‑shifted for variation. The mixer also tracks file usage to ensure balanced sampling and prevent excessive reuse of the same event file.

To generate the dataset for a specific split, run:
```
python esas_mixer.py --split {train,val,test} --clips_per_scene N [ --max_reuse_per_file M ]
```

The generated audio files are saved under ``data/esas_data/{split}/`` with filenames like ``{scene_label}_{split}_{...}.wav``. Metadata for the split is written to ``data/metadata/{split}.csv``.

After all three splits have been generated, the folder structure should look like:
```
.../data/ESAS/
├── train/           # background + known clips
├── val/             # background + known clips
├── test/            # background + known + unknown clips
└── meta_data/       # per-split CSV files
```

## 𝑪𝒖𝒔𝒕𝒐𝒎𝒊𝒛𝒆 𝒀𝒐𝒖𝒓 𝑺𝒚𝒔𝒕𝒆𝒎

Deploy your model in `model/backbones/` and inherit the **_BaseBackbone**:
```
class YourModel(_BaseBackbone):
...
```
Implement new spectrogram extractor in `util/spec_extractor/` and inherit the **_SpecExtractor**:
```
class NewExtractor(_SpecExtractor):
...
```
Declare new data augmentation method in `util/data_augmentation/` and inherit the **_DataAugmentation**:  
```
class NewAugmentation(_DataAugmentation):
...
```

More instructions can be found on [LightningCLI](https://lightning.ai/docs/pytorch/stable/cli/lightning_cli.html)

## 𝑪𝒊𝒕𝒂𝒕𝒊𝒐𝒏
If you find our code helps, we would appreciate using the following citation:
```
@misc{cai2026eventrobustacousticsceneclassification,
      title={Towards Event-Robust Acoustic Scene Classification}, 
      author={Yiqiang Cai and Bohan Hu and Yu Yang and Pengwei Lu and Shengchen Li and Xi Shao},
      year={2026},
      eprint={2606.06921},
      archivePrefix={arXiv},
      primaryClass={cs.SD},
      url={https://arxiv.org/abs/2606.06921}, 
}
```

