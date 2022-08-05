# 🗒️ Graph Datasets
A list of graph datasets for machine learning and network science projects. Mostly dedicated to Graph Neural Networks. :)

##### Contents   

1. [Node classification](#node-classification)
2. [Node regression](#node-regression)

## Node classification

### Zachary's karate club

These are data collected from the members of a university karate club by Wayne Zachary. Zachary (1977) used these data and an information flow model of network conflict resolution to explain the split-up of this group following disputes among the members.

| **Nodes** | **Edges** | **Features** | **Classes** |
|:---:|:---:|:---:|:---:|
| 34 | 156 | 0 or 34 | 2 or 4 |

#### Links
* [File](http://vlado.fmf.uni-lj.si/pub/networks/data/Ucinet/UciData.htm)
* [NetworkX](https://networkx.org/documentation/stable/auto_examples/graph/plot_karate_club.htm)
* [PyTorch Geometric](https://pytorch-geometric.readthedocs.io/en/latest/modules/datasets.html#torch_geometric.datasets.KarateClub)

#### Citing
```
@article{10.2307/3629752,
         ISSN = {00917710},
         URL = {http://www.jstor.org/stable/3629752},
         author = {Wayne W. Zachary},
         journal = {Journal of Anthropological Research},
         number = {4},
         pages = {452--473},
         publisher = {[University of New Mexico, University of Chicago Press]},
         title = {An Information Flow Model for Conflict and Fission in Small Groups},
         urldate = {2022-08-05},
         volume = {33},
         year = {1977}
}
```

### Cora

The Cora dataset consists of 2708 scientific publications classified into one of seven classes. The citation network consists of 5429 links. Each publication in the dataset is described by a 0/1-valued word vector indicating the absence/presence of the corresponding word from the dictionary. The dictionary consists of 1433 unique words.

| **Nodes** | **Edges** | **Features** | **Classes** |
|:---:|:---:|:---:|:---:|
| 2,708 | 10,556 | 1,433 | 7 |

#### Links
* [File](https://linqs.org/datasets/#cora)
* [Papers With Code](https://paperswithcode.com/dataset/cora)
* [PyTorch Geometric](https://pytorch-geometric.readthedocs.io/en/latest/modules/datasets.html#torch_geometric.datasets.Planetoid)
* [DGL](https://docs.dgl.ai/generated/dgl.data.CoraGraphDataset.html#dgl.data.CoraGraphDataset)
* [Spektral](https://graphneural.network/datasets/#citation)

#### Citing
```
@article{sen:aim08,
         title = {Collective Classification in Network Data},
         author = {Prithviraj Sen, Galileo Mark Namata, Mustafa Bilgic, Lise Getoor, Brian Gallagher, and Tina Eliassi-Rad},
         journal = {AI Magazine},
         year = {2008},
         publisher = {AAAI},
         pages = {93--106},
         volume = {29},
         number = {3},
}
```

### CiteSeer

The CiteSeer dataset consists of 3312 scientific publications classified into one of six classes. The citation network consists of 4732 links. Each publication in the dataset is described by a 0/1-valued word vector indicating the absence/presence of the corresponding word from the dictionary. The dictionary consists of 3703 unique words.

| **Nodes** | **Edges** | **Features** | **Classes** |
|:---:|:---:|:---:|:---:|
| 3,327 | 9,104 | 3,703 | 6 |

#### Links
* [File](https://linqs.org/datasets/#citeseer-doc-classification)
* [Papers With Code](https://paperswithcode.com/dataset/citeseer)
* [PyTorch Geometric](https://pytorch-geometric.readthedocs.io/en/latest/modules/datasets.html#torch_geometric.datasets.Planetoid)
* [DGL](https://docs.dgl.ai/generated/dgl.data.CiteseerGraphDataset.html#dgl.data.CiteseerGraphDataset)
* [Spektral](https://graphneural.network/datasets/#citation)

#### Citing
```
@conference{rossi:aaai15,
            title = {The Network Data Repository with Interactive Graph Analytics and Visualization},
            author = {Ryan Rossi and Nesreen Ahmed},
            booktitle = {AAAI Conference on Artificial Intelligence},
            year = {2015},
            publisher = {AAAI},
            pages = {4292--4293},
            volume = {29},
            address = {New York, NY, USA},
}
```

### PubMed

The Pubmed dataset consists of 19717 scientific publications from PubMed database pertaining to diabetes classified into one of three classes. The citation network consists of 44338 links. Each publication in the dataset is described by a TF/IDF weighted word vector from a dictionary which consists of 500 unique words.

| **Nodes** | **Edges** | **Features** | **Classes** |
|:---:|:---:|:---:|:---:|
| 19,717 | 88,648 | 500 | 3 |

#### Links
* [File](https://linqs.org/datasets/#pubmed-diabetes)
* [Papers With Code](https://paperswithcode.com/dataset/pubmed)
* [PyTorch Geometric](https://pytorch-geometric.readthedocs.io/en/latest/modules/datasets.html#torch_geometric.datasets.Planetoid)
* [DGL](https://docs.dgl.ai/generated/dgl.data.PubmedGraphDataset.html#dgl.data.PubmedGraphDataset)
* [Spektral](https://graphneural.network/datasets/#citation)
* [HuggingFace](https://huggingface.co/datasets/pubmed)

#### Citing
```
@conference{namata:mlg12,
            title = {Query-Driven Active Surveying for Collective Classification},
            author = {Galileo Mark Namata, Ben London, Lise Getoor, and Bert Huang},
            booktitle = {International Workshop on Mining and Learning with Graphs},
            year = {2012},
            publisher = {MLG},
            address = {Edinburgh, Scotland},
}
```

### Facebook Page-Page

This webgraph is a page-page graph of verified Facebook sites. Nodes represent official Facebook pages while the links are mutual likes between sites. Node features are extracted from the site descriptions that the page owners created to summarize the purpose of the site. This graph was collected through the Facebook Graph API in November 2017 and restricted to pages from 4 categories which are defined by Facebook. These categories are: politicians, governmental organizations, television shows and companies. The task related to this dataset is multi-class node classification for the 4 site categories.

| **Nodes** | **Edges** | **Features** | **Classes** |
|:---:|:---:|:---:|:---:|
| 22,470 | 171,002 | 128 | 4 |

#### Links
* [File](http://snap.stanford.edu/data/facebook-large-page-page-network.html)
* [Papers With Code](https://paperswithcode.com/dataset/facebook-page-page)
* [PyTorch Geometric](https://pytorch-geometric.readthedocs.io/en/latest/modules/datasets.html#torch_geometric.datasets.FacebookPagePage)

#### Citing
```
@misc{rozemberczki2019multiscale,
      title={Multi-scale Attributed Node Embedding},
      author={Benedek Rozemberczki and Carl Allen and Rik Sarkar},
      year={2019},
      eprint={1909.13021},
      archivePrefix={arXiv},
      primaryClass={cs.LG}
}
```
## Node regression

### Wikipedia Network

The data was collected from the English Wikipedia (December 2018). These datasets represent page-page networks on specific topics (chameleons, crocodiles and squirrels). Nodes represent articles and edges are mutual links between them. The presence of a feature in the feature list means that an informative noun appeared in the text of the Wikipedia article. The target csv contains the node identifiers and the average monthly traffic between October 2017 and November 2018 for each page. The goal is to predict the log average monthly traffic of December 2018. PyTorch Geometric has a node classification variant of this dataset, where the goal is to predict the correct bin.

| **Name** | **Nodes** | **Edges** | **Features** | **Classes** |
|:---|:---:|:---:|:---:|:---:|
| Chameleon | 2,277 | 31,421 | 2,325 | Continuous |
| Crocodile | 11,631 | 170,918 | 2,325 | Continuous |
| Squirrel | 5,201 | 198,493 | 2,325 | Continuous |

#### Links
* [File](https://snap.stanford.edu/data/wikipedia-article-networks.html)
* [PyTorch Geometric](https://pytorch-geometric.readthedocs.io/en/latest/modules/datasets.html#torch_geometric.datasets.WikipediaNetwork)

#### Citing
```
@misc{rozemberczki2019multiscale,
      title={Multi-scale Attributed Node Embedding},
      author={Benedek Rozemberczki and Carl Allen and Rik Sarkar},
      year={2019},
      eprint={1909.13021},
      archivePrefix={arXiv},
      primaryClass={cs.LG}
}
```
