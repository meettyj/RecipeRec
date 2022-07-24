# RecipeRec
This is the official repo for the IJCAI'22 paper "[RecipeRec: A Heterogeneous Graph Learning Model for Recipe Recommendation](https://arxiv.org/pdf/2205.14005.pdf)".

## Data
Please first [download the data](https://drive.google.com/drive/folders/1DvjFUa9gGqalrFAYFzbB2onGXU2K4LNu?usp=sharing), then put them under folder 'data/'.

For the mappings between the nodes in URI-Graph and the recipe text (recipes_weighted_and_USDAmapped.json) or user ID, please check the following code block:
```
recipeID2nodeID_dict, nodeID2recipeID_dict = torch.load('../data/recipeID2nodeID_and_nodeID2recipeID.pt')
ingreID2nodeID_dict, nodeID2ingreID_dict = torch.load('../data/ingre2nodeID_and_nodeID2ingre.pt')
userID2userNodeID_dict, userNodeID2userID_dict = torch.load('../data/userID2userNodeID_and_userNodeID2userID.pt')
```

## Code
All codes have been put into a jupyter notebook for easy reading and executing. We further log the results in the notebook for demonstration purposes. 

## Citing RecipeRec
If you find RecipeRec useful, please cite our paper.
```
@inproceedings{RecipeRec,
  author = {Tian, Yijun and Zhang, Chuxu and Guo, Zhichun and Huang, Chao and Metoyer, Ronald and Chawla, Nitesh V.},
  title = {RecipeRec: A Heterogeneous Graph Learning Model for Recipe Recommendation},
  booktitle = {IJCAI},
  year = {2022}
}
```
