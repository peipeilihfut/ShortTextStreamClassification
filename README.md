# ShortTextStreamClassification

					 
<DIV id="contentArea">
<DIV class="zone" id="mainZone">
<DIV class="compositeModule_1Zone ">
<DIV class="zone">
<DIV class="title deM"><B>Concept based Short Text Stream Classification with Topic Drifting Detection</B>
<DIV class="cl"></DIV></DIV>
<DIV class="conM ">
<P>&nbsp;</P>
<P>Short text stream classification is a very challenging
and significant task due to the characteristics of short
length, weak signal, high velocity and especial topic drift
in short text stream. However, this challenge has received
little attention from the research community. Motivated by
this, we propose a new feature extension approach for short
text stream classification using a large scale, general purpose
semantic network obtained from a web corpus. Our approach
is built on an incremental ensemble classification model. First,
in terms of the open semantic network, we introduce more
semantic contexts in short texts to make up of the data sparsity.
Meanwhile, we disambiguate terms by their semantics to
reduce the noisy impact. Second, to effectively track the hidden
topic drifts, we propose a concept cluster based topic drifting
detection method. Finally, extensive experiments demonstrate
our approach can detect topic drifts effectively compared to
several well-known concept drifting detection methods in data
stream. Meanwhile, our approach can perform best in the
classification of text data stream compared to several stateof-
the-art short text classification approaches.</P>
<H2>Introduction</H2>
<P>Short texts are prevalent on the Web, such as search
snippets and tweets. Unlike traditional normal texts such as
news articles, short texts refer to the length of the shorter
text form. For example, a tweet has a 140 character limit.
In recent years, these short texts swept the world at an
alarming rate, and have produced a large quantity of data
stream. We call them as short text streams. However, short
text stream classification is a very challenging task, owing
to the fact that these data have inherent defects such as short
length, weak signal and high ambiguity for each short text,
meanwhile, because of the explosive growth and popularity
of short textual content.</P>
<P>Given the characteristics of these short text streams, there
are several challenges with applying the traditional text
classification [1] to build models. This is because first, each
short text does not contain enough statistical signals to make
the analysis meaningful. Second, the limited contexts make
it more difficult to identify the senses of ambiguous words in
each short text. Third, they present the characteristics of data
streams as being continuous, high-volume, open-ended and
topic drifting in short texts. Meanwhile, existing short text classification approaches rarely focus on the characteristics
of data stream. It is hence a challenge for them in the
tackling of short text stream classification. To handle of the
short text classification, existing approaches mainly follow
two directions to enrich the short text. The first one is to
extend the feature space only using the rules or statistical
information hidden in the current short text contexts [2],
called the self-resource based approach. While the other is
to extend the feature space by external sources, called the
external resource based approach, and it can be divided into
four categories[3], [4], including link based approach [5],
Web search based approach [6], taxonomy based approach
[7] and topic based approach [8].</P>
<H2>Our Approach</H2>
<P>However, all of the aforementioned approaches are batch
algorithms, they are hence not suitable for short text stream
classification especially in the cases with topic drifts. Thus,
we propose a new feature extension approach for short text
stream classification using a large scale, general purpose
semantic network obtained from a web corpus. Our contributions
are as follows.</P>
<P>The main contributions of this paper are:</P>
<P>First, our approach produces higher
classification accuracy. We use an open semantic network
called Probase1 instead of other popular taxonomy knowledgebases
(such as Wikipedia) as the external resources. In
terms of the taxonomy in Probase, our approach introduces
more semantic contexts hidden in short texts to make up
of the data sparsity. Meanwhile, our approach seeks to
disambiguate terms in short texts and thus excludes noises
from irrelevant senses of terms. It is conducive to improve
the classification accuracy.</P>
<P>Second, our approach can detect
the topic drifts effectively. Contrary to the classificationerror
based concept drifting method, we use the concept
clusters of terms to represent the data distributions of each
chunk, and then compute the distance between concept
clusters to detect the topic drifts hidden in short text streams.</P>
<H2>Data Set </H2>
<P><A herf= "http://jwebpro.sourceforge.net/data-web-snippets.tar.gz" >Web Search Snippets</A>: Search snippets consists of three
parts: a URL, a short title and a short text description. The
search snippets were selected from the results of web search
transaction using predefined phrases of different domains.
There are eight categories with 12340 records.</P>
<P><A herf= "http://acube.di.unipi.it/tmn-dataset/" >News</A>:News is a dataset of 32K english news extracted from RSS
feeds of popular newspaper websites. It has seven categories.
Each news in the file has the structure of title, description
and category. We only extract titles as the data set here.</P>

