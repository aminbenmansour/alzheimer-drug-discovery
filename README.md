# 🧬 🧪 Alzheimer-drug-discovery
> Hearing the stories of people suffering from alzheimer is always heartbreaking. Our goal is to make machine learning beneficial for everybody.
## 📜 Definitions

a drug is biological or chemical entity that can modulate the course of a **desease state** by interacting with its **target protein**

* *biological entity* is composed of *proteins or peptide*. (e.g. antibodies)
* *chemical entity* is composed of *compounds* aka molecules. (e.g. small molecules)
---
**Bioinformatics** is a discipline entailing the useof computational approaches to analyze biological data.
* Analyze and compare genes, proteins and genomes.
* Exploring structures and functions of biomolecules (DNA, protein, lipid and carbohydrate).
* explore network biology and letabolic pathways.
---

## ✨ Demo

## 🏗 Project's structure
in this subsection we will emphasise the role each directory plays in thos repository.
* `notebooks` contains jupyter notebooks for all the hooks a *professional* model should pass through, from data gathering, EDA, approving or denying hypothesis, model training and models comparison.
* `data` contains data processed at each step.
* `figures` contains saved figures that could be useful for scientists writing their report.
* `toolkits` contains required files to run PaDEL descriptors
* `bioactivity-prediction-app` here resides the webapp, it summarizes all efforts done in other directories.

## 🧑‍💻 Usage

* **Prerequisites**

    Make sure you have:
    * `python 3.X` installed
    * `conda environment` by installing [anaconda](https://www.anaconda.com/products/individual) or [miniconda](https://conda.io/miniconda.html) (recommended).

* **Serializing the model**

    The size of the serialized model was relatively too large so you have to generate it by yourself.
    
    Under `bioactivity-prediction-app` directory, open the following Jupyter Notebook `bioactivity_prediction_model.ipynb` and run it with your `conda environment`.
    
    You will remark that a new file, `bioactivity_prediction_model.ipynb`, appears.

* **Launching application**

    Under `bioactivity-prediction-app` directory, open the `bash terminal` and execute the following commands.

    1. create a virtual environment
    ``` 
    python3 -m venv alzheimer-drug-discovery
    ```

    2. activate the virtual environment
    ```
    source  alzheimer-drug-discovery/bin/activate 
    ```
    3. install the projects' dependencies
    ```
    pip install -r requirements.txt
    ```
    
    4. start the application
    ```
    streamlit run app.py
    ```
   
Enjoy interacting with your application on your favorite web browser 🎉

## 🧑‍🔬 Domain knowledge
building domain knowledge is the most fragile part of every data science project. **It took me hours of research to get the fundamentals of *bioinformatics***. I would rather write a wiki instead but you can deep dive into the [references](https://github.com/aminbenmansour/alzheimer-drug-discovery#-references--research-papers) below 👇.
## 🏦 Database
[ChEMBL](https://www.ebi.ac.uk/chembl/) is a manually curated database of bioactive molecules with drug-like properties. It brings together chemical, bioactivity and genomic data to aid the translation of genomic information into effective new drugs.
## ⁉️ Frequently Asked Questions (FAQ)
### **🙋 why are we calculating pubchem fingerprints even after calculating thelipinski descriptors ? what is the difference ?**
👉 the **lipinski descriptors** will provide us with a set of a simple molecular descriptors that will provide us with the drug-like (oral drug) properties of the molecule (rule of five). in the other hand, thanks to the **pubchem fingerprints**, each molecule will be described by the unique building blocks, this will allow us to create a unique properties of the drug and that is the essence of *drug discovery* and *drug design*. the connectivity of the blocks are giving rise to the unique structure of the molecule and also the unique molecular properties. **we have to find a way to rearrange the blocks in such a way that the molecule provides the most potency toward the target protein while also being safe and not so toxic**.
## 📑 References & Research papers
* [Alzheimer's disease - plaques, tangles, causes, symptoms & pathology](https://www.youtube.com/watch?v=v5gdH_Hydes)
* [What is Alzheimer's disease? - TED-Ed](https://www.youtube.com/watch?v=yJXTXN4xrI8)
* [Efficacy of acetylcholinesterase inhibitors in Alzheimer's disease](https://www.sciencedirect.com/science/article/pii/S0028390820304202)
* [Treatment of dementia and Alzheimer's disease l Acetylcholinesterase inhibitors](https://www.youtube.com/watch?v=yD4W-iAHfUo)
* [An Introduction to Computational Drug Discovery](https://www.youtube.com/watch?v=RL25hgfLd8Q)
* [Computational Drug Discovery: Machine Learning for Making Sense of Big Data in Drug Discovery](https://www.youtube.com/watch?v=uoVAd_zd-90)
* [Probing the origins of human acetylcholinesterase inhibition via QSAR modeling and molecular docking](https://peerj.com/articles/2322/)
* [Machine Learning for Drug Discovery (Explained in 2 minutes)](https://www.youtube.com/watch?v=xDMzOUUnNzw)
## 📝 License
[MIT License](./LICENSE)
## ©️ Credits

Huge thanks to Mr. [Chanin Nantasenamat](https://github.com/dataprofessor) for making this project possible through his clear explanation whether at the algorithmic level or at the domain-knowledge level 🙏
