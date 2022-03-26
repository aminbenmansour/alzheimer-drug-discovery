# 🧬 🧪 Alzheimer-drug-discovery

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

## ⁉️ Frequently Asked Questions (FAQ)
🙋
👉
## 📑 References
## ©️ Credits

Huge thanks to mr. [Chanin Nantasenamat](https://github.com/dataprofessor) for making this project possible through his clear explanation whether at the algorithmic level or at the domain-knowledge level 🙏
