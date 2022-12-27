# anomaly_detection_bosch_milling
Anomaly detection is conducted on sequential data on an heavily operated industrial equiment - CNC Milling Machine. 

Computer Numerical Control (CNC) machines are the pioneer of assembly lines for any manufacturing industry. Self-regulated
fabrication plants which use CNC for milling, demand the equipment to operate at high-speed resisting unfavourable environmental
factors despite task complexities. However, the breakdown of such
equipment can cause a domino effect in delivering the targets and
unplanned maintenance costs. It becomes crucial to identify the
reasons causing the machine failure and recognize the peculiar traits
before the actual malfunction. 

A model is proposed using a stacking
ensemble of neural networks known as Convolutional Autoencoders
which competently detects an abnormality in the series of vibrations. Using the reconstructive property of AutoEncoder, multiple
AutoEncoders are tuned individually as sub-models on normal and
anomalous data and feature space is regenerated. Feature predictions from each estimator are fed to a supervised meta-learner build
using a dense neural network which classifies the signal as faulty and
not faulty. The CNC Milling data which is used in the experiment is
very recent and no benchmark models have been published. Thus,
in order to prepare some baseline, two more models are build using classic machine learning algorithm Fast Fourier Transform and
decision-tree based approach Isolation Forrest. 
We have compared
the proposed model with other two using standard performance evaluation metrics and successfully achieved better results for anomaly
detection
