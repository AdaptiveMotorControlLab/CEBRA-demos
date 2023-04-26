Demo Notebooks
==============

We provide a set of demo notebooks to get started with using CEBRA. To
run the notebooks, you need a working Jupyter notebook server, a CEBRA

   Hypothesis-driven analysis <demo_notebooks/Demo_hypothesis_testing.ipynb>
   Consistency <demo_notebooks/Demo_consistency.ipynb>
   Decoding <demo_notebooks/Demo_decoding.ipynb>
   Topological data analysis <demo_notebooks/Demo_cohomology.ipynb>
   Technical: Training models across animals <demo_notebooks/Demo_hippocampus_multisession.ipynb>
   Technical: conv-piVAE <demo_notebooks/Demo_conv-pivae.ipynb>
   Technical: S1 training with MSE loss <demo_notebooks/Demo_primate_reaching_mse_loss.ipynb>
   Technical: Learning the temperature parameter <demo_notebooks/Demo_learnable_temperature.ipynb>

Installation
------------

Before you can run these notebooks, you must have a working installation of CEBRA.
Please see the dedicated :doc:`Installation Guide </installation>` for information on installation options using ``conda``, ``pip`` and ``docker``.

Synthetic Experiment Demo (CEBRA, piVAE, tSNE, UMAP):
This demo requires several additional packages that have differing
requirements to CEBRA. Therefore, we recommend using the supplied
``docker`` container or ``conda`` cebra-full env.

Download Demo Data From FigureShare
-----------------------------------

We host prepackaged data on
`figshare <https://figshare.com/s/60adb075234c2cc51fa3>`__. Please
download them and check the loading directory is correct in the
notebook. By default we assume you have downloaded the data in the
``./data/`` directory in the repository root.

For different paths, you can specify the ``CEBRA_DATADIR=...``
environment variable. You can do this by placing
``import os; os.environ['CEBRA_DATADIR'] = "path/to/your/data"`` at the
**top** of your notebook.

For reference, the original data is available at:

- Allen Institute `Neuropixels dataset <https://allensdk.readthedocs.io/en/latest/visual_coding_neuropixels.html>`_ and `2P dataset  <https://allensdk.readthedocs.io/en/latest/>`_.


