# SKIN-CANCER-DIAGNOSIS-AND-DETECTION PAPER

Skin Cancer Diagnosis and Detection
Mr. Kota Venkateswara Rao.1*  , Pothabattula Usha. 2 , Gode Mary Nikhitha.2, Indupalli Sunanda.2
1 Professor , Department of Computer Science And Engineering, Andhra Loyola Institute of Engineering and Technology, Vijayawada, Andhra Pradesh, India.
2 Andhra Loyola Institute of Engineering and Technology, Vijayawada, Andhra Pradesh, India; 
*Corresponding Author’s email: siva278@gmail.com
      Abstract: Nowadays it is really very important to watch and analyze the cancer disease automatically at intervals in the first stages. Irregular streaks square measure one in every of the foremost very important features(included in most of dermoscopy algorithms) that show high association with carcinoma and basal cell malignant growth malady. The diagnostic test technique for the detection is most painful and harmful. So, we have a tendency to tend to square measure going for the machine - driven detection. Here we have a tendency to tend to square measure practice the GLCM choices for the detection, the choices of skin lesions square measure extracted normalized symmetrical grey Level Co-occurrence Matrices GLCM. GLCM based texture choices square measure extracted from each of the four classes and given as input to the Multi-class Support vector machine that’s utilized for classification purpose.
Keywords:Image Processing,GLCM technique,Gabor filtering,Support Vector Machine,Classification and Segmentation.

Introduction
At present Melanoma is dangerous and it is rapidly increasing skin cancer all over the World,as it spreads to lymph nodes rapidly,way before identifying the cancer. Early detection and diagnosis may cure melanoma completely.Skin cancer can be developed by tanning and by hereditary.Dermoscopy pictures of lesions are inspected carefully.There are many methods available that identify melanoma from benign using dermoscopic images.
The proposed framework detects cancer stage based on tumor thickness and yields improved results than existing systems.The main advantage of this proposed system is,it classifies the stage of cancer with higher accuracy that is we can detect the cancer cells in the skin and to which type does it belong,whether it is cancerous or Non-cancerous and the corresponding stage such as benign and malignant.Also gives the class of the skin cells which it belongs.
Literature Review
There are many methods to identify Melanoma.Melanoma needs to be classified at an early stage and start diagnosis of the patient at the earliest.There are many methods and techniques that classify melanoma and benign skin lesions. Many automatic systems exist which identify melanoma and benign skin lesions from dermoscopic images and using features of dermoscopic images.

•Melanoma skin cancer detection using various classifiers (Barata et al.) 2014.

•Computational methods for the image segmentation of pigmented skin lesions (Ma and Tavares) 2016.

•Early identification and aversion of melanoma (Abuzaghleh et al.) 2015.

•Identifying stage of melanoma cancer based on tumor thickness (Jaworek-Korjakowska et al.) Using Transfer Learning with VGG16 CNN   2017.
Research Methodology
Proposed Solution
Cancer image classification is an important task to generate classification maps as number of world observation cancer increasing day by day and this cancer contains different tools capable of capturing imagery time to time and utilized for a wide range of application.Thus,classification of cancer imagery has current area of researches and classification results can be used for different real-time application.This system proposed a novel approach for classification of six different classes actinic keratosis,Basal cell carcinoma,cherry nevus,dermatofibroma,Melanocytic nevus and Melanoma by utilizing Cancer imagery.To achieve an effective Cancer image classification framework this system isolates its works in various stage; these phases are important to give the better classification accuracy and the next page described these phases in details.

System Architecture

System design is the process or art of defining the architecture,components,modules,interfaces, and data for a system to satisfy specified requirements. One could see it as the application of systems theory to product development. There is some overlap and synergy with the disciplines of system analysis,systems architecture and systems engineering.
This defines the structure or behavior of the system.And it focuses on the mission forming a pattern.


Fig.System Architecture

