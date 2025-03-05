Demo Notebooks
==============

We provide a set of demo notebooks to get started with using CEBRA. To
run the notebooks, you need a working Jupyter notebook server, a CEBRA
installation, and the datasets required to run the notebooks, available on 
`FigShare <https://figshare.com/s/60adb075234c2cc51fa3>`_.


.. nbgallery::
   :maxdepth: 2

   Getting Started with CEBRA <demo_notebooks/CEBRA_best_practices.ipynb>
   Encoding of space, hippocampus (CA1) <demo_notebooks/Demo_hippocampus.ipynb>
   Decoding movie features from (V1) visual cortex <demo_notebooks/Demo_Allen.ipynb>
   Forelimb dynamics, somatosensory (S1) <demo_notebooks/Demo_primate_reaching.ipynb>
   Synthetic neural benchmarking <demo_notebooks/Demo_synthetic_exp.ipynb>
   Hypothesis-driven analysis <demo_notebooks/Demo_hypothesis_testing.ipynb>
   Consistency <demo_notebooks/Demo_consistency.ipynb>
   Decoding <demo_notebooks/Demo_decoding.ipynb>
   Topological data analysis <demo_notebooks/Demo_cohomology.ipynb>
   Technical: Training models across animals <demo_notebooks/Demo_hippocampus_multisession.ipynb>
   Technical: conv-piVAE <demo_notebooks/Demo_conv-pivae.ipynb>
   Technical: S1 training with MSE loss <demo_notebooks/Demo_primate_reaching_mse_loss.ipynb>
   Technical: Learning the temperature parameter <demo_notebooks/Demo_learnable_temperature.ipynb>
   Demo: Using OpenScope Data <demo_notebooks/Demo_openscope_databook.ipynb>
   Demo: Using Dandi Data <demo_notebooks/Demo_dandi_NeuroDataReHack_2023.ipynb>
   

The demo notebooks can also be found on `GitHub <https://github.com/AdaptiveMotorControlLab/CEBRA-demos>`__.

Installation
------------

Before you can run these notebooks, you must have a working installation of CEBRA.
Please see the dedicated :doc:`Installation Guide </installation>` for information on installation options using ``conda``, ``pip`` and ``docker``.

Synthetic Experiment Demo (CEBRA, piVAE, tSNE, UMAP):
This demo requires several additional packages that have differing
requirements to CEBRA. Therefore, we recommend using the supplied
``docker`` container or ``conda`` cebra-full env.


Demo Data 
---------

We host prepackaged data on
`figshare <https://figshare.com/s/60adb075234c2cc51fa3>`__. And several of the demo notebooks have an automatic data download function.


If you don't see the auto-download, and you use Google Colaboratory, you can easily add the following code into an early cell in the notebook to directly download and use:

.. code-block::

   #for google colab only, run this cell to download and extract data:
   !wget --content-disposition https://figshare.com/ndownloader/files/36869049?private_link=60adb075234c2cc51fa3
   !mkdir data
   !tar -xvf "/content/data.tgz" -C "/content/data"

For different paths, you can specify the ``CEBRA_DATADIR=...``
environment variable. You can do this by placing
``import os; os.environ['CEBRA_DATADIR'] = "path/to/your/data"`` at the
**top** of your notebook.

Contributing 
------------

We welcome Demo notebooks from others! Please fork the repo, add your notebook, check that it works on Google Colaboratory (remove the launch button within your PR), and then open a PR! Please also edit the "gallery" list (see the soure code for this page), and finally, add an icon `here <https://github.com/AdaptiveMotorControlLab/CEBRA-assets>`__.


For reference, the original open-source data we used in Schneider, Lee, Mathis 2023 is available at:

- `Hippocampus dataset <https://crcns.org/data-sets/hc/hc-11/about-hc-11>`_, using a 
  `preprocessing script <https://github.com/zhd96/pi-vae/blob/main/code/rat_preprocess_data.py>`_.
- `Primate S1 dataset <https://gui.dandiarchive.org/#/dandiset/000127>`_.
- Allen Institute `Neuropixels dataset <https://allensdk.readthedocs.io/en/latest/visual_coding_neuropixels.html>`_ and `2P dataset  <https://allensdk.readthedocs.io/en/latest/>`_.


