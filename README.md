# Training on the Test Set: Mapping the System-Problem Space in AI

This repo provides a single Jupyter notebook for the experiment setup as reported in our paper _"Training on the Test Set: Mapping the System-Problem Space in AI"_, in which we introducing the concept of assessor models.

The experiment has been rewritten to provide single readable and linear flow without any abstraction for instructional and documentation purposes. No GPU is required to run, as the dataset and the models are very small.

The results here should be reproducible, as we have made all computations deterministic, and provided fine-grained description of the dependencies through the `pyproject.toml` and corresponding `poetry.lock`.

## Disclaimer

Statistical significance of results is abysmal. Dataset size is small, nor do we report across repetitions. Any difference in performance in predictive power between the assessor and the task system is subject to high variance, and can be no indication of any superiority of the assessor models calibration (quite the opposite).

We have also observed that the baseline neural nets are now better calibrated by default in this reimplementation in Pytorch (previously Tensorflow), potentially due to programming error on our side before, or due to the variation.

Because of these reasons, the plots generated here are of course different from the one in the paper, but we have included the original instance level results as well.

In any case, the goal of the paper has never been to prove any sort of improvement in calibration with assessors, only that it was possible to build them and be comparable.
