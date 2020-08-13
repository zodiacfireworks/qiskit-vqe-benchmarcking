# VQE Benchmarking

A simple set of examples to test VQE with a variety of configurations.

## Some nice images

See more at [gallery] or a full collection at [images] directory

This images corresponds to an experiment run with `qasm_simulator` with a noise model from
`ibmq_16_melbourne`. The experiment was run with 100 shots, using and `UCCSD` initial state and
100 trials of `SPSA` optimizer. The plots shows comparison graphs of the same setup against
distinct qbit mappings.

![img](./results/images/noisy__100__hf__uccsd__spsa__100__energy.jpg)
![img](./results/images/noisy__100__hf__uccsd__spsa__100__energy_convergence_at_minimum_energy.jpg)
![img](./results/images/noisy__100__hf__uccsd__spsa__100__logscale_error_at_minimum_energy.jpg)

## Reqirements

* Python 3.8
* [Pyenv] (optional)
* [Poetry] (optional)

## Install

1. Clone the repository

    ```
    git@github.com:zodiacfireworks/qiskit-vqe-benchmarcking.git
    ```

2. Install python packages

    With poetry

    ```
    poetry intall
    ```

    Or just plain pip

    ```
    pip install -r requirements.dev.txt
    ```

3. Install Juyter plugins
    ```
    poetry run jupyter labextension install @jupyterlab/debugger @jupyterlab/git @jupyterlab/toc @krassowski/jupyterlab_go_to_definition @lckr/jupyterlab_variableinspector @ryantam626/jupyterlab_code_formatter nbdime-jupyterlab
    ```

4. Run Jupyter lab
    ```
    poetry run jupyter lab
    ```


[gallery]: ./GALLERY.md
[images]: ./results/images

[Pyenv]: https://github.com/pyenv/pyenv
[Poetry]: https://python-poetry.org/
