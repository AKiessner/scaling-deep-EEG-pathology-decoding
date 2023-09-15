
# Indices for sampling smaller subsets

indices can be used to load a smaller subset, indicies refer to inidices stated in the data description file

```

with open("./indices/TUAB-Random/indices_seed0_TUAB-Random_trainsize_100.pkl", 'rb') as f:
         ids_to_load_train = pickle.load(f) 


task_name = 'TUAB_subset_' + str(subset_size)

whole_train_set = load_concat_dataset(train_folder, preload=False, ids_to_load=ids_to_load_train)


```
