# Text and Multimedia Mining 20-21: Bird Predictions
This repository contains the Jupyter Notebook files used for my individual project for the course [Text and Multimedia Mining at Radboud University](https://www.ru.nl/courseguides/socsci/courses-osiris/ai/let-rema-lcex06-text-multimedia-mining/).
This README contains a short description for what happens in each of the .ipynb files, and a summary of the contents of the other files.
First however, the resources used within this project are listed:
* [Microsoft AI for Earth](https://www.microsoft.com/en-us/ai/ai-for-earth-tech-resources): The Species Classification API is trained to recognise over 5000 species. It can be used after requesting a key. The species classification in this project is done by this API.
* [Waarneming.nl](https://waarneming.nl/): Everyone can upload observations of any species seen in the Netherlands to this website. There is also an international version. The images used in this project were taken from this website.

Jupyter files:
* IdentificationWithAI4Earth.ipynb: Retrieves the image linked to a photo ID from Waarneming.nl and passes it on to the Species Classifier API and stores all the resulting predictions.
* ObtainBirdIDs.ipynb: Finds the ID of a list of bird species on Waarneming.nl.
* ObtainBirdImageIDs.ipynb: Requests a page of images from Waarneming.nl for every species in birdsForClassification.txt and stores the IDs of all the images.
* ResultAnalysis.ipynb: Generates a network graph from the Species Classifier API predictions and calculates its accuracy and makes some graphs of the relation between accuracy and other features of a species.

Other files:
* Accuracies.txt: Accuracy of the classification, rarity, number of annual observations and number of observed individuals of each of the species from BirdsForClassification.txt.
* BirdIDs.txt: List of the 298 bird species with their ID on Waarneming.nl.
* BirdInfo.txt: List of the 298 bird species that occur in the Netherlands according to Sovon in 2020.
* BirdInfo.xlsx: From [Sovon](https://www.sovon.nl/soorten), Excel file with all breeding and non-breeding birds in the Netherlands in 2020.
* BirdsForClassification.txt: Same as BirdIDs.txt, but only the subset of species that the Species Classifier API can recognise.
* BirdSpeciesNetwork.html: **Interactive network** of the predicted bird species. However, GitHub does not support viewing HTML files. Instead, do 'Run All' in ResultAnalysis.ipynb to view it.
* PhotoIDs.txt: Contains 24 IDs of a photo for each of the species from BirdsForClassification.txt. The images can be viewed on https://old.waarneming.nl/fotonew/$.jpg, where the $ should be replaced with an ID, for example https://old.waarneming.nl/fotonew/9/28774829.jpg.
* PredictedSpecies.txt: Contains the image ID, correct species, and the top-5 predictions of the Species Classifier API.
* SpeciesExampleImages.txt: A examplar image for each of the species from BirdsForClassification.txt, retrieved from the [Netherlands Biodiversity API](https://bioportal.naturalis.nl/api)
