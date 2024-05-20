# Medical-conditions-observation-in-scientific-computing-analysis
Electrocardiogram (ECG) is the process of producing a recording of the heart's electrical activity through repeated cardiac cycles. An ECG is visualized as a graph of voltage versus time. The voltage is the electrical activity of the heart measured by placing electrodes on the skin.¶
Python has a built-in ECG dataset
from scipy.misc import electrocardiogram
Sampling rate is 360 Hz ecg = electrocardiogram()
• Unfortunately, this patient has patterns of unusual heart beats.
• For reference, the time period 9 seconds to 10.2 seconds is a set of normal heart activity.
• From 46.5 seconds to 50 seconds the ECG shows what doctors call premature ventricular contractions.
• Time period 207 seconds to 215 seconds show significant abnormal activity.
We will find out FFT and spectrograms to be used to help diagnose heart conditions. Specifically, we will compute FFT and spectrograms for the three time periods above as well as the entire time period to observe conditions.
