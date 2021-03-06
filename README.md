# Minerals-image-classification

## Convolutional Neural Network (CNN) on minerals image dataset ([Kaggle dataset](https://www.kaggle.com/asiedubrempong/minerals-identification-dataset))
### We have 6 Minerals/classes
* muscovite: is a hydrated phyllosilicate mineral of aluminium and potassium with formula KAl2(AlSi3O10)(F,OH)2, or (KF)2(Al2O3)3(SiO2)6(H2O). Muscovite is the most common mica, found in granites, pegmatites, gneisses, and schists, and as a contact metamorphic rock or as a secondary mineral resulting from the alteration of topaz, feldspar, kyanite.
* chrysocolla: is a hydrated copper phyllosilicate mineral with formula: Cu2−xAlx(H2−xSi2O5)(OH)4·nH2O (x<1)[1] or (Cu,Al)2H2Si2O5(OH)4·nH2O. Associated minerals are quartz, limonite, azurite, malachite, cuprite, and other secondary copper minerals.
* quartz: is a hard, crystalline mineral composed of silicon and oxygen atoms. Quartz is a defining constituent of granite and other felsic igneous rocks. It is very common in sedimentary rocks such as sandstone and shale. It is a common constituent of schist, gneiss, quartzite and other metamorphic rocks.
* bornite: is a sulfide mineral with chemical composition Cu5FeS4. Bornite is an important copper ore mineral and occurs widely in porphyry copper deposits along with the more common chalcopyrite.
pyrite: is an iron sulfide with the chemical formula FeS2 (iron(II) disulfide).
* malachite: is a copper carbonate hydroxide mineral, with the formula Cu2CO3 (OH)2. Malachite often results from the weathering of copper ores, and is often found with azurite (Cu3(CO3)2(OH)2), goethite, and calcite.
* biotite: Biotite is a common group of phyllosilicate minerals within the mica group with the approximate chemical formula K(Mg,Fe)3AlSi3O10(F,OH)2.

## Read the data and create label/image list

![Load Data](/loadData.PNG)

## Data preparation
![Load Data](/dataPrep.PNG)

## Splitting train/test dataset - 80% train 20% test
![Load Data](/split.PNG)

### We have 744 training samples and 186 test samples
![Load Data](/dimData.PNG)

# Define the model
## Hyperparameters 
* Filters: the numbers of kernels that we choose for the convolutional layer to learn.
* Kernel size: the size of a convolutional filter. The height and width of the 2D convolution window.
* Padding: Padding is a process of adding zeros to the input matrix symmetrically. ([source](https://towardsdatascience.com/covolutional-neural-network-cb0883dd6529))
* Activation function:  is a mathematical equation that determine the output of a neural network.
![Load Data](/modelDef.PNG)

## Data Augementation
Image data augmentation is a technique that can be used to artificially expand the size of a training dataset by creating modified versions of images in the dataset.
![Load Data](/dataAug.PNG)

## ReduceLROnPlateau
Reduce learning rate when a metric has stopped improving
![Load Data](/reduceLR.PNG)

## Compile the model
![Load Data](/modelCom.PNG)

## Fit the model
![Load Data](/fitModel.PNG)

## Plot
![Load Data](/plotModel.PNG)

## Model predictions and test images 
![Load Data](/minPred1.PNG)

![Load Data](/minPred2.PNG)
