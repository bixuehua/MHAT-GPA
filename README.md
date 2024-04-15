# mHAT-GPA
A method for gene-phenotype association prediction by using multi-level heterogeneous graph attention network
### Dataset ###
<table>
    <tr>
        <th></th>
        <th>Gene Num</th>
        <th>HPO Num</th>
        <th>Disease Num</th>
        <th>G-H Num</th> 
        <th>G-D Num</th>
        <th>H-D Num</th>
        <th>Pos Num</th> 
        <th>Neg Num</th> 
	</tr>
    <tr>
        <td><p align="center">Fold 1</p></td> 
        <td><p align="center">4454</p></td> 
        <td><p align="center">8092</p></td>
        <td><p align="center">3567</p></td>
        <td><p align="center">144396</p></td>
        <td><p align="center">10713</p></td>
        <td><p align="center">113612</p></td>
        <td><p align="center">34283</p></td>
        <td><p align="center">34283</p></td>
   </tr>
    <tr>
  		<td><p align="center">Fold 2</p></td> 
        <td><p align="center">4454</p></td> 
        <td><p align="center">8092</p></td>
        <td><p align="center">3567</p></td>
        <td><p align="center">144240</p></td>
        <td><p align="center">10713</p></td>
        <td><p align="center">113612</p></td>
        <td><p align="center">34439</p></td>
        <td><p align="center">34439</p></td>
    </tr>
    <tr>
        <td><p align="center">Fold 3</p></td> 
        <td><p align="center">4454</p></td> 
        <td><p align="center">8092</p></td>
        <td><p align="center">3567</p></td>
        <td><p align="center">144727</p></td>
        <td><p align="center">10713</p></td>
        <td><p align="center">113612</p></td>
        <td><p align="center">33952</p></td>
        <td><p align="center">33952</p></td> 
    </tr>
    <tr>
        <td><p align="center">Fold 4</p></td> 
        <td><p align="center">4454</p></td> 
        <td><p align="center">8092</p></td>
        <td><p align="center">3567</p></td>
        <td><p align="center">144112</p></td>
        <td><p align="center">10713</p></td>
        <td><p align="center">113612</p></td>
        <td><p align="center">34567</p></td>
        <td><p align="center">34567</p></td> 
    </tr>
    <tr>
        <td><p align="center">Fold 5</p></td> 
        <td><p align="center">4454</p></td> 
        <td><p align="center">8092</p></td>
        <td><p align="center">3567</p></td>
        <td><p align="center">144211</p></td>
        <td><p align="center">10713</p></td>
        <td><p align="center">113612</p></td>
        <td><p align="center">34468</p></td>
        <td><p align="center">34468</p></td> 
    </tr>
</table>

### Data description ###
#### feature
* gene_pac_feature_512.npy: Genetic characteristics after PCA treatment.
* hpo_pac_feature_512.npy: Phenotypic characteristics after PCA treatment.
* disease_pac_feature_512.npy: Disease characteristics after PCA treatment.
#### fold1~fold5
* edge_train1~5.plk: Heterogeneous network adjacency matrix.
* train_sample1~5.json: Training set samples.
* test_sample1~5.json: Test set samples.
#### Similarity_matrix
* adj_dd: Disease similarity matrix.
* adj_gg: Gene similarity matrix
* adj_hh: Phenotypic similarity matrix

### Run Step ###
  Run run_main.py to train the model and obtain the predicted results of gene phenotype association.

### Requirements ###
  - python==3.6.13
  - pytorch==1.10.1
  - scipy==1.5.2
  - scikit-learn==0.21.3
  - numpy==1.19.2
  - pandas==1.1.5