<H2>Experiment Results</H2>
<P>Table 1 shows the benchmark data sets used in our experiments. 
<!--Due to the space limit, other experimental results are not shown here, you can get details from Download.-->
</P>
<P align="center"><B>Table 1: DATA SETS USED IN THE EXPERIMENTS</B></P>
<P>
<TABLE width="700" align="center" class=" borderColumns borderRows tableBorder" 
cellSpacing="0" cellPadding="0">
  <TBODY>
  <TR>
    <TD align="center"><B>domain</B></TD>
    <TD align="center"><B>#documents</B></TD>
    <TD align="center"><B>domain</B></TD>
    <TD align="center"><B>#documents</B></TD>
    </TR>
  <TR>
    <TD align="center" colspan="2">Web Search Snippets</TD>
    <TD align="center"colspan="2">News</TD>
</TD>
</TR>
<TR>
    <TD align="center">Business</TD>
    <TD align="center">1500</TD>
    <TD align="center">Sport</TD>
    <TD align="center">8190</TD>
</TR>
<TR>
    <TD align="center">Computer</TD>
    <TD align="center">1500</TD>
    <TD align="center">Business</TD>
    <TD align="center">5367</TD>
</TR>
<TR>
    <TD align="center">Culture-Arts-Ent</TD>
    <TD align="center">2210</TD>
    <TD align="center">U.S.</TD>
    <TD align="center">4783</TD>
</TR>
<TR>
    <TD align="center">Education-Science</TD>
    <TD align="center">2660</TD>
    <TD align="center">Health</TD>
    <TD align="center">1851</TD>
</TR>
<TR>
    <TD align="center">Engineering</TD>
    <TD align="center">370</TD>
    <TD align="center">Sci&amp;Tech</TD>
    <TD align="center">2872</TD>
</TR>
<TR>
    <TD align="center">Politics-Scienty</TD>
    <TD align="center">1500</TD>
    <TD align="center">Entertainment</TD>
    <TD align="center">3286</TD>
</TR>
<TR>
    <TD align="center">Health</TD>
    <TD align="center">1180</TD>
    <TD align="center">World</TD>
    <TD align="center">6255</TD>
</TR>
<TR>
    <TD align="center">Sport</TD>
    <TD align="center">1420</TD>
    <TD align="center">/</TD>
    <TD align="center">/</TD>
</TR>
<TR>
    <TD align="center">total</TD>
    <TD align="center">12340</TD>
    <TD align="center">total</TD>
    <TD align="center">32604</TD>
</TR>
  </TBODY></TABLE>
<P></P>

