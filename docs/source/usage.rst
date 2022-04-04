Usage
=====

.. _installation:

Installation
------------

Source code from `Github <https://github.com/changlubio/GenomePrep>`_ :

.. code-block:: console

   $ git clone git@github.com:changlubio/GenomePrep.git

Setup
------------

To use GenomePrep, first download relevant files:

.. code-block:: console

   $ make datadir
   $ cd datadir
   $ wget tp://ftp.ensembl.org/pub/release-75/fasta/homo_sapiens/dna/Homo_sapiens.GRCh37.75.dna.toplevel.fa.gz
   $ gunzip Homo_sapiens.GRCh37.75.dna.toplevel.fa.gz
   $ wget https://supfam.mrc-lmb.cam.ac.uk/GenomePrep/datadir/api.23andme.com
   $ wget https://supfam.mrc-lmb.cam.ac.uk/GenomePrep/datadir/badalleles.dat
   $ wget https://supfam.mrc-lmb.cam.ac.uk/GenomePrep/datadir/RS2GRCh37Orien_1.dat
   $ wget https://supfam.mrc-lmb.cam.ac.uk/GenomePrep/datadir/THE_LIST.dat

Use liftOver for build other than GRCh37

.. code-block:: console

   $ wget ftp://hgdownload.cse.ucsc.edu/goldenPath/hg38/liftOver/hg38ToHg19.over.chain.gz
   $ wget http://hgdownload.soe.ucsc.edu/goldenPath/hg18/liftOver/hg18ToHg19.over.chain.gz

Running test DNA
----------------

Run GenomePrep on a typical 23andMe file

.. code-block:: console

   $ cd ..
   $ bin/process.py tutorial/testgenome.zip -d ./datadir -o ./outputs -i vcfindex