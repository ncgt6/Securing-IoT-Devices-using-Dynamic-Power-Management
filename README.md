# Securing-IoT-Devices-Using-Dynamic-Power-Management
This repository includes details about dataset used for developing a ML based malware detector using DVFS signatures on Android OS platform. The dataset comprises of DVFS states time-series of benign applications selected from android benchmarks, MiBench Test Suite and malware applications selected from DREBIN dataset.

# Benign Dataset

/benign_dataset/benigns.tar.gz

This includes the DVFS signatures of 23 android benchmark applications. There are 100 traces of each application and each trace has 40000 time samples. The size of the dataset is (23,100,40000). The length of time-series of each trace is 40000, 0-20000 corresponds to time-series of energy-efficient core(Core1), and 20000-40000 comprises of time-series of high-performance core(Core2).

/benign_dataset/benigns_MiBench.tar.gz

This includes the DVFS signatures of 10 benign benchmarks selected from MiBench suite. There are 14 traces per benchmark and each trace has 40000 time-samples. The size of the dataset is (10,14,40000).

# Malware Dataset

/malware_dataset/malwares.tar.gz

This includes the DVFS signatures of 21 malware applications, each selected from different malware family, 100 traces per application and each trace has 40000 time-samples. The size of dataset is (21,100,40000). 

/malware_dataset/malwares_unknown.tar.gz

This includes 146 malware applications which variants of malware family in malware.tar.gz dataset. There is only 1 trace per application, 40000 time-samples per trace. The size of dataset is (146,40000). This dataset is used to test the trained model on out-of-distribution test examples, which corrsponds to unknown malware applications, unseen by trained ML model. 


The details on generating training and testing dataset is included in the paper.
https://ieeexplore.ieee.org/document/9186163
