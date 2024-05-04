# Translation-Reasoning

### Translation

The commond-line arguments can be changed to perform translation in other dataset, model, source and target languages.

```
python3 DER/Translation/translate.py --model=deepseekcoder --dataset=codenet --source_lang=python --target_lang=java --gpu_id=0 --cache_dir=.
```

### Cleaning
To clean the generated translations and extract the proper code from model output, please execute the following:

```
bash scripts/clean_generations.sh deepseekcoder no_test
```

The command-line arguments can be changed to perform cleaning for other models and testing scenarios (e.g., no_test, w_test, misleading_test).

### Validation
To validate the correctness of generated translations, please execute the following:

```
bash scripts/test_translation.sh deepseekcoder no_test
```

The command-line arguments can be changed to perform validation for other models and testing scenarios (e.g., no_test, w_test, misleading_test).

### Reasoning
Please refer to [IER](IER/README.MD) and [SR](SR/README.MD) for execution reasoning scripts and instructions.
