# AF1 Experiment

This directory contains demo code to run specifically the Table 4 experiment on the "Original" template, testing the AF1 circuit on a Llama 3 8B model. We hope this gives some more clarity into the code and mechanisms.

## Setup

It is recommended to use `conda` to manage dependencies.

1.  **Create and activate a conda environment from the provided file:**

    The file `af1-env.yml` in the root directory contains the necessary dependencies.

    ```bash
    conda env create -f af1-env.yml
    conda activate af1-env
    ```
    Note: There may be additional unneeded packages in this yml. 

## Running the experiment

To run the experiment for the "Original" template, execute the following script:

```bash
python table_4_original.py
```

You can customize the experiment by passing command-line arguments. For example, to use a different model:

```bash
python table_4_original.py --model_name pythia
```

For a full list of options, run:
```bash
python table_4_original.py --help
``` 
