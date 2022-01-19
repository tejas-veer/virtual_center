Background
==========
This section discusses the algorithms, data, problems, tools, educational material, feature 
engineering, and the emerging areas related to machine learning in Earth sciences. These have 
been summarized in the mind map, depicted in Figure 1, taking the case of weather and climate 
sciences as an example.

Machine learning algorithms for ESS
++++++++++++++++++++++++++++++++++++++++
Various algorithms which have shown remarkable performance in computer vision, natural 
language processing, and reinforcement learning etc can be directly applied to the problems of 
ESS. For example, the super-resolution methodology (SRCNN, DeepSD) developed by Dong et 
al. (2015)
8
to enhance the resolution of image datasets has been used to downscale the precipitation 
datasets from coarser resolution to a high resolution9,10
. Seasonable forecast of various aspects of 
monsoon has been studied using single and stacked encoder-based techniques11,12
. Prediction of 
solar irradiance using CNN with added attention has been used12. Recent advances in the computer 
vision community show that algorithms such as SRGAN, LapSRN, FSRGAN, and UNET 
outperform the standard SRCNN. Long short-term memory (LSTM) networks, sequence to 
sequence networks, and the recent attention-based Transformer models have improved the 
accuracies in natural language processing. Some of these algorithms have also been used or can 
5
be applied to the time series forecasting problems in ESS. For example a survey on these 
applications can be found in Lim and co-authors13 . Weather and climate data are so massive that 
it is not even encountered by the community working on big data. The spatio-temporal nature of 
the datasets, i.e., three-dimensional fields at each temporal dimension, makes it a complex problem 
to solve. The patterns in this four-dimensional data cannot be deciphered manually, and machine 
learning offers the perfect opportunity. Models that have shown good performance on video 
datasets such as ConvLSTM can be used to build large-scale deep learning-based systems which 
can predict the information in high spatial and temporal resolutions14,15
. Sequence-to-sequence and
LSTM has been used to predict and forecast active-break cycles of Indian monsoon16
. Before 
starting any analysis, traditional algorithms such as random forests, support vector machines and 
multivariate linear regression should be the first goto methods. EnhanceNeT and PSPNet are 
algorithms which can be used for classification of objects in images and spatially locating them. 
They have shown excellent results in computer vision applications. They can be used for problems 
such as the identification of floods from satellite imagery.

ESS datasets
___________________
The understanding of ESS datasets is most important while developing machine learning models. 
These datasets primarily come in three classes, viz the observational data, reanalysis product
combination of model data and observation created in a consistent manner) , dynamical model 
simulated outputs (such as climate change data from models) . For the South Asian domain, longperiod ground-based observations from the India Meteorological Department (IMD) are available. 
These datasets can now be obtained from https://dsp.imdpune.gov.in. Satellite- based products are 
available from the Tropical Rainfall Measuring Mission (TRMM), Landsat, Sentinel and MODIS. 
Reanalysis products are gridded products and are very useful for the fields which are/cannot be 
measure directly by instruments. They offer insights into the information which is nearest to 
reality. Various reanalysis products are available for the South Asian region, such as 
(i) IMDAA reanalysis, 
(ii) NCEP/NCAR reanalysis, 
(iii) CAMS reanalysis, 
(iv) ERA5 reanalysis, 
(v) MERRA-2 reanalysis and
(vi) JRA55 reanalysis. 
As regards model products are considered, various model products such as TIGGE, 
CMIP5/CMIP6, and Seasonal to sub-seasonal (S2S) hindcasts are available. The model outputs 
are based on the integrations of partial differential equations based on dynamical systems. Machine 
learning offers an innovative methodology to improve these dynamical model estimates by 
combining them with observed or reanalysis products. The archive of seismic waveform data, 
Global Positioning System (GPS) data, oceanographic and other geoscience datasets in the country 
are increasing exponentially every year, calling for fast and efficient processing and dissemination 
of information to the public service systems. 

Research problems in ESS
______________________________
6
South Asia is home to more than two billion inhabitants and is heavily dependent on the natural 
climate variability for livelihood. For example, the Indian monsoon feeds agricultural lands over 
the region, thus directly impacting the region's economic well-being. Monsoon is a complex multiscale problem and is nonlinear and hence linear methods cannot unravel the real processes
especially the feedback processes leading to its variability. Forecasts at various temporal scales 
such as short to medium range (1-10 days), extended range (2-3 weeks), seasonal scale (for coming 
season) and climate scale (100s year) are important for planning hydrological resources over the 
region. It has been known that the crop yields are dependent on the meteorological variables;
machine learning can be used to accurately forecast the spatial crop yield a season in advance and 
economically benefit the society. The demographics in the South Asian region have considerably 
changed in the past decades and many people now live in the cities.
Moreover, the population density in these areas is very high. Hence, locally accurate urban 
forecasts are need of the hour. These locations are also sources of chemical species which are 
harmful for the environment and all living beings. Hence air pollution prediction is an important 
problem. Identifying localities with higher air pollution is also essential for city planning, for 
example, deciding the number of electric buses by the city authorities. Machine learning-based 
algorithms can be used to improve the cyclone forecasts of dynamical models. Extreme weather
events such as heat waves and cloud bursts are causing havoc in recent times, as it is challenging 
to predict them accurately. In seismology, AI/ML techniques are being tried out for earthquake 
detection, phase-picking (measurement of arrival times of distinct seismic phases), event 
classification, earthquake early warning, ground motion prediction, tomography and earthquake 
geodesy.

