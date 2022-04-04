.. GenomePrep documentation master file, created by
   sphinx-quickstart on Fri Jun  8 10:09:40 2018.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.


GenomePrep: Preprocess Direct-To-consumer (DTC) Genomes
=======================================================

**GenomePrep** is a Python library for genetics enthusiasts 
that prepare direct-to-consumer DNA data for analysis using popular bioinformatics tools. 
It performs the following tasks:

1. Parse SNPs from popular DTC providers
2. Check for missing calls and duplicated SNPs
3. Determine assembly, and sanity check for similarity to the reference genome
4. Deduce the genotyping array version
5. Apply a genotyping-array-based SNP sanity filter (optional)
6. Convert to 23andMe-like format and VCF format for downstream analysis

This project was developed on the goodwill of over 7,000 open genome data made public between 2011 and 2020, 
addressing the problem of processing raw DTC DNA data in the context of the present: genotype arrays.

More information about genotyping array, ancestral relatedness can be found in `our paper on CSBJ <https://doi.org/10.1016/j.csbj.2021.06.040>`_:

C. Lu, B. Greshake Tzovaras, J. Gough, A survey of direct-to-consumer genotype data,and quality control tool (GenomePrep) for research, Computational and Structural Biotechnology Journal(2021)

You can upload and process your genome `on server <https://supfam.mrc-lmb.cam.ac.uk/GenomePrep/checkit.html>`_.

**Usage**

.. code:: bash

    process.py [infile]
    
--------

Check out the :doc:`usage` section for further information, including
how to :ref:`installation` the project.
.. toctree::

   usage
   api
