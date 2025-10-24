# ContinuousAI
This repository contains models and evaluation datasets for ContinuousAI.

## Setup and Usage Instructions

### 1. Install TTool  
First, install **TTool** from [https://ttool.telecom-paris.fr](https://ttool.telecom-paris.fr).  
The recommended method is to download and compile it from its public GitLab repository:  
[https://gitlab.telecom-paris.fr/mbe-tools/TTool](https://gitlab.telecom-paris.fr/mbe-tools/TTool).  
Detailed installation and configuration instructions are available here:  
[https://ttool.telecom-paris.fr/installation.html](https://ttool.telecom-paris.fr/installation.html)

---

### 2. Configure TTool-AI  
Once TTool is installed, configure **TTool-AI** as described here:  
[https://ttool.telecom-paris.fr/ttoolai.html](https://ttool.telecom-paris.fr/ttoolai.html).  
You will need either an **OpenAI** or **MistralAI** API key, or a locally hosted LLM.

---

### 3. Run TTool and Select the AI Model  
Launch TTool, then open or create a model.  
In the menu **AI > Set AI Model**, select the LLM you want ContinuousAI to use.

---

### 4. Compute AI Suggestions  
To generate suggestions, you can:  
- Click **AI > Compute Suggestions with AI**, or  
- Right-click a model element in the design panel and choose **Compute a new suggestion with AI**.
  
Depending on the selected interaction mechanism (configurable in the **AI** menu), suggestions can also be triggered when you:  
- Hover your mouse pointer over a model component for 2 seconds, or  
- Modify the model directly.

You can also, by right-clicking on computed suggestions in the left panel, request the refreshing or the refinement of a (set of) suggestion(s).


## Content of the Repository

### `./models`  
This directory contains models that you can use as a basis to compute suggestions.  
For intellectual property reasons, we have not uploaded the full dataset used in our evaluation. However, we provide a model of a ship's stabilization system and its specification, inspired by Fincantieri public documentation:  
[https://www.fincantieri.com/globalassets/prodotti-servizi/sistemi-e-componenti/sistemi-e-componenti-navali/fin-stabilizers_mp-03-14.pdf](https://www.fincantieri.com/globalassets/prodotti-servizi/sistemi-e-componenti/sistemi-e-componenti-navali/fin-stabilizers_mp-03-14.pdf).  

The model also includes two lists of suggestions computed by ContinuousAI.

### `./evaluationData`  
This directory contains our full evaluation results, including all suggestions provided by ContinuousAI.