Popular tools to perform machine learning for ESS
_______________________________________________________
The availability of open-source software packages has provided a bridge to the domain experts to 
avoid reinventing the wheel while applying machine learning to their problems. Python is the most 
popular language for machine learning, and various libraries such as TensorFlow, PyTorch, 
Theano, mxnet, OpenCV, Keras, and others are available freely. Visualization software such as 
TensorBoard and Tableau assist in communicating the results from machine learning models. In 
addition to the software requirements, deep learning needs Graphical Processing Units (GPUs) to 
perform the tensor computations in neural networks. Tensor Processing Units (TPUs) are a step 
ahead of GPUs wherein the neural network is encoded on the chip to perform fast calculations. 
The TPUs are only available over the cloud, and every individual can't buy a personal GPU for 
deep learning. Hence, free and paid cloud computing services, such as Amazon Web Services 
(AWS), Microsoft Azure, Google Cloud Platform (GCP), Paperspace, Digital Ocean, Google 
Earth Engine provide an option to build machines over the cloud to perform deep learning and 
conduct analysis in climate science17. A step further, the concept of Jupyter notebooks as a service 
has become popular and there are several frees as well as paid vendors providing notebook as a 
service. Notable amongst them include the free services provided by Kaggle, Google Colab and 
others. More cloud vendors can be found at https://github.com/binga/cloud-gpus, 
https://github.com/zszazi/Deep-learning-in-cloud, https://github.com/discdiver/deep-learning-
7
cloud-providers/blob/master/list.md and others actively maintained. “Docker containers” have 
also become an important part of the ecosystem helping deploy end-to-end packages for deep 
learning. 

Educational materials to learn machine learning for ESS
_____________________________________________________________
A key component in the machine learning cycle is the educational resources to build knowledge 
and apply it to Earth and climate science. The avenues to learn data science and hence use machine 
learning for Earth science applications are the Coursera specializations, courses, professional 
certificates, Udacity nanodegrees, Udemy courses and other free and paid material available as 
MOOCs. The Development of Skilled Manpower in Earth System Sciences (DESK) at the 
Ministry of Earth Sciences (MoES), Government of India regularly holds training programs to 
train young researchers on machine learning applications in in Earth sciences. One such training 
workshop was conducted in 2021 and the details can be found at 
https://www.youtube.com/watch?v=2cQmhDgFinQ&list=PLgQCKqNw6z_CMKiKoWMAukvo
8vyEe1KLb

Decision making for machine learning in ESS
__________________________________________________
After the weather/hydrological forecasts have been generated, they have to be used to take
decisions for the benefit of society. Deep reinforcement learning is an excellent methodology for 
this purpose. State of the art algorithms such as deep q networks, vanilla policy gradient, trust 
region policy optimization, proximal policy optimization, deep deterministic policy gradient 
(DDPG), soft actor critic, twin delayed DDPG and others can be used to train agents which can 
guide in decision making. The most crucial aspect of deep reinforcement learning is the design 
of the environment, action(s), and reward(s). The decision-making can be used for disaster 
preparedness/mitigation, hydrological planning, and other associated tasks.

Feature engineering for machine learning in ESS
_________________________________________________________
Feature engineering is the generation of meaningful predictors or parameters to improve the 
performance of a machine learning model. It is performed after cleaning the data and preparing it 
in a format that can train statistical models. It has been noted that removing redundant variables 
improves the performance of machine learning systems. Various methods can be used to find the 
most valuable predictors some of them are: Principal Component Analysis (PCA), Empirical 
Orthogonal Functions (EOF), and Independent Component Analysis (ICA). Binning, counts, 
transforms or filtering can be used to extract the predictive signal from data to improve the models. 
Unsupervised learning techniques such as autoencoder can also assists in finding valuable 
predictors from raw datasets. The deep learning-based models are, however, coded for imagebased input datasets. To overcome this limitation, strategies such as transforming the spherical
global data to a cubed sphere or tangent planes mapping can effectively reduce spherical distortions 
in the data.
8

Emerging areas in machine learning for ESS
_______________________________________________
While the previous decade has seen the hype of deep learning overshadow other machine learning 
methodologies, there are numerous emerging and innovative machine learning methods which can 
be used for ESS. Graph machine learning is training neural networks on graphs and is becoming 
increasingly popular. Complex networks and recurrence plots come in the category of nonlinear 
methodologies and come in handy for specific applications. One major concern while using 
machine learning for the physical sciences is that these models are known as black box models. 
Interpretable machine learning aims to address this concern and analysis of deep learning model 
weights reveal the patterns learned. Ongoing active research is happening in this area, and it is 
crucial for the increasing acceptability of deep learning models at the production scale in ESS. The 
emerging fields of augmented reality, virtual reality, improved remote sensing measurements, 
crowd-sourcing and drone technology offer excellent potential to advance the observation data 
collection and improve machine learning models. 
