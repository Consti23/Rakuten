# **Challenge_Rakuten_py**

## Präsentation und Installation
Dieses Projekt ist Teil der Herausforderung "Rakuten France Multimodal Product Data Classification". Ziel ist es, den Produkttyp-Code (wie er im Katalog von Rakuten France definiert ist) anhand einer Textbeschreibung und eines Bildes vorherzusagen.

Rakuten France möchte in der Lage sein, seine Produkte automatisch anhand der Bezeichnung, Beschreibung und Bilder der auf seiner Website verkauften Produkte zu kategorisieren.

Dieses Projekt wurde im Rahmen unserer Data Scientist-Ausbildung mit dem Ausbildungszentrum Datascientest entwickelt. (https://datascientest.com/)

Unser Projektentwicklungsteam bestand aus:
  * Flavien SAUX ([GitHub](https://github.com/Flav63s) / [LinkedIn](https://www.linkedin.com/in/flavien-s-712596190/))
  * Chadi BOULOS ([GitHub](https://github.com/Chadiboulos) / [LinkedIn](https://www.linkedin.com/in/chadi-boulos-6b05aa2a/))
  * Constantin NZWESSA ([GitHub](https://github.com/Consti23) / [LinkedIn](https://www.linkedin.com/in/constantin-nzwessa-322121250/))
  * Michaël DEVAUX ([GitHub](https://github.com/MichaelD24) / [LinkedIn](https://www.linkedin.com/in/michaël-devaux-362760139/))

## Projektverlauf
Das Projekt folgte einem mehrstufigen Plan :

* Datensammlung, -aufbereitung, erste Exploration, statistische und visuelle Analysen.
* Modellierung verschiedener grundlegender Textklassifikationsalgorithmen wie Linear SVC, Random Forest, Gradient Boost.
* Modellierung grundlegender logistischer Regressionsalgorithmen für die Bildklassifikation.
* Modellierung von Deep-Learning-Algorithmen mit TensorFlow:
  * Convolutional Neural Networks (CNN: Mobilenet, Lenet, Resnet50) zur Bildklassifikation,
  * Recurrent Neural Networks (RNN: LSTM, BERT) zur Textklassifikation.
* Fusionsmodell: Kombination eines Textmodells (BERT) und eines Bildmodells (Resnet50).
* Mögliche Weiterentwicklungen des Modells.
  
## **README**

Wir konnten die benötigten Daten nicht auf GitHub hochladen, damit Sie dieses Projekt unter den gleichen Bedingungen wie wir nachbilden können.
Diese waren zu umfangreich, um in unserem Speicherplatz untergebracht zu werden. Sie können sie jedoch auf der Website herunterladen. [challengedata](https://challengedata.ens.fr/challenges/35).
Nach der Registrierung können Sie auf die 4 Dateien zugreifen, die die Daten umfassen:
* X_train_update.csv
* X_test_update.csv
* Y_train_CVw08PX.csv
* Der Ordner, der alle Bilder enthält


## Streamlit App

**Installation de Streamlit.**
```
pip install -r requirements.txt
```
Pour exécuter l'application (attention aux chemins des fichiers dans l'application) :

```shell
conda create --name my-awesome-streamlit python=3.9
conda activate my-awesome-streamlit
pip install -r requirements.txt
streamlit run app.py
```

The app should then be available at [localhost:8501](http://localhost:8501).