<DIV style="clear: both;"></DIV>
<DIV class="conM ">
<H2>Used Data Sets: Download</H2>
<P>More Details Refer to <A onclick="stc(this, 26)" href="http://121.42.218.45/peipeili/Used-Data-Sets-and-demo.rar" 
target="_new"> Used Data Sets</A>.</P></DIV>
<DIV style="clear: both;"></DIV>
<DIV class="conM ">
<H2>Source codes: Download</H2>
<P>More Details Refer to <A onclick="stc(this, 26)" href="http://121.42.218.45/peipeili/ShortTextClassification-src.rar" 
target="_new"> Source codes</A>.</P></DIV>
<DIV style="clear: both;"></DIV>
<DIV class="conM ">
<H2>References</H2>
<P>[1] K. Nigam, A. McCallum, S. Thrun, and T. Mitchell, “Text
classification from labeled and unlabeled documents using
em,” Machine learning, vol. 39, no. 2, pp. 103–134, 2000.</P>
<P>[2] X. Cheng, X. Yan, Y. Lan, and J. Guo, “Btm: Topic modeling
over short texts,” IEEE Transactions on Knowledge and Data
Engineering, vol. 26, pp. 2928–2941, 2014.</P>
<P>[3] M. Chen, X. Jin, and D. Shen, “Short text classification improved
by learning multi-granularity topics,” in Proceedings
of IJCAI’11, 2011, pp. 1776–1781.</P>
<P>[4] L. Gao, S. Zhou, and J. Guan, “Effectively classifying short
texts by structured sparse representation with dictionary filtering,”
Information Sciences, vol. 323, pp. 130–142, 2015.</P>
<P>[5] X. Wang, Y. Wang, W. Zuo, and G. Cai, “Exploring social
context for topic identification in short and noisy texts,” in
AAAI’15, 2015, pp. 1868–1874.</P>
<P>[6] D. Bollegala, Y. Matsuo, and M. Ishizuka, “A web search
engine-based approach to measure semantic similarity between
words,” IEEE TKDE, vol. 23, pp. 977–990, 2011.</P>
<P>[7] M. SHIRAKAWA, K. NAKAYAMA, T. HARA, and
S. NISHIO, “Wikipedia-based semantic similarity measurements
for noisy short texts using extended naive bayes,” IEEE
Transactions on Emerging Topics in Computing, vol. 3, pp.
205–219, 2015.</P>
<P>[8] X. Phan, C. Nguyen, D. Le, L. Nguyen, S. Horiguchi, and
Q. Ha, “A hidden topic-based framework toward building
applications with short web documents,” IEEE Transactions
on Knowledge and Data Engineering, vol. 23, pp. 961–976,
2011.</P>
</DIV>
<DIV class="conM ">
<H2>Contact</H2>
<P><A title="" style="zoom: 1;" onclick="stc(this, 30)" href="http://ci.hfut.edu.cn/index/teacherinfo/tid/522" 
target="_new" alt="">Peipei Li</A> (peipeili@hfut.edu.cn): Hefei University of Technology<BR>
<A title="" style="zoom: 1;" onclick="stc(this, 30)" href="http://haixun.olidu.com/" 
target="_new" alt="">Lu He</A> (luhe@mail.hfut.edu.cn): Hefei University of Technology <BR><A title="" style="zoom: 1;" onclick="stc(this, 29)" 
target="_new" alt="">Xuegang Hu</A> (jsjxhuxg@hfut.edu.cn): Hefei University of Technology<BR>
<A title="" style="zoom: 1;" onclick="stc(this, 30)" href="http://ci.hfut.edu.cn/index/teacherinfo/tid/477" 
target="_new" alt="">Yuhong Zhang</A> (zhangyuhong@hfut.edu.cn): Hefei University of Technology<BR>
<A title="" style="zoom: 1;" onclick="stc(this, 30)" href="http://ci.hfut.edu.cn/index/teacherinfo/tid/521" 
target="_new" alt="">Lei Li</A> (lilei@hfut.edu.cn): Hefei University of Technology<BR>
<A title="" style="zoom: 1;" onclick="stc(this, 30)" href="http://www.ucs.louisiana.edu/~xxw8007/" 
target="_new" alt="">Xindong Wu</A> (xwu@uvm.edu): University of Louisiana</P>
<P class="smallText"></P>
<P class="smallText">&nbsp;</P></DIV>
<DIV style="clear: both;"></DIV></DIV>
<DIV style="clear: left;"></DIV></DIV></DIV></DIV><!--NOINDEX_START-->					 
<DIV class="cl"></DIV>
<DIV class="bt" id="bGrad"></DIV></DIV></DIV>
			-->			 
<SCRIPT type="text/javascript">
				rmc.AE(window, "unload", rmc.PageDepth);
				rmc.AE(window, "scroll", rmc.MaxScroll);
			</SCRIPT>
		 </DIV><!--NOINDEX_STOP-->         <!-- this used to click count when feedback popup is clicked --> 
        <IMG id="clickCountImg" style="display: none;">	 
<SCRIPT type="text/javascript">
function stc(e,linkIndex){if(document.images){var linkText;if(navigator.appName.toLowerCase()=="microsoft internet explorer"){linkText=e.innerText}else{linkText=e.textContent}if(linkText==""){if(e.firstChild){var firstChild=e.firstChild.nodeName.toUpperCase();if(firstChild=="IMG"){linkText="Image: "+getName(e.firstChild.getAttribute('src'))}}else{var nodeName=e.nodeName.toUpperCase();if(nodeName=="AREA"){linkText="ImageMap: "+e.href}}}if(linkText==""){linkText=e.href}(new Image()).src="/a/i/stg.gif?f="+escape(document.location.href)+"&t="+escape(e.href)+"&i="+linkIndex+"&n="+escape(trimString(linkText))}}function getName(s){if(s.lastIndexOf('/')>=0){return(s.substring(s.lastIndexOf('/')+1,s.length))}else{return(s)}}function trimString(s){return(s.replace(/^\s*/,"").replace(/\s*$/,""))}
</SCRIPT>
 </DIV></BODY></HTML>


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

