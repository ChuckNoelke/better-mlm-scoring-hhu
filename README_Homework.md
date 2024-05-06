# A Better Way to Do Masked Language Model Scoring Homework


Practical Part:

- create venv Python 3.10
- install requirements

- adjusted dataset_scoring.py to allow facebook models
 - line 37 - 47
 - line 93


- created correlate-opt-and-bert-scores.ipynb as copy from original notebook
    - added additional directory for facebook model
    - added function call for comparison of models




## Run
Scoring the `bert-base-cased` model on the `EventsAdapt` dataset using the `PLL-word-l2r` metric:
```
cd better-mlm-scoring-analyses
```
```
python dataset_scoring.py --dataset EventsAdapt \
                          --model bert-base-cased \
                          --which_masking within_word_l2r
```
Masking options are `original`, `within_word_l2r`, `within_word_mlm`, `global_l2r`

