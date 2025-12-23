\# PROIECT-MADDM (Movies) - Preprocessing, Clustering, Classification (Global vs CIEL), Visualization



Acest proiect analizeaza un dataset de filme (movies\_metadata.csv) si implementeaza un pipeline complet:

1\) curatare si preprocesare date,

2\) clustering (zone/grupuri de filme),

3\) clasificare (modele globale + metoda CIEL cu experti locali),

4\) vizualizari interactive cu Plotly/Dash (ROI si analize derivate).



\## Structura proiectului



\- `1\_Preprocessing.ipynb`  

&nbsp; Curata dataset-ul si face conversii (numeric/date), trateaza valori lipsa/outlieri si salveaza un fisier curatat (ex: `cleaned\_movies\_metadata.xlsx`).



\- `2\_Clustering.ipynb`  

&nbsp; Creeaza clustere pe baza feature-urilor (ex: non-financiare / financiare, in functie de implementare). Rezultatul este folosit ulterior in clasificare.



\- `3\_Classification.ipynb`  

&nbsp; Testeaza clasificatori globali (ex: Decision Tree / SVM / Random Forest / Gradient Boosting) si compara cu metoda CIEL:

&nbsp; - Input clustering (KMeans)

&nbsp; - antrenare experti locali (cate un model per cluster)

&nbsp; - predictie pe baza clusterului (hard assignment)

&nbsp; - raportare metrici (Accuracy, F1 macro, Cohen's Kappa)



\- `5\_Visualization.ipynb`  

&nbsp; Rapoarte interactive cu Plotly/Dash, inclusiv grafice pentru ROI (profit/buget) si agregari (ex: ROI mediu in functie de rating, harta ROI mediu pe tari).



\## Date de intrare



Dataset: `movies\_metadata.csv` (ex: Kaggle / TMDB metadata).  

Fisierul trebuie sa fie in root-ul proiectului (sau actualizezi calea in notebook-uri).





