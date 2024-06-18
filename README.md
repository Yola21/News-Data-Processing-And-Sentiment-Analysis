### Reuter News Data Processing and Sentiment Analysis

#### Project Overview
- **Objective**: Developed a pipeline for processing and analyzing Reuters news data, involving data extraction, transformation, storage, and sentiment analysis using Java, MongoDB, Apache Spark, and Hadoop.

#### Key Technologies & Tools
- **Programming Languages**: Java
- **Libraries & Frameworks**: Jsoup, Apache Spark
- **Databases**: MongoDB
- **Cloud Services**: Google Cloud Platform (GCP)
- **Tools**: MongoDB Compass, Hadoop, BufferedWriter

#### Project Details

**Part 1: Data Extraction and Storage**
- **Database Setup**: Created a MongoDB Atlas account, set up the database "ReuterDb" and collection "ReuteFile".
- **Data Parsing**: Used Jsoup to parse Reuters news HTML files to extract and clean data (titles and body text).
- **Data Storage**: Stored cleaned data as documents in MongoDB, resulting in 2,000 documents.

**Part 2: Data Processing with Apache Spark**
- **Cluster Configuration**: Configured and initialized an Apache Spark cluster on GCP.
- **Data Cleaning**: Implemented HTMLTextExtract class to clean HTML data and remove stopwords.
- **Word Frequency Analysis**: Developed SparkWordCounter class to count word frequencies using JavaRDD, resulting in an output file with word frequencies.
- **Results**: Identified words with maximum and minimum frequencies, such as "mln" (2182 occurrences) and "ISTANBUL" (1 occurrence).

**Part 3: Sentiment Analysis**
- **Sentiment Analysis Model**: Implemented a Bag-of-Words model for sentiment analysis on news titles.
- **Polarity Calculation**: Compared extracted words with positive and negative word lists to calculate sentiment scores.
- **Results**: Classified news titles as Positive, Negative, or Neutral and exported the results to a CSV file.

#### Key Takeaways
- Successfully processed and analyzed large datasets with efficient use of cloud computing and big data tools.
- Achieved accurate sentiment classification by leveraging comprehensive positive and negative word lists.
- Built a scalable data pipeline capable of handling extensive text data for real-time processing and analysis.
