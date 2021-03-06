# allennlp-autorun

This is a script to automate running multiple models with minor changes to the config. Inspired from a [HW from Prof. Sameer Singh](https://github.com/sameersingh/uci-statnlp/tree/master/hw3).

`encoders.py` - This file contains the script to extend the base config mentioned at `./test/config` with the mentioned custom config at `encoders.py:18`. 

### What it does?
- The script creates multiple config files and saves them at `./test/config/`. 
- Runs all the listed config files with [AllenNLP](https://github.com/allenai/allennlp) and saves the models to `./test/models/`. 
- Collects `best_validation_accuracy3` metric for all the models and saves the list at `./test/results/autogen_results`
- [Only on macOS] Once all the models are processed, plays an alarm so that you can run to your laptop to check the results. 😄
