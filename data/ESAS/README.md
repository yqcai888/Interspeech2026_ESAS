The Event-Shifted Acoustic Scene (ESAS) dataset is a benchmark designed to evaluate the robustness of Acoustic Scene Classification (ASC) systems against unknown sound events under event-shift conditions.

Unlike existing ASC datasets that contain clean and consistent audio, ESAS simulates real-world acoustic variability by injecting foreground sound events into background scenes. The dataset combines background recordings from CochlScene (13 scene classes) with foreground events from FSD50K (96 event classes). Semantic consistency between events and scenes is guided by a large language model (LLM).

Dataset statistics:
- Total duration: 211 hours
- Audio format: 10-second mono clips, 44.1 kHz
- Total samples: 76,115
- Scene classes: 13
- Known event types: 27
- Unknown event types: 69

Split composition:
- Training set: 60,855 clips (background only + known events)
- Validation set: 7,573 clips (background only + known events)
- Test set: 7,687 clips (background only + known events + unknown events)

Each sample is accompanied by metadata including original scene labels, event labels and counts, timestamps, signal-to-noise ratio (SNR), dataset split, and mix type.

This dataset is introduced in the paper:
"ESAS: Event-Shifted Acoustic Scene Dataset for Robust Acoustic Scene Classification" 
Accepted at Interspeech 2026.

Please cite the above paper when using this dataset.
