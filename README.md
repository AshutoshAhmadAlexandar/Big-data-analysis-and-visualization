# Big-data-analysis-and-visualization

OVERVIEW:
In this lab, we will expand our skills in data exploration developed in Lab1 and enhance them by adding big data analytics and visualization skills. This document describes Lab2: Data Aggregation, Big Data Analysis and Visualization, involves (i) data aggregation from more than one source using the APIs (Application programming interface) exposed by data sources, (ii) Applying classical big data analytic method of MapReduce to the unstructured data collected, and (iii) building a visualization data product.
We will leverage the data collection and exploratory data analysis skills developed in Lab1 to accomplish the goals of Lab2.

LEARNING OUTCOMES:
 Automate data collection from multiple sources using the APIs offered by the businesses
 Explain the importance of evaluating the reliability of data (for example: social media vs news
media)
 Apply classical big data analytical methods: MapReduce for word count and related family of
algorithms
 Work on Hadoop 2.x, and HDFS and process the data using big data algorithms
 Learn a high level language-based data analysis by exploring Python as data processing language
 Apply modern visualization methods and disseminate results using the web/mobile interface

OBJECTIVES:
The lab goals will be accomplished through these specific objectives:
1. Explore a high level programming language for data collection and analysis. This will be Python with its popular libraries such as “pandas”.
2. Choose a topic of interest to you. It could be “sports”, “weather” or anything of current interest. Make sure you will get enough data from your data sources on the topic you have chosen.
3. Aggregate data from multiple sources to corroborate any findings and outcomes of data analysis.
4. Install a virtual machine (VM) image for data storage in HDFS and Hadoop infrastructure.
5. Familiarize yourself with MapReduce (MR) model and programming using this model.
6. Code solutions in Java or Python to process data in <key,value> format using MR model.
7. Visualize the outcome of the MR analysis using “wordcloud” visualization tool.
8. Compare the outcomes of the same analysis for at least two different sources: first an opinion social
media source such a twitter and the second one, a reliable researched source such as NYTimes.
9. Create a responsive web interface (web tool) for visualizing the outcome of your analysis.
10. Document the complete development process as a README in your submission.
 
11. (optionally) Extend the work to collect “real” big data on a topic and apply sophisticated methods such as Latent Dirichlet Allocation (LDA) and a generate conference poster or paper.
LAB DESCRIPTION:
Introduction: An important and critical phase of the data-science process is data collection. Several organizations including the federal government (data.gov) have their data available to the public for various purposes. Social network applications such as Twitter and Facebook collect enormous amount of data contributed by their numerous and prolific user. For other businesses such as Amazon and NYTimes data is a significant and valuable byproduct of their main business. Nowadays everybody has data. Most of these data generator businesses make subset of their data available for use by registered users for free. Some of them as downloadable data files (.csv, .xlsx) as a database (.db, .db3). Sometimes the data that needs to be collected is not in a specific format but is available as a web page content. In this case, typically a web crawler is used to crawl the web (pages) and scrap the data from these web pages and extract the information needed. Data generating organizations have realized the need to share at least a subset of their data with users interested in developing applications. Entire data sets are sold as products.
Recall from Lab 1, that an API or application programming interface is a standard, secure and programmatic access to data by an organization that owns the data. An API offers a method for one or two way communication among software (as well as hardware) components as long as they carry the right credentials. These credentials for authentication for programmatic access is defined by another standard OAuth (Open Authentication) delegation protocol [6] or API key in some case as in NYTimes data access [7].
We will collect data about from at least two sources, one opinion-based social media in twitter, and research data in New York Times, for the same topic or key phrase. Process the two data sets collected individually using classical big data methods. Compare the outcomes using popular visualization methods.

LAB 2: WHAT TO DO?

PAIR PROGRAMMING: We are going to allow pair programming for this lab. You will work in groups of one or two. (No groups >2). You will get an F for the course if your group plagiarizes or copies somebody else’s work or some other group’s work. You can discuss anything ONLY with your pair team member. Members in the pair have to work on the entire problem and submit your own notebooks, and submission.
Preparation: Here are the preliminary requirements for the lab.
1. Development language: We plan to use python. If you do not know the language we are giving
an opportunity to do in the part 1 of the lab. You will work with examples in Chapters 3-5 of
your text book. We will leave two copies of your text as reference in the Lockwood library.
2. For twitter and NYTimes data you will need to get the appropriate Oauth and AI keys. You do
have the Oauth keys from Lab1 and you can reuse it for twitter search API. For NYTimes or any
2 other API, you will have to apply and get the API keys ready. Now you know how to get access to
many other data sources using the standard APIs the data organizations provide.
3. For data analytics, you will need to either use the Hadoop VM we have provided or use a
Hadoop installation you are familiar with. You may install it from scratch if you have prior experience with this. Many organizations such as Cloudera provide their bundle. You can also use cloud offerings by aws (amazon), and Google cloud, if you are familiar with them. You have too many choice. Cannot decide? Just use the VM, easy for you and for use to grade.
4. Now for the visualization of the results. We want you to use the d3.js, a very popular javascript library for visualization. We have chosen to introduce d3.js for you understand origins of d3.js and how it came about from NYTimes need for complex visualizations.
