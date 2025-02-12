
How to Download and Run PlasticEnz

Option A: Using Conda/pip downloads

1. Clone the repositiory and navigate into the tool main folder (where setup.py is located)

    `git clone https://github.com/AMK06-1993/PlasticEnz.git`

2. Set Up the Conda Environment with External Tools
Since some external tools aren’t available via pip, start by creating a new conda environment with all required tools. Open your terminal and run:

    `conda create -n plasticenz_env -c bioconda -c conda-forge -c defaults \
        python=3.11.11 prodigal hmmer diamond bowtie2 samtools && conda clean --all -y`

Activate the environment:

    `conda activate plasticenz_env`

3. Install Python Package Dependencies
With your conda environment activated, the required Python packages by running:

    `pip install -r requirements.txt`
    
4. Install the package

    `pip install .`
    
5. Test if it runs correctly
Run:
    `plasticenz` OR `plasticenz --help`
