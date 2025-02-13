
![logo-transparent](https://github.com/user-attachments/assets/5eb22c43-970c-4945-9970-8dc012438753)


# How to Download and Run PlasticEnz

## Option A: Using Conda/pip downloads

1. Clone the repositiory and navigate into the tool main folder (where setup.py is located)

<pre> git clone https://github.com/AMK06-1993/PlasticEnz.git </pre>

2. Set Up the Conda Environment with External Tools
Since some external tools aren’t available via pip, start by creating a new conda environment with all required tools. Open your terminal and run:

<pre>conda create -n plasticenz_env -c bioconda -c conda-forge -c defaults \
    python=3.11.11 prodigal hmmer diamond bowtie2 samtools && conda clean --all -y </pre>


Activate the environment:

<pre>conda activate plasticenz_env</pre>

3. Install Python Package Dependencies
With your conda environment activated, the required Python packages by running:

<pre>pip install -r requirements.txt</pre>
    
4. Install the package

<pre>pip install .</pre>
    
5. Test if it runs correctly
Run:
<pre>plasticenz</pre> 
OR 
<pre>plasticenz --help</pre>
