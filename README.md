## 0. Check to files
```
hdfs dfs -ls /
```
```
hdfs dfs -ls /user
```
```
hdfs dfs -ls /user/train
```

## 1. Create new file

```
hdfs dfs -mkdir /user/train/hdfs_odev
```

## 2. Check the file
```
hdfs dfs -ls /user/train/
```

## 3. Dowland DataSets in local
```
wget https://raw.githubusercontent.com/erkansirin78/datasets/master/Wine.csv -O ~/datasets/Wine.csv
```

## 4. Check DataSets
```
ls -l ~/datasets/
```

## 5. Put DataSets from local to hdfs

```
hdfs dfs -put ~/datasets/Wine.csv /user/train/hdfs_odev
```

## 6. Check the dataset

```
hdfs dfs -ls  /user/train/hdfs_odev/Wine.csv
```

## 7. Look at the datasets

```
hdfs dfs -head  /user/train/hdfs_odev/Wine.csv
```

## 8. Create new file in temp
```
hdfs dfs -mkdir /tmp/hdfs_odev
```

## 9. Copies /user/train/hdfs_odev/Wine.csv` to `/tmp/hdfs_odev
```
hdfs dfs -cp /user/train/hdfs_odev/Wine.csv /tmp/hdfs_odev/Wine.csv
```


## 10. Check the datasets
```
hdfs dfs -ls /tmp/hdfs_odev/
```




