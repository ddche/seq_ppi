## Multifaceted Protein-Protein Interaction Prediction Based on Siamese Residual RCNN
check pull and push orders.
i want to change files. second
This is the repository for PIPR (originally Lasagna in our previous preprint version). This repository contains the source code and links to some datasets used in our paper.

Environment:

    python 2.7 or 3.6
    Tensorflow 1.7 (with GPU support)
    CuDNN
    Keras 2.2.4
    
./binary contains the implementation for the binary prediction task. This includes scripts to run on three datasets: Yeast, Human and multi-species.    
./type contains that for the interaction type prediction task.  
./regression contains that for the binding affinity prediction task. 
Each folder is attached with a **run.sh** to show how to run the evaluation program.  
./embeddings contains pre-trained amino acid embeddings and the training script.  

## Datasets

Here we include altogether 6 datasets. New datasets processed in this work are marked *ND*.  
1. The Yeast dataset for binary PPI prediction provided in [Guo et al. 2008](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC2396404/).  
2. The *multi-species dataset (C. elegans, D. melanogaster and E. coli)* extracted from DIP for binary PPI prediction. (*ND*)  
3. Added another binary PPI prediction dataset from [Pan et el. 2010](https://www.ncbi.nlm.nih.gov/pubmed/20698572) under the folder *sun*.  
4. The SHS27k dataset for interaction type prediction can be downloaded from [here](http://yellowstone.cs.ucla.edu/~muhao/pipr/SHS_ppi_beta.zip) or from the [Google Drive](https://drive.google.com/open?id=1y_5gje6AofqjrkMPY58XUdKgDuu1mZCh). (*ND*)  
5. The larger SHS148k dataset for interaction type prediction can be found in the links above. (*ND*)  
6. Link to the normalized SKEMPI dataset is [here](http://yellowstone.cs.ucla.edu/~muhao/pipr/SKEMPI_all_dg_avg_(PIPR).zip).  

## Reference
This work has been published in the Bioinformatics journal featuring ISMB/ECCB 2019.

DOI: http://dx.doi.org/10.1093/bioinformatics/btz328  
Bibtex:

    @article{chen2019pipr,
        title={Multifaceted Protein-Protein Interaction Prediction Based on Siamese Residual RCNN},
        author={Chen, Muhao and Ju, Chelsea and Zhou, Guangyu and Chen, Xuelu and Zhang, Tianran and Chang, Kai-Wei and Zaniolo, Carlo and Wang, Wei},
        journal={Bioinformatics},
        volume = {35},
        number = {14},
        pages = {i305-i314},
        year = {2019},
        month = {07},
        publisher={Oxford University Press}
    }
  
## MuPIPR (NAR GaB 2020)
Also check out the follow up work in the NAR Genom. Bioinform. paper [Mutation effect estimation on protein–protein interactions using deep contextualized representation learning](https://academic.oup.com/nargab/article/2/2/lqaa015/5781175), in which a *pre-trained neural language model* helps the PIPR architecture to help estimate the point mutation effect in PPI.  
The released software is available at [guangyu-zhou/MuPIPR](https://github.com/guangyu-zhou/MuPIPR).
