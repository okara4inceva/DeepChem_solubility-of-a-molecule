# DeepChem_solubility-of-a-molecule

DeepChem
MLP model that uses a python based AI system to find a suitable candidate in drug discovery
RdKit
RDKit is an open-source toolkit for cheminformatics and molecular modeling. It provides a wide range of functions and algorithms to work with chemical structures, perform chemical calculations, and analyze chemical data.
#dataset delaney 
The Delaney (ESOL) dataset a regression dataset containing structures and water solubility data for 1128 compounds. The dataset is widely used to validate machine learning models on estimating solubility directly from molecular structures (as encoded in SMILES strings).

Scaffold splitting is recommended for this dataset.

The raw data csv file contains columns below:

“Compound ID” - Name of the compound

“smiles” - SMILES representation of the molecular structure

“measured log solubility in mols per litre” - Log-scale water solubility
of the compound, used as label

Parameters
featurizer (Featurizer or str) – the featurizer to use for processing the data. Alternatively you can pass one of the names from dc.molnet.featurizers as a shortcut.

splitter (Splitter or str) – the splitter to use for splitting the data into training, validation, and test sets. Alternatively you can pass one of the names from dc.molnet.splitters as a shortcut. If this is None, all the data will be included in a single dataset.

transformers (list of TransformerGenerators or strings) – the Transformers to apply to the data. Each one is specified by a TransformerGenerator or, as a shortcut, one of the names from dc.molnet.transformers.

reload (bool) – if True, the first call for a particular featurizer and splitter will cache the datasets to disk, and subsequent calls will reload the cached datasets.

data_dir (str) – a directory to save the raw data in

save_dir (str) – a directory to save the dataset in
https://deepchem.readthedocs.io/en/latest/api_reference/moleculenet.html#delaney-datasets
