🧠 Machine Learning – Product Category Classification

📌 Περιγραφή  
Αυτό το notebook υλοποιεί ένα μοντέλο Μηχανικής Μάθησης που προβλέπει την κατηγορία ενός προϊόντος με βάση τον τίτλο του. Χρησιμοποιείται το dataset **“PriceRunner Product Classification and Categorization”** από το Kaggle, κατάλληλο για πρόβλημα ταξινόμησης πολλαπλών κατηγοριών (multi-class classification).

👤 Ονοματεπώνυμο & ΑΜ  
Ονοματεπώνυμο: Μαρία Χαριλάου  
Αριθμός Μητρώου (ΑΜ): 20238534

🔍 Περιγραφή Μοντέλου  
Χρησιμοποιήθηκε ο αλγόριθμος **Random Forest Classifier** για την πρόβλεψη της κατηγορίας του προϊόντος βάσει του τίτλου του.

Κατηγορίες προϊόντων:
- Mobile Phones
- CPUs
- Dishwashers
- TVs
- Microwaves
- Washing Machines
- Fridge Freezers
- Digital Cameras
- Fridges
- Freezers

📊 Βασικά Χαρακτηριστικά:
- Τύπος προβλήματος: Multi-class Classification
- Train/Test split: 80/20
- Vectorization: TF-IDF σε τίτλο προϊόντος
- Μετρικές αξιολόγησης: Accuracy, Precision, Recall
- Χρήση Label Encoding για τις κατηγορίες

🧪 Βήματα Εκπαίδευσης
1. **EDA & Visualization**: Εξετάστηκε η κατανομή των προϊόντων ανά κατηγορία.
2. **Προεπεξεργασία Κειμένου**: Εφαρμόστηκε TF-IDF στο πεδίο `product_title_raw`.
3. **Label Encoding**: Οι κατηγορίες κωδικοποιήθηκαν αριθμητικά.
4. **Εκπαίδευση Μοντέλου**: RandomForestClassifier σε training set.
5. **Αξιολόγηση**: Με classification report και confusion matrix.

✅ Περιεχόμενο Notebook:

| Απαίτηση                              | Status |
|--------------------------------------|--------|
| Εισαγωγή dataset από Kaggle          | ✅ `pricerunner_aggregate.csv` |
| EDA (κατανομή κατηγοριών)            | ✅ `value_counts()` + `countplot` |
| Encoding κατηγορικών                 | ✅ `LabelEncoder()` στον στόχο |
| Δημιουργία target                    | ✅ `product_category` |
| TF-IDF vectorization για input       | ✅ Κειμενική μετατροπή |
| Train/Test split                     | ✅ 80/20 |
| Εκπαίδευση με RandomForest           | ✅ |
| Classification report               | ✅ Accuracy, Precision, Recall |
| Confusion Matrix                     | ✅ |
| Σαφής ροή και καθαρότητα notebook    | ✅ |

▶️ Οδηγίες Εκτέλεσης  
Ανοίξτε το αρχείο:  
`ML_Model_Product_Classification.ipynb` μέσω **Google Colab** ή **Jupyter Notebook**.

Εκτελέστε βήμα-βήμα:

1. Εισάγετε το αρχείο `pricerunner_aggregate.csv`
2. Τρέξτε την εξερεύνηση (EDA) και την προεπεξεργασία
3. Εκπαιδεύστε το μοντέλο
4. Αξιολογήστε το με classification metrics

📦 Απαιτούμενες Βιβλιοθήκες:

- pandas  
- sklearn  
- seaborn  
- matplotlib  

Εάν εργάζεστε τοπικά:

```bash
pip install pandas scikit-learn seaborn matplotlib
```
