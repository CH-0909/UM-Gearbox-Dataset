# UM-Gearbox-Dataset
This dataset was provided by Dr. Hao Chen from Prof. Yang Zhixin's team at the University of Macau.

The dataset contains multi-sensor monitoring data for gears and bearings, and the data acquisition experiments were accomplished on two experimental platforms named Test Rig A and Test Rig B, respectively.

**==================== TEST RIG A ====================**
Test Rig A is driven by a motor and the transmission system comprises a planetary gearbox and a parallel gearbox. The fault components include the sun gear G1 in the planetary gearbox, the gear G2 on the second stage drive shaft in the parallel gearbox, and the bearing B1 of the second stage drive shaft. At the other end of the system is a magnetic brake. 

**The following faulty parts are used on Test Rig A：**

1-Gear G1 contains the four faults of broken teeth (CT), missing teeth (MT), root chipping (RC), and surface wear (SF). 

2-Gear G2 contains the four faults of Broken Tooth (CT), Missing Tooth (MT), Root Chip (RC) and Surface Wear (SF) and the aggravation of these four faults, i.e., Heavy Broken Tooth (HCT), Heavy Missing Tooth (HMT), Heavy Root Chip (HRC) and Heavy Surface Wear (HSF).

3-Bearing B1 contains three types of faults: inner race fault (IR), outer race fault (OR), and ball fault (B).

**The experimental setup was as follows：**

The motor input speeds were set to 600, 1200, 1800 rpm, and the brake damping (i.e., load) was set to 0-4 L. The experiments on Test Bench A were fault tests on three components, with 180 single fault types, in addition to a variety of mixed fault types, with 192 G1-G2 mixed faults, 72 G1-B1 mixed faults, 96 G2-B1 mixed faults, and 144 G1-G2-B1 mixed faults. 144 types, and 96 types of G1-G2-B1 mixed faults. Two acceleration sensors were mounted on the test bench A. The sensors had a sampling frequency of 25.0%. The sampling frequency of the sensors was 25.6 kHz. The duration of collected data was approximately 3600 seconds for each type.

**The data file format is described as follows：**

The data from Test Rig A is stored in 7 folders for single fault, double fault and triple fault cases. The data are stored in .mat format files, and the naming scheme for single-fault data is “<component name>-<status name>\_<RPM>\_<load>\_<time>.mat”, and the naming scheme for multiple-fault type is “<component name 1><status name 1>-<component name 2><state name 2>\_<RPM>\_<Load>\_<Time>.mat”. Each data file contains two matrices, ”data_recorded“and “data_rectime”, where the size of the “data_recorded” matrix is L\*3, L means the length of signals, the first column is the axial sensor signal, the second column is the radial sensor signal. The third column is the speed encoder signal. The size of "data_recorded” is L\*3, which is the time-stamp of the corresponding data.
![test_rig_A](https://github.com/CH-0909/UM-Gearbox-Dataset/blob/main/images/test_rig_A.jpg)


**==================== TEST RIG B ====================**
Test Rig B contains a planetary gearbox and three parallel gearboxes. The same faulty components are used on Test Rig B as on Test Rig A (G2 contains only normal level faults).
![test_rig_B.jpg](https://github.com/CH-0909/UM-Gearbox-Dataset/blob/main/images/test_rig_B.jpg)

**The experimental setup was as follows：**

Test Rig B was set up with no load and speed settings of 600, 1200 and 1800 rpm. The experiments on Test Rig B collected single faults data including 36 classes ; two-compound faults data including 48 classes per case (G1-B1, G1-G2, and G2-B1) for a total of 144 types; and three-compound faults G1-G2-B1 including 36 calsses. 11 sensors were installed on Test Rig B, including five acceleration sensors, two current sensors, one microphone, one torque sensor and two homemade sensors. The sampling frequency of the torque sensor and the homemade sensors was 25.6 kHz, while the other sensors were sampled at 51.2 kHz. The length of the data collected was approximately 900 seconds.
![sensor_channels.jpg](https://github.com/CH-0909/UM-Gearbox-Dataset/blob/main/images/sensor_channels.jpg)

**The data file format is described as follows：**

The data from Test Rig B is stored as .mat format files in 1 folder for a total of 219 files. The single fault data is named as “<component name><status name>\_<RPM>\_<load>.mat” and the multiple fault data is named as “<component name 1>-<component name 2>\_<status name 1>-<status name 2>\_<RPM>\_ <load>.mat” and “<component name 1>-<component name 2>-<component name 3>\_<status name 1>-<status name 2>-<status name 3>\_<RPM>\_ <load>.mat”. Each data file contains three data matrices, “Data1”, “Data2” and “Statistics”, of which the size of the “Data1” matrix is L\*8, 8 columns of data correspond to sensors 3,4,5,6,1,2,7,8 in turn; the size of the “Data2” matrix is L\*3, 3 columns of data correspond to sensors 9,10,11 in turn; the size of the “Statistics”  is 11\*120\*4, means that the 11 channel signals (Data1 and Data2 are totally consists of 11 channels) are divided into 120 slices to calculate the statistics, including: peak-to-peak value, root mean square (RMS), kurtosis, and frequency center of gravity.

**==================== Dataset Download ====================**
This dataset can be downloaded through two channels：\\
<1> NAS system of our group （Suggested for overseas users）\\
Link: http://QuickConnect.to/Smart5001\\
Account: DatasetAtESWA\\
Password: Smart2025\\
File Station -> DatasetAtESWA -> please download the data you want!\\

<2> A data backup link on Baidu.com disk\\
Test Rig A Dataset: https://pan.baidu.com/s/1SHAE6HzOd3mmMPHQcOD6zA?pwd=v3tt      password: v3tt\\
Test Rig B Dataset: https://pan.baidu.com/s/1rOezeU2fnMv1p-mE-4qSWA?pwd=977k      password: 977k \\