Model and Algorithm
Image Preprocessing
Preprocessing of an image means “preparation” of the image to introduce it to an algorithm for specified task:tracking targets,recognition,feature extraction etc.It increases the signal-to-noise ratio and accentuates image features using custom or predefined filters.And it extracts meaningful information from images,such as finding shapes,counting objects,identifying colors,or measuring object properties.

Edge Detection
Identifying object boundaries in an image using pre-built algorithms includes Sobel,Prewitt,Roberts,Canny and Laplacian of Gaussian methods.
Fig. Edge Detection with MATLAB

Image Region Analysis
Calculates the properties of regions in images,such as area,centroid,and orientation.Use the image region analysis app to automatically count,sort,and remove regions based on properties(Image Region Analyzer App,Advanced Maneuvers with regionprops)

GLCM Technique

Gray Level Co-occurrence matrix is used to define over an image of co-occurring pixel values at a given offset to be the distribution.We use this for texture analysis with several applications specifically in medical analysis.

Gabor Filtering

Gabor filters are used in image processing for feature extraction,texture analysis and stereo disparity estimation.
Gabor filters will examine for specific content in the picture in some directions in a region around a point.

(1)Input Image A Cancer image is chosen for classification.
(2)Pre-processing(Contrast-Stretching,Noise Filtering)Noise Filtering is used to filter the unnecessary information and remove various types of noises from the images using the image processing toolbox.
(3)Apply Fuzzy C Means which is used for Image Segmentation and Clustering.
(4)Feature extraction using Gabor Filter: find the color of the user’s skin and use it as a threshold to binarize the image.
GLCM & Gabor Filter extracts feature vectors from input Cancer pictures like texture.Texture element is extracted from the RGB colored picture.The GLCM function characterize these texture feature of an image by calculating how often pairs of pixels with specific values and in a specified spatial relationship occur in an image and global color histograms in extricating the color features of Cancer pictures.Apart from the statistical features,we have extracted another feature i.e.,Area.
(5)Training and testing framework using SVM Support Vector Machine algorithm utilizes these element vectors(color and texture)to prepare and train our proposed structure.The features color and texture of each Cancer image are stored in database and these features will be used for the next stage of classification in light of these component vectors Color and Texture this proposed structure using SVM will group the Cancer pictures into various classes.For the effective classification of the image with images,various distance metrics are used to measure similarities of features.Here,similarity evaluation using SVM classifiers achieved between the features of the Query Image and the features of the database images.The SVM classifier will compute the feature value of input image and the feature value of database images,based on this value the SVM classifier will classify the input image belong to which class.
(6)Classified Image Input image is classified as either from the categories or other than these six categories and the type of the cancerous cells are detected by area by using thresholding technique.
 



Fig.Preprocessed Image 



Fig.Segmented Image

     		Fig.Real parts of Gabor Filters


    		Fig.Magnitudes of Gabor Filters



Results


Fig.MATLAB Interface


Fig.Uploading Files in MATLAB

Fig.Input Interface


Fig.Input dermoscopic images


		Fig.Output with its classification

Discussion

We all know that cancer is dangerous but can’t be cured if found out late.In this paper we have discussed how to identify cancer using Image Preprocessing,GLCM,Gabor filtering and SVM.If it is possible we can use 3D images in the future for better enhancement. As we are classifying of which cancer it is now,so we could also tell the percentage of disease that spreads in the body in coming days.And could possibly suggest nearest hospital and medicine.We could make online treatment plans and also could make it possible for people to consult hospitals with our suggestions.This could be improved in the future as we know technology is improving day by day. 

