# ShortTextStreamClassification
Concept based Short Text Stream Classification with Topic Drifting Detection

All benchmark data sets are used in our experiments below. 
Web search Snippets: http://jwebpro.sourceforge.net/data-web-snippets.tar.gz
News: http://acube.di.unipi.it/tmn-dataset/

How to use our source codes?
1. The solution is built on Visual Studio 2010 C# plateform.
2. The main function is in the project of LibSVMSharp.Examples.Classification
Train using SVM classifier and implement the concept drifting detection, namely the function of TrainAndDriftDetectAndTest is called in the main function.
All parameter settings are below. （You can use the default values in the parameter settings).
 /// <summary>
 /// Training by SVMClassifier over data chunks and concept drfiting detection
        /// </summary>
        /// <param name="thresOfWin">thresOfWin: the threshold of the size of window (data chunk), default: 0.5</param>
        /// <param name="parameter">parameter: the parameters of SVM training</param>
        /// <param name="modelMaxNum">modelMaxNum: the size limit of ensembling models</param>
        /// <param name="thresOfWin">thresOfWin: the threshold of window</param>
        /// <param name="slidWinSize">sildWinSize: the size of the sliding window,default: 2000</param>
        /// <param name="maxW">maxW: the maximum size of the sliding window, default: 1000</param>
        /// <param name="minW">minW: the minmum size of the sliding window, default: 200</param>
        /// <param name="srcTextOfAllTerms">srcTextOfAllTerms: the directory of reading all terms including the dominant clusters for entities</param>
        /// <param name="srcTextOfDC">srcTextOfDC: the directory of reading the dominant clusters for entities</param>
        /// <param name="srcTextOfVSM">srcTextOfVSM: the directory of reading the feature space for classifier generation, the file can be "CVSM" or "WCVSM"</param>
        /// <param name="chunkSize">chunkSize: the chunk size in the concept drifting detecton</param>
        /// <param name="labelPos">labelPos: the postition of labels, default: 0 (at the begining) </param>
        /// <param name="basicAlg">basicAlg: the basic algorithm, default: "SVM" </param>
        /// <param name="fadingFactor">fadingFactor: the value of fading factor, eg., 0.995</param>
        /// <param name="estimatorType">estimatorType: prequential error estimator in sliding window/uing fading factor</param>
        /// <param name="serverName">serverName: the server name, default: "LPP-PC" </param>
        /// <param name="dataSrc">dataSrc: the database name, default: "corev52" </param>
        /// <param name="bUseSynonym">bUseSynonym: whether it uses the synonym data or not, default value: false </param>
        /// <returns></returns>
		
3. in the folder of demo, we give an example to show how to run our executable file.
the batch file:  F:\shortTextData\News\train+test\title\allData titleAll.ReOrgConcept200.termRecog-tfidf.VSMWithCluster titleAll.ReOrgConcept200.termRecog-tfidf.dominantCluster titleAll.ReOrgConcept200.termRecog-tfidf.SVSM 50 0 false 0.75 cosine KNN 1000 0.85 prequentialByFading 0

In order to run this batch file, you need the following prepared data:
(1) titleAll.ReOrgConcept200.termRecog-tfidf.VSMWithCluster 
(2) titleAll.ReOrgConcept200.termRecog-tfidf.dominantCluster
(3) titleAll.ReOrgConcept200.termRecog-tfidf.SVSM
These data can be obtained by the funtions in the project of "ConceptualizationTerms"
a) step 1: term recognition, namely call the funtion RecognizeTerms() in the main function;
b) step 2: generate vector space model for texts with term recognition, namely call the funtion GenVSM() in the main function;
b) step 3: Disambiguation, namely call the funtion DisambiguateTerms() in the main function; 
More details refer to examples in the main function  of "ConceptualizationTerms" project.

In this batch file, description of input parameters is below:
string directory = args[0]; //the path directory: F:\shortTextData\News\train+test\title\allData
string srcTextOfAllTerms = args[1]; // source data with term recognition
string srcTextOfDC = args[2]; // source data with dominant senses
string srcTextOfVSM = args[3]; //source data with vectorization using senses
int chunkSize = Convert.ToInt32(args[4]);//data chunk, default '200'; 
int labelPos = Convert.ToInt32(args[5]);//the label position given the training data, default: at the beginig, namely '0';
bool labelUnKnown = Convert.ToBoolean(args[6]);//whether the label is known or not, defualt: known, namely 'false', if unknown, use 'true' 
double thresInitCenter = Convert.ToDouble(args[7]);//the threshold used in the concept cluster based topic drifting detection, default: '0.5'
string distEvalType = args[8];//the similarity function, default: cosine
string basicAlg = args[9];//the prediction function, default: "KNN"
Int64 slidWinSize = Convert.ToInt64(args[10]);//the window size
double drifThres = Convert.ToDouble(args[11]);//the threshold used in the topic drifting detection, if the distance between clusters is larger than this threshold, drift is considered.
string estimatorType = args[12]; //the type of topic drifting detection, using prequential prediction by sliding window or by fading factor
double fadingFactor = 0;
if (estimatorType == "prequentialByFading")//in the topic drifting detection, if you select the prequential test by fading factor, it is necessary to set the value of fading factor.
    fadingFactor = Convert.ToDouble(args[13]);

