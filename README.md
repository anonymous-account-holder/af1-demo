# AF1 Experiment

This directory contains code to run an experiment testing the AF1 circuit on a Llama 3 8B model.

## Setup

It is recommended to use `conda` to manage dependencies.

1.  **Create and activate a conda environment from the provided file:**

    The file `full_eap_ig_env.yml` in the root directory contains the necessary dependencies.

    ```bash
    conda env create -f ../full_eap_ig_env.yml
    conda activate eap-ig
    ```
    Note: if you are not in the `af1-demo` directory, adjust the path to `full_eap_ig_env.yml` accordingly.

2.  **Install additional packages:**

    Some packages need to be installed or updated via pip.

    ```bash
    pip install torch transformer_lens tqdm
    ```

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