# Recommender System using NMF

This project implements a simple **Recommender System** using **Non-negative Matrix Factorization (NMF)**.  
It demonstrates how to decompose a user-item rating matrix into latent factors and generate recommendations.  
Additionally, it includes functionality to find similar items using **cosine similarity**.

---

## 📂 Project Structure
- **Recommender_System_using_NMF.ipynb** → Jupyter Notebook version of the project.  
- **recommender_system_using_nmf.py** → Python script version of the project.  

---

## 🚀 Features
- **Matrix Factorization with NMF**  
  Factorizes the user-item rating matrix into:
  - `W`: Item-feature matrix  
  - `H`: Feature-user matrix  

- **User Recommendations**  
  Predicts the most relevant items for a given user.  

- **Item Similarity Search**  
  Finds items similar to a target item using **cosine similarity**.  

- **Specific Item Recommendation**  
  Recommends the single best item for a given user.  

---

## 📊 Example Workflow
1. **Synthetic dataset** is created with users as columns and items as rows.  
2. **NMF** is applied to decompose the dataset into latent factors.  
3. Recommendations are computed by multiplying `W` and `H`.  
4. Similar items are retrieved for a target item.  
5. A specific item is recommended for a user.

---

## 🛠 Installation
Make sure you have Python 3.8+ installed.  
Install the required dependencies:
```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

---

## ▶️ Usage
Run the Python script:
```bash
python recommender_system_using_nmf.py
```

Or open the Jupyter Notebook:
```bash
jupyter notebook Recommender_System_using_NMF.ipynb
```

---

## 📌 Example Output
- **Recommendations for a User**
```
Recommendation for User1:
        Recommendation
Item3          2.45
Item1          1.78
Item5          1.21
...
```

- **Similar Items**
```
Similar items to 'Item1':
    Item  Similarity
0  Item4    0.892134
1  Item3    0.754332
2  Item2    0.645211
```

- **Specific Recommended Item**
```
Recommended specific value for User1: Item3
```

---

## 📖 References
- [Scikit-learn: NMF](https://scikit-learn.org/stable/modules/generated/sklearn.decomposition.NMF.html)  
- [Recommender Systems Introduction](https://en.wikipedia.org/wiki/Recommender_system)
