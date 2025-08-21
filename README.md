# Smartphone Sensor Fusion for Joint Recognition of Human Activity and Behavioral Context

This repository contains the Python code for an approach accepted in the journal *Computing*:  
**“Smartphone Sensor Fusion for Joint Recognition of Human Activity and Behavioral Context”**
<img width="877" height="567" alt="{F0EB6AD2-AD5E-4258-A209-5441BF98B8B1}" src="https://github.com/user-attachments/assets/93931679-5667-43a5-a298-2470b38c1bfe" />

---

## Repository Contents

The project includes **three Jupyter notebooks** with the associated results:

### 1. `01-feature_extraction_extrasensory_5s_10s_20s.ipynb`
- Feature extraction on the **ExtraSensory** dataset.  
- Three time windows are used: **5s, 10s, and 20s**.  
- Integrates **information fusion** across different smartphone sensors.  

#### Usage Instructions
1. Navigate to the directory containing the **raw ExtraSensory dataset**.  
2. Modify the **`folder`** variable to point to the `accelerometer` folder (it should contain 60 files, one per user).  
3. Verify and update all paths in the notebook.  
4. Run the notebook.  

⚠️ **Important**:  
- Download the **raw ExtraSensory data** (not preprocessed data) from [http://extrasensory.ucsd.edu/](http://extrasensory.ucsd.edu/).  
- Required files:
  - Accelerometer measurements  
  - Audio measurements  
  - Absolute location  
  - Features and labels  
- If you add other files, you must **adapt the code accordingly**.  

---

### 2. `02-label_mapping_multiclass_extrasensory.ipynb`
- Preprocessing and **label mapping** for each time window (5s, 10s, 20s).  
- Create three folders (`5s`, `10s`, `20s`) and update their paths in the code via:  

```python
os.chdir(r"your/path")
```
---
### 3. `03-ProposedApproach_classification.ipynb`

This notebook presents results obtained using the **ETR (Extremely Randomized Trees)** algorithm.

You can modify and test the notebook with other classification algorithms.

---

## Citation

If you use this code, please cite:

**Hocine Attoumi, Achour Achroufene, Redouane Saifi, Lydia Souici, Djamila Boukredera**.  
*Smartphone Sensor Fusion for Joint Recognition of Human Activity and Behavioral Context*.  
Accepted for publication in **Computing (2025)**.

BibTeX format:

```bibtex
@article{attoumi2025smartphone,
  title={Smartphone Sensor Fusion for Joint Recognition of Human Activity and Behavioral Context},
  author={Hocine, Attoumi and Achour, Achroufene and Redouane, Saifi and Lydia Souici and Djamila Boukredera},
  journal={Computing},
  year={2025},
  note={Accepted for publication}
}
```

