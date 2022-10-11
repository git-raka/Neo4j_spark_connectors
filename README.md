# SPARK-INSTALL
Download spark packages from apache archive
```
 wget https://archive.apache.org/dist/spark/spark-2.4.5/spark-2.4.5-bin-hadoop2.7.tgz
```

### Extract packages
```
tar -xvf spark-2.4.5-bin-hadoop2.7.tgz
```
### Rename directory spark-2.4.5 to spark
```
 mv spark-2.4.5-bin-hadoop2.7 spark
```
### add environtment spark to basrc/profile
```
sudo nano .bashrc
```
```
export SPARK_HOME=/home/ddi/spark
export PATH=$PATH:$SPARK_HOME/bin:$SPARK_HOME/sbin
export PYSPARK_PYTHON=/usr/bin/python3
```


### Start master spark
<img width="763" alt="image" src="https://user-images.githubusercontent.com/77326619/195049033-373372f7-493c-4c5c-a819-4fddb823316d.png">


```
start-master.sh
```

### Start slave spark
<img width="766" alt="image" src="https://user-images.githubusercontent.com/77326619/195049141-4c3188c0-59a7-4ff7-bd01-236ecfdc6498.png">

```
start-slave.sh spark://ddi-spark:7077
```

### open spark-shell
```
spark-shell
```
<img width="666" alt="image" src="https://user-images.githubusercontent.com/77326619/195049621-a60088b7-6658-4314-929e-7cc4ec6e10e7.png">