Conclusions
Cancer starts when our healthy cells change and are out of control,forming tumors. A Tumor can be either cancerous or benign. Melanoma skin cancer is very dangerous and gets metastasized very fast and spread to other body parts.It is required and important to identify the stage of cancer to start the diagnosis.Classification of the stages of dermoscopic images is considered one of the challenging tasks.Classification of the stages of cancer is a very tedious task and very important when the patient diagnosis is considered.This paper proposed non-invasive stage classification system of melanoma skin cancer.Skin cancer can be treated when treatment is done in before stages. Skin Cancer can be avoided by less exposure to the Sun,by using sunscreens and protective clothing.Skin cancer treatments are quite expensive and everyone needs to know and educate others on how to prevent skin cancer.
Acknowledgments
This research project was partially supported by the Department of Computer Science and Engineering, Andhra Loyola Institute of Engineering and Technology, Jawaharlal Nehru Technological University. We are grateful to Associate Professor Mr. K Venkateswara Rao for leading us to develop and contribute a paper to the conference.

References
Abuzaghleh,O.,Barkana,B.D.,Faezipour,M.,2015.Noninvasive real-time automated skin lesion analysis system for melanoma early detection and prevention s4300212 IEEE J.Transl.Eng.Health Med. 3,1-12. https://doi.org/10.1109/JTEHM.2015.2419612.
Barata,C.,Ruela,M.,Francisco,M.,Mendonca,T.,Marques,J.S.,2014.Two systems for the detection of melanomas in dermoscopy images using texture and color features.IEEE Syst. J., 965-979 Breslow , A., 1970. Thickness,cross-sectional areas and depth of invasion in the prognosis of cutaneous melanoma.
Ann.Surg. 172(5),902-908.Chim,H., Deng, X., 2010.Efficient phrase-based document similarity for clustering.IEEE Trans.Knowl. Data Eng. 20(9), 1217-1229.
Gong,A.,Yao,X.,Lin,W.,2020.Dermoscopy image classification based on StyleGANs and decision fusion. IEEE Access 8, 70640-70650. https://doi.org/10.1109/ACCESS.2020.2986916.
Reshma,M., Shan, B.P., 2017. Two methodologies for identification of stages and different types of melanoma detection, in: 2017 Conference on Emerging Devices and Smart Systems(ICEDSS), Tiruchengode, 2017, pp. 257-259, https://dx.doi.org/10.1109/ICEDSS.2017.8073689.
Rubegni,Pietro et al., 2010. Evaluation of cutaneous melanoma thickness by digital dermoscopy analysis:a retrospective study.Melanoma Res. 20,212-217.
Saez,Aurora,Sanchez-Monedero,Javier,Gutierrez,Pedro Antonio,Hervas-Martinez,Caesar,2016.Machine Learning methods for binary and multiclass classification of melanoma thickness from dermoscopic images.IEEE Trans.Med. Imaging 25, 1036-1045.
Sangve,S.M.,P
atil,R.R.,2014. Competitive analysis for the detection of melanomas in dermoscopy images IJERT 3(6), 351-354.Wang, X., Jiang, X., Ding, H., Liu, J.,2020. Bi-directional d.
Diwakar Gautam and Mushtaq Ahmed, “Melanoma Detection and Classification Using SVM Based Decision Support System”, INDICON, pp. 1-6,2015.
M. Elgamal, “Automatic Skin Cancer Images Classification”, Int. Journal of Advanced Computer Science and Applications, Vol. 4, pp. 287-294,2013.
Research on Computation of GLCM of Image Texture; BO Hua,MA Fu-long,JIAO Li-cheng,China.
Koh HK, Geller AC. Public health interventions for melanoma. Prevention, early detection, and education.Hematol Oncol Clin North Am.1998;12:903-28.
N Vikranth Kumar, P Vijeeth K Pramodh, Yepuganti Karuna, “Classification of Skin diseases using Image processing and SVM”, Vision Towards Emerging Trends in Communication and Networking (ViTECoN) 2019 International Conference on, pp. 1-5, 2019.
Reshma and Shan (2017) Total dermoscopic score to identify stage of melanoma. Using rgb2gray conversion and median filter to reduce noise.
