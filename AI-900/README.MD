
**Boomarian Azure AI Fundamentals**

Artificial Intelligence (AI)



* AI is the ability for a computer to mimic human intelligence
* AI can be derived from machine learning or deep learning
* Microsoft Azure defines AI as:
    * Machine learning (predict)
    * Anomaly detection (detect outliers based on data)
    * Computer vision
    * Natural language processing (process language and infer context)
    * Conversational ability

Machine Learning (ML)



* Machine is a subset of artificial intelligence
* Machine learning is the creation of algorithms or models from data without explicit programming
* Machine learning works by performing a specific task multiple times on a known data set and it then uses that model to perform that task on a unknown data set

Deep Learning (DL)



* Deep learning is a subset of machine learning that uses neural networks (mimicking the human brain) to learn from large datasets
* It is particularly good for unstructured data such as language or images or audio

Data science (DS)



* Data science is the combination of maths, statistics, predictive modelling and machine learning to make predictions based on patterns in data

Data Set



* Data set is group of units of data that are related or share the same data structure
* Data sets are used to train machine learning algorithms and are also used for real world applications to predict outcomes
* There are some commonly used publicly available datasets such as:
    * MNIST database 
        * A large collection (over 10,000 images) of handwritten digits/numbers 
        * Used for optical character recognition)
    * Common objects in context (coco)
        * A collection of image in JSON file (coco format) which is used to identify objects within an image and can be used for training computer vision models
        * There are around 329000 images with over 200000 labelled and around half a million object instances

Data labelling



* Data labelling is the process of identifying raw data such as images or text and adding an informative label to it to provide an identifier to the data that can assist in machine learning
    * Supervised machine learning is where data is labelled by a human
    * Unsupervised machine learning is where labels are products by a machine
* Data scientists can use 'ground truths' as an objective standard to assess or train a model; ground truths are data sets that have been labelled accurately and are considered 'correct'; this means that can be used as a standard to compare new models against

Supervised learning



* Supervised learning is a machine learning approach where data that has been labelled is used to create a model that can be used to predict outcomes 
* Some examples of supervised learning include:
    * Tagging spam emails
    * Predicting business revenue (regression)
    * Identifying objects in images
    * Optical character recognition
    * Algorithmic recommendations on YouTube or Instagram
    * Sentiment analysis

Unsupervised learning



* Unsupervised learning is where the machine learning model is used to label unclassified data
* Unsupervised learning is useful for finding patterns or trends within data
* Some examples of unsupervised learning
    * Grouping data / customers into different attributes such as nationality or age (clustering)
    * Making links between attributes within the data or market basket analysis (association)
    * Anomaly detection
    * Image compression
    * Reducing number of features (variables) whilst preserving essential information (dimensionality reduction or feature selection)

Reinforcement learning



* Reinforcement learning is where a machine learning model generates data in an attempt to reach a goal; there is no pre-existing data to base assumptions off
* Some examples of reinforcement learning include:
    * Robot navigation
    * Game AI (Code bullet videos)
    * Learning tasks

Neural network



* Neural networks are connections between 'neurons' that the human brain utilises and can also be applied to machine learning models
* A neural network is comprised of artificial neurons (nodes) which act as a function such that data entering a node will have an output that has been changed by the node function
* The connection between nodes are weighted
    * A weight is basically a multiplicative factor that is iteratively modified by the machine learning model until the model becomes mature
    * For example, if the model is designed to identify between babies and adults, nodes that are related to ageing features such as wrinkles will have a high weight whereas nodes that are associated with attributes common in babies and adults such as "has a mouth" will be given a low weight
* Nodes are organised into layers
    * The first layer will be the input layer
    * There are then multiple hidden layers which data undergoes transformations
    * The output layer is the final layer where the final output is created
* Deep learning is a neutral network that has three or more hidden layers
* A feed forward network is where connections between nodes are non-cyclical (the signal always moves in one direction)
* Backpropagation is the process where a neural network is 'trained' and involves adjusting weights of nodes until the desired outcome is achieved
    * This requires supervised learning (data set has been labelled and thus the output is known) 
    * The neural network will slowly adjust its weighting between nodes until it achieves the outcome we are looking for
    * An example would be a game of charades; when the guessers (hidden layer) provide an incorrect answer, backpropagation is the feedback the actor gives that modifies the guesser's guess (weighting changes).
* A loss function is a function that provides an error value that correlates how 'wrong' a neural network's performance is compared to the ground truth
* Activation functions are mathematical functions that are applied to signals within the hidden layers and can transform the neural network from a linear function (multiplication with weights) to a nonlinear function
    * The most common activation function is the rectified linear unit (ReLU) which sets negative inputs to 0 (whilst keeping positive inputs unchanged)
    * Activation functions facilitate backpropagation
    * Activation functions also solve the vanishing gradient descent problem 
* Layers can be classified as dense or sparse
    * Dense layers are where there are more nodes than the previous layer
    * Sparse layers are where the are less nodes than the previou layer

Machine learning pipeline (steps for machine learning)



* Preparation
    * Data labelling (supervised learning only)
    * Feature engineering (transform data to numerical elements which the machine learning model can understand)
* Model creation
    * Training (perform millions of computations to create our final model)
    * Hyperparameter tuning (modification of higher level parameters such as the learning rate or number of units per layer)
* Azure level stuff
    * Serving (machine learning happens on a computer which could be a virtual machine or a container)
    * Inference stage (the act of making a prediction)
        * Real-time endpoint (a URL that can be used to invoke a model)
        * Batch processing (use a model on multiple inputs to benefit from parallel computing for expensive models or when the input consists of a large amount of files)

Learning rate



* The learning rate is how much the model will 'modify' parameters (weighting and bias) within a model based on the error function
* Learning rates too large/fast result in wild variation in results that bounce around the 'sweet spot'
* Learning rates too small/slow result in small variation in results but the time it takes to get the 'sweet spot' can be protracted

Jupyter Notebooks



* A web-based application for creating documents that includes a mix of:
    * Live code blocks
    * Descriptive text
    * Equations
    * Visualisations (graphs or maps)
* Jupyter notebooks use the iPython version of python
* JupyterLabs is a modern IDE that includes Jupyter notebook, file browser, text editor and terminal

GPU (graphics processing unit)



* GPUs are designed to render high-resolution images and videos concurrently with the operations of the CPU
* GPUs perform parallel operations on multiple sets of data which is useful for images but also useful for machine learning tasks where we want to run an experience/function multiple times
* CPUs usually only have 4 to 16 cores (so only 4 to 16 concurrent operations can occur) whereas GPUs can have thousands of cores
* CPUs are optimised for serial tasks whereas GPUs are optimised for parallel tasks
* Some use cases for GPUs include:
    * Rendering graphics (video editing or gaming)
    * Cryptocurrency mining
    * Neural networks / machine learning
* CUDA (Compute unified device architecture) is a platform and API that allows developers to use CUDA-enabled GPUS for general computing (instead of using the GPU as a graphics card)

Feature



* In AI, a feature is a variable that we use to predict a label
* A common example is time

Label



* In AI, a label is a variable we want to predict
* A common example is 'sales'

Forecasting



* Forecasting is a term to describe the act of making a prediction using relevant data and uses trend analysis to come to this conclusion (think of predicting the weather based on current weather data)

Prediction



* Prediction is a term to describe the 'guess' of a future outcome without relevant data using statistics and decision theory (think of predicting stock market prices; there is historical data but past performance is not indicative of future performance)

Performance / Evaluation metrics



* Performance metrics are numbers used to indicate whether a machine learning algorithm is working well or not
* Some examples of performance metrics
    * Classification 
        * Accuracy - Correctness of predictions
        * Precision - Proportion of true positive predictions amongst all positive predictions
        * Recall - Proportion of true positive predictions amongst actual positive instances
        * F1 score - Harmonic mean of precision and recall
        * Receiver operating characteristic (ROC) curve
        * Area under the curve (AUC)
    * Regression
        * R2 (R squared) ranging from 0 to 1		Lower value means lower predictability
        * Mean squared error (MSE)			Lower value means higher predictability
        * Root mean squared error (RMSE)		Lower value means higher predictability
        * Mean absolute error (MAE)			Lower value means higher predictability
    * Ranking
        * Mean reciprocal rank (MRR)
        * Discounted cumulative gain (DCG)
        * Normalised DCG
    * Statistics 
        * Correlation
    * Computer vision 
        * Peak signal-to-noise ratio
        * Structural similarity index
        * Intersection over union (IoU)
    * Natural language processing (NLP)
        * Perplexity
        * BLEU (Bilingual Evaluation Understudy) score
        * METEOR (Metric for Evaluation of Translation with Explicit Ordering)
        * ROGUE ( Recall-Oriented Understudy for Gisting Evaluation)
    * Deep learning
        * Inception score 
        * Frechet Inception distance
* Internal evaluation metrics
    * Internal evaluation metrics are scores that assess the performance of the model
    * These metrics include accuracy, F1 score, precision and recall
* External evaluation metrics
    * External evaluation metrics are scores that assess the quality of the final prediction

Regression 



* Regression in data science is the technique of predicting outcomes of continuous functions based on the relationship between a dependent variable (response / outcome) and one or more independent variables (predictors or features) 
* Regression models can predict future outcomes based on labelled (supervised) data
* Regression uses a mathematical model to predict the value of the dependent variable
    * Linear regression 
    * Logistic regression (binary classification)
    * Polynomial regression
    * Multiple regression (multiple independent variables)
    * Ridge and Lasso regression
* Regression is used for many tasks such as predicting:
    * Market prices
    * Risk assessment
    * Disease progression
    * Marketing
    * Sales forecast
    * Population growth
* Models using regression will generally produce a regression line (line of best fit) which is a mathematical function that fits the data with the lowest 'error' or residual (difference between a real data point and the regression line)
* We use values such as sum of squared errors or mean square error to see how well the line of best fit matches our data set

Classification



* In data science, classification is a supervised machine learning method of predicting the category that can be applied to a data point
* There are many algorithms to classify data
    * Logistic regression (binary classification)
    * Decision trees (tree-based model)
    * Random forest
    * Support vector machines 
    * K-Nearest neighbour
    * Naive Bayes
    * Neural networks
* Classification utilise various metrics including F1-score, precision, recall and ROC-AUC (area under receiver operating characteristic curves)
* Classification is important in:
    * Spam detection
    * Image recognition
    * Sentiment analysis
    * Medical diagnosis 

Clustering 



* Clustering is the grouping of unsupervised (unlabelled) data based on similarities or differences
* Clustering enables us to label unlabelled data
* Clustering uses different algorithms including
    * K-mean
    * K-meanoids
    * Density-based (DBSCAN or density-based  spatial clustering of applications with noise)
    * Hierarchical
* Use cases for clustering
    * Identify communities or common interests amongst groups or dividing customers into meaningful groups
    * Search result grouping
    * Medical imaging grouping
    * Anomaly detection

Confusion matrix



* A confusion matrix is a table that can be used to measure the accuracy of a classification model

<table>
  <tr>
   <td>
   </td>
   <td>
Model No
   </td>
   <td>Model Yes
   </td>
  </tr>
  <tr>
   <td>True No
   </td>
   <td>True negative
   </td>
   <td>False positive
   </td>
  </tr>
  <tr>
   <td>True Yes
   </td>
   <td>False negative
   </td>
   <td>True positive
   </td>
  </tr>
</table>




* Confusion matrices are mainly for binary outcomes but can have multiple parameters (the matrix will have more columns for more parameters)

Anomaly (outliers)



* An anomaly (outlier) is an instance that stands out due to its unusual characteristics, behaviour, or values and is generally defined as a data point that is too many standard deviations from the norm 
* Examples of Anomalies:
    * Fraud detection or unauthorised transaction detection
    * Abnormal network activity as part of a cybersecurity attack
    * Abnormal patient health findings signifying disease
    * Detection of defects in manufactured items during quality control

Computer Vision 



* Computer vision is the analysis and identification of objects from an image using machine learning neural networks
* There are two main algorithms that compute vision models use
    * Convolutional Neural Network (CNN)
        * Image and video recognition
        * Mimics the processes a real eye uses
    * Recurrent Neural Network (RNN)
        * Handwriting or speech recognition
* Types of computer vision
    * Image classification (what is it)
    * Object detection (labelling objects in an image)
    * Semantic segmentation (identifying objects or segments using pixel masks - useful or moving objects)
    * Image analysis (analyse an image and give it a description such as a black cat on the fence)
    * Optical character recognition (physical text to digital text)
    * Face detection (detect faces and compare to database / track it)

Azure Computer Vision



* Seeing AI App (uses phone camera to identify environment; mainly for blind people)
* Computer Vision 
    * Analyses images and videos
    * Can help with classification, extra text from an image or identify people
* Custom Vision
    * Does the same thing as Computer VIsion but the user provides their own labelled images and a custom model is created using the user's data
    * Mainly useful for finding defects in manufacturing or identifying a specific model of an item
* Form Recogniser
    * Converts scanned documents into key/value pairs or tabulated data
* Face service
    * Detect and identify faces as well as emotion

Natural Language Processing (NLP)



* NLP is machine learning that can understand context of a body of text (corpus)
* Some examples of what NLP can do
    * Analyse (classify) and interpret text 
        * Automatically put an email into a folder based on its content (such as spam filtering)
        * Also enables for semantic search (search based on text meaning vs. regex)
    * Interpret or contextualise text (sentiment analysis)
    * Synthesise speech (voice assistants)
    * Automatically translate spoken or written phrases between languages
    * Interpret written or spoken commands and determine appropriate actions (voice assistants)

Azure Natural Language Processing



* Text Analytics
    * Sentiment analysis
    * Find key phrases
    * Identify language of text
    * Categorise entities within text
* Translator 
    * Multi-language support
    * Text-based translation
    * Real-time text translation
* Speech
    * Convert audible speech into text
* ~~Language understanding (LUIS) ~~
    * Replaced by Conversational Language Understanding (CLU)
    * A service that can be customised for our own applications and can be used to understand the data within our application and create a chat bot that is customised for our application

Conversational AI



* Conversational AI is an extension of NLP that allows computers to converse with humans in real time
* Conversational AI is used in:
    * Chat bots
    * Voice assistants
    * Interactive voice recognition systems (IVRS) - mainly used in call centres
* Use cases for conversational AI
    * Online customer support
    * Voice assistants (Google assistant / Amazon Alexa / Apple Siri)
    * Auto-complete search
    * Accessibility (voice operated UI for visually impaired individuals)
* Azure conversational AI services
    * QnA Maker (makes a conversational bot based on existing knowledge base)
    * Azure Bot Service (deploys and manages bots such as bots made with QnA maker)

Microsoft and responsible AI



* Fairness
    * AI systems should treat all people fairly
    * AI systems should avoid any bias that is introduced during the development of the AI
    * There are projects such as Fairlearn that assess the fairness of an AI model
* Reliable and Safe
    * AI systems must be tested before release and in scenarios where mistakes can happen, these mistakes must be quantified and reported to end-users
    * An example of where this is important is an AI system that controls an (auto-pilot) autonomous driving vehicle or an AI system that recommends medications based on diagnosis
* Privacy and Security
    * Many deep learning models use personally identifiable information in their training and AI systems created from this data must ensure that the data is not leaked or disclosed
    * One way to mitigate this is to run machine learning models locally on the user's device (edge computing)
* Inclusiveness
    * AI systems should be designed to empower everyone and engage people
    * Microsoft's principle is that if we can design AI solutions for a minority of users then we can design AI solutions for the majority of users
    * In reality, inclusiveness is somewhat mutually exclusive to speciality 
* Transparency
    * Transparency in AI is the concept that AI systems should be understandable to users and developers who develop these systems should be open on why they are using AI and what limitations their AI system has
    * Transparency can help mitigate unfairness, foster trust in users and help developers with debugging
* Accountability
    * The people who develop AI systems should be held accountable for maintaining ethical and legal standards 
    * AI systems should also work within the framework of governance and adhere to organisational principles

Azure Cognitive Service



* Azure Cognitive services is a family of AI services and APIs to build various AI-based applications
* Some features of Azure Cognitive Services include:
    * Use pretrained models
    * Deploy these services from the cloud or into containers
    * No machine learning expertise required
    * Adheres to strict ethical standards 
* Included services
    * Decision
        * Anomaly detector
        * Content moderator
        * Personaliser
    * Language
        * QnA Maker
        * Text Analytics
        * Translator
        * Language Understanding (Conversational Language Understanding)
    * Speech
        * Speech to Text
        * Text to Speech
        * Speech translation
        * Speaker recognition
    * Vision
        * Computer Vision
        * Custom Vision
        * Face detection
* Deploying Azure Cognitive Services involves creating a Cognitive Service resource which will then create a key and endpoint URL which we can access our AI service on Azure
* Azure Cognitive Service is designed to create a service that Azure Bot Service can then use to and create an bot interface for users to interact with the data that has been analysed by Azure Cognitive Service 

Knowledge mining



* Knowledge / data mining is the use of AI to extract important data from documents and organise it such that it is 'labelled' and easy to identify important information
* Knowledge mining involves three processes:
    * Ingest
        * Provide our AI model with structured data from Azure data storage
            * Comma separated value files (CSV)
            * Databases
        * Provide our AI model with unstructured data
            * Images
            * Document files (PDF)
            * Audio
            * Images
    * Enrich
        * The enrichment process involves using machine learning to:
            * Find patterns
            * Extract information
        * AI services we can utilise
            * Vision
            * Language
            * Speech
            * Decision
            * Search
    * Explore
        * Utilise this newly indexed data using various tools
            * Customer relationship management (CRM)
            * ERP (Enterprise resource planning software)
            * Power BI
            * RAP systems
* Use cases of knowledge mining
    * Content research
        * Knowledge mining can help individuals 'summarise' data from documents which it can then index and produce a searchable reference library
    * Identification of important details
        * Knowledge mining can read documents and extract various aspects of information (for example it could identify text relating to a specific drug in a scientific study) without users needing to manually read through the entire document
    * Customer support
        * We can automate customer support queries by training a model on a knowledge bank and then use language AI services to match the customer's query with an entry in the knowledge bank
    * Digital asset management
        * Organisations with large amounts of unstructured data can index this data using knowledge mining to create a search index 

Azure Face Service



* Azure Face service can identify:
    * Faces in an image
    * Faces with specific attributes 
        * Accessories (nose ring or earring)
        * Age
        * Blurriness of image
        * Emotion (smiling face)
        * Exposure
        * Facial hair
        * Gender
        * Glasses
        * Hair
        * Head pose
        * Make up
        * Occlusion (whether face is partially occlused)
        * Noise
    * 27 different Face landmarks (such as hair colour)
    * Similar faces (grouping or verification)
    * The same face of the same identity across a gallery of images (identification / grouping)

Azure Translate service



* Supports 90 languages and dialects
* Uses neural machine translation (used to use statistical machine translation)
* Can be customised to translate technical jargon for specific business use case

Azure Speech service



* Speech-to-text
    * Real time encoding
    * Batch processing
    * Multi-device conversation
    * Conversational transcription (identifies who the speaker is as well as what they say)
* Text-to-speech (speech synthesis) 
    * Can utilise speech synthesis markup language (SSML) that can customise:
        * Tone (such as whispering)
        * Pause (silence duration)
        * Punctuation
    * We can also create custom voices
* Speech recognition
    * Speech verification and identification 

Azure Text Analytics API



* Sentiment analysis
    * Determines if a small body of text is positive, neutral or negative
* Opinion mining
    * Subset of sentiment analysis that identifies a subject and its attached opinion
    * If the review is "the coffee is great" then sentiment analysis will give it a positive score but opinion mining will attach a positive score to the coffee
* Key phrase extraction
    * Extracts key words from a large body of text
* Language detection
* Named entity recognition
    * Can be used to identify personally identifiable information
    * Mainly used to identify entities in text such as people or places
    * Used for unstructured text
    * An example would be identifying disease names and medication names from a medical document
    * There are pre-defined semantic types:
        * Location
        * Event
        * Person
        * DIagnosis
        * Age
        * Values (number)

Optical character recognition (OCR)



* OCR is the process of extracting characters from images or video
* Azure has two APIs that can perform OCR
    * OCR API
        * Uses an older recognition model that only supports images
        * It is fast (works synchronously) but more suitable for short bodies of text
        * It is easy to implement and supports many languages
    * Read API
        * Uses a more modern recognition model that can support images and PDFs
        * It is a slower process (asynchronous) but handles large bodies of text better
        * It is harder to implement and supports fewer languages
* Azure OCR utilises the computer vision SDK

Form recogniser



* The form recogniser is a specialised OCR service that translates printed text into digital text but also preserves the structure and relationship of form-like data
    * An example would be the ingredient list table on packaging; form recogniser will not only extract the text but make the key-value pair connection between table contents (such as Sodium 500mg)
* Form recogniser can identify
    * Key value pairs
    * Selection marks (like ✔)
    * Table structures
* When a form recogniser creates an output it will show:
    * Bounding box 
    * Original file relationship (such as grouping rows in a table together)
    * Confidence score (how accurate the model thinks its recognition is)
* Form recogniser comes with pre-built models for various document types (such as invoices or business cards) but it can also use custom built document processing models
    * Custom model training
        * We can provide a minimum of 5 sample input forms and Azure form analyser can then use this data to create a custom model for recognising data on similar datasets
        * The data used to train the model can be unsupervised (unlabelled) or supervised (labelled by a human prior to training); supervised learning will allow the model to extract values of interest based on their label
    * Pre-build models
        * Receipts
            * ReceiptType: Indicates the type of receipt (e.g., purchase, return).
            * MerchantName: The name of the merchant or store where the transaction occurred.
            * MerchantPhoneNumber: Contact phone number for the merchant.
            * MerchantAddress: The address of the merchant’s location.
            * TransactionDate: Date when the transaction took place.
            * TransactionTime: Time of the transaction.
            * Total: The total amount paid, including taxes and tips.
            * Subtotal: The cost of items before taxes and tips.
            * Tax: The tax amount applied to the transaction.
            * Tip: Any additional amount added as a tip.
            * Items: A list of purchased items, including their names, quantities, and prices.
        * Business cards
            * ContactNames: Indicates the type of receipt (e.g., purchase, return).
            * FirstName: The name of the merchant or store where the transaction occurred.
            * LastName: Contact phone number for the merchant.
            * CompanyNames: The address of the merchant’s location.
            * Departments: Date when the transaction took place.
            * JobTitles: Time of the transaction.
            * Emails: The total amount paid, including taxes and tips.
            * Websites: The cost of items before taxes and tips.
            * Addresses: The tax amount applied to the transaction.
            * MobilePhones: Any additional amount added as a tip.
            * Faxes: A list of purchased items, including their names, quantities, and prices.
            * WorkPhones: A list of purchased items, including their names, quantities, and prices.
        * Invoices
            * CustomerName: Indicates the name of the customer associated with the billing or invoice.
            * ShippingAddress: Refers to the address where the goods or services are being shipped.
            * Customerld: Represents a unique identifier for the customer.
            * ShippingAddressRecipient: The recipient’s name or organization at the shipping address.
            * PurchaseOrder: A reference number for the purchase order.
            * SubTotal: The total cost of items before taxes and other charges.
            * Invoiceld: A unique identifier for the invoice.
            * TotalTax: The total tax amount applied to the invoice.
            * InvoiceDate: The date when the invoice was issued.
            * Invoice Total: The overall amount due on the invoice.
            * DueDate: The deadline for payment.
            * AmountDue: The outstanding balance to be paid.
            * VendorName: The name of the vendor or supplier.
            * ServiceAddress: The address related to the services provided.
            * VendorAddress: The address of the vendor.
            * ServiceAddressRecipient: The recipient’s name or organisation at the service address.
            * VendorAddressRecipient: The recipient’s name or organisation at the vendor address.
            * RemittanceAddress: The address where payments should be sent.
            * CustomerAddress: The address of the customer.
            * RemittanceAddressRecipient: The recipient’s name or organisation at the remittance address.
            * CustomerAddressRecipient: The recipient’s name or organisation at the customer address.
            * ServiceStartDate: The start date for the services provided.
            * BillingAddress: The address related to billing.
            * ServiceEndDate: The end date for the services provided.
            * BillingAddressRecipient: The recipient’s name or organisation at the billing address.
            * PreviousUnpaidBalance: Any outstanding balance from previous transactions.
        * Identity documents (passports or  driver licences)
            * 

LUIS (Language understanding service)



* LUIS (to be superceded by Conversational Language Understanding or CLU) is a no-code machine learning service to build natural language AI models into applications, bots and IoT devices
*  A LUIS app is composed of a schema which is a JSON file that is auto-generated and is used to define the components of the LUIS app
    * Intent 
        * If set to none, it will use the default trained model to determine intent
        * Otherwise, it can be set to a predefined intent such as 'bookFlight'
    * Entities 
        * Entities are a specific piece of information extracted from a user's input
        * So for the utterance: "book three flights to Melbourne", 'three' and 'Melbourne' are treated as entities (and a bookFlight intent would be used)
    * Utterances 
        * Utterances are examples of user input that is used to train the machine learning model
        * These examples include a pre-defined intent and entity which helps the model learn from
        * It is recommended that at least 15 utterances are used for training

QnA Maker Service



* The QnA cloud-based NLP service used to make chat bots that will create an answer based on any input from the user's custom knowledge base (KB) of information
* Some features of QnA Maker Service
    * Automatically create a machine learning model based off a URL, document or PDF file
    * Create question and answer pairs
        * Includes alternate forms of a question
        * Use metadata tags to help filter answers during a search
        * Provide follow up prompts to improve search refinement
            * This occurs when the question cannot be answered without more context from the user
            * It can also be used to provide suggestions on how to improve the knowledge base based on end-user inputs
    * Stores answers in markdown language
    * Includes 'chit-chat' options for when users ask questions that are not directly related to the knowledge base 
        * An example would be an end user asking "how are you feeling today"
        * There are around 100 predefined questions and answer pairs 
        * Administrators can set the tone of the chatbot to different types (such as friendly or professional)
    * Utilises layered running to organise  search results based on different criteria with different weighting
        * A search score is given by Azure search
        * Top results from Azure search are then funnelled into QnA Maker's natural language processing model to rerank results

Azure Bot Service



* The Azure Bot Service is a serveless on-demand bot service that is accessible via Azure Portal and administrators can register and publish their bots on different channels
    * Alexa
    * Office 365
    * Facebook
    * LINE
    * Microsoft Teams
* The bot framework SDK v4 is an open-source software development kit (SDK) that allows developers to build bots that are capable of handling sophisticated conversations
* The bot framework composer is an application (IDE) that can be used by developers to create, test, provision and manage bots
    * Bots can be deployed as an Azure web app or via Azure functions
    * There are templates to create various bots such as:
        * QnA Maker Bot
        * Personal assistant bot
        * Language bot
        * Calendar bot
        * People bot
    * There is a bot framework emulator that allows developers to debug their bot creations
    * Includes a package manager to organise third-party libraries 

Azure Machine Learning Service



* A service that provides various tools for running machine learning workloads
* Includes the following services:
    * Jupyter Notebooks
    * Azure Machine Learning SDK for Python
    * Machine Learning Ops (MLOps) for automated machine learning model pipelines
    * Data Labelling Service
    * Azure Machine Learning Designer (drag and drop interface to visually build and test ML models)
* The Azure Machine Learning Studio has a dashboard to perform various tasks
    * Notebooks: Jupyter notebooks where you write Python code to build ML models
        * A compute instance needs to be selected to run the Jupyter notebook as well as a kernel (Jupyter-specific selection)
        * We can also choose to open the notebook using the classic notebook interface, Jupyter Labs or within VSCode
    * AutoML: Automate the process of building and training a ML model
        * AutoML automates the process of creating a ML model
            * The user supplies a data set and the type of task we want the model to learn (classification, regression or time-series forecasting)
            * Classification models will make a prediction of category a piece of data will fall into based on binary (yes/no) or multiple classes
            * Regression models predict a continuous variable based on other variables
            * Time-series forecasting predicts an outcome based on time (generally follows a regression model) 
                * Examples include forecasting customer demand or revenue or inventory stock over time
                * Automated time-series experiments are treated as multivariate (many variables) regression problems
        * AutoML also includes data guard rails which is an automatic feature that performs checks on data to insure input data used to train models are of 'good quality'
            * It can check for high cardinality (too many variables in the data mix)
            * It can check for missing feature values (such as rows or columns with missing data)
            * It can perform validation split handling (split dataset into training set (bulk of data will be used for this), a validation set (evaluate and modify trained model) and a test set (assess the model's performance))
            * With AutoML, a scaling or normalisation technique will be utilised by the model
                * Standard scale wrapper (Converts 'features' or variables to be -3 to 3 based on their deviation from the 'mean')
                * Min Max Scalar (All feature values are scaled to between 0 to 1 or -1 to 1 for features with negative values) 
                * Max Absolute Scaler (Each feature is scaled to its absolute maximum; it keeps features separate from one another)
                * Robust scalar (calculate the median and interquartile range for each feature and is useful for data with extreme outliers)
                * Principal component analysis (applies linear dimensionality reduction to reduce the number of 'dimensions' (labels) a data set has making it easier to analyse)
                * Truncated SVD Wrapper (another linear dimensionality reduction technique)
                * Sparse Normaliser
        * AutoML uses a primary metric to optimise model training; this can be changed by the user though it is usually selected automatically for the user
            * Classification
                * Accuracy
                * AUC (area under curve) weighted
                * Average precision score weighted
                * Normalised macro recall
                * Precision score weighted
            * Regression and time series forecasting
                * Normalised root mean squared error
                * R2 score
                * Normalised mean absolute error
                * Spearman correlation
        * Some scenarios where a primary metric would be suitable

<table>
  <tr>
   <td rowspan="3" >
Large balanced dataset
   </td>
   <td>Accuracy
   </td>
   <td>Image classification
<p>
Sentiment Analysis
<p>
Churn prediction
   </td>
  </tr>
  <tr>
   <td>Average precision score weighted 
   </td>
   <td>Sentiment Analysis
   </td>
  </tr>
  <tr>
   <td>Normalised macro Recall
   </td>
   <td>Churn Prediction
   </td>
  </tr>
  <tr>
   <td>Small imbalanced dataset
   </td>
   <td>AUC weighted
   </td>
   <td>Fraud detection
<p>
Image classification
<p>
Spam / Anomaly detection
   </td>
  </tr>
  <tr>
   <td>Large ranged dataset (regression)
   </td>
   <td>R2 (R squared) score
   </td>
   <td>Airline delay
<p>
Bug resolution time
<p>
Salary estimation
<p>
Inventory optimisation
<p>
Price Forecasting
   </td>
  </tr>
  <tr>
   <td>Small ranged dataset (less than 20,000 data points)
   </td>
   <td>Normalised root mean squared error
   </td>
   <td>Price prediction
<p>
Review score prediction
   </td>
  </tr>
</table>


				



        * AutoML provides model validation capabilities to test our model and are several validation techniques
            * K-fold cross validation
            * Train-validation split
            * Monte Carlo cross validation
        * AutoML comes with the ability to select a statistical model that Azure thinks is best algorithm (such as standard scale wrapper or min max scalar) for preparing data prior to auto machine learning 
            * Each algorithm will be ranked based on the normalised root mean squared error (the smaller the error, the less variation and thus more accurate the model is)
            * An explanation (explainability) is given for each algorithm to show:
                * Aggregate feature importance (which features or 'variables' stand out as influencing the data)
                * Individual feature importance
                * Dataset explorer
                * Model performance (how accurate the model is when it comes to predicting outcomes)
    * Designer: Visual drag and drop process to build end-to-end ML pipelines (no-code)
    * Assets: Data that you upload which will be used for training
        * Azure ML datasets allows users to register datasets for use with ML workloads
        * Datasets can have a profile generated (does require a compute instance to generate a profile) which can detail statistics and distribution of data within the dataset
        * We can also utilise open datasets which are publicly hosted datasets which can be used for learning how to build ML models
    * Pipelines: Lists ML workflows that have been built or used
        * Pipelines is an executable workflow of a complete machine learning task (not the same as DevOps pipelines)
        * Each pipeline consists of subtasks and each subtask is independent with its own computer resource SKU and each subtask can be worked on by data scientists individually
        * Once a pipeline has been published, it can be given a REST API endpoint which allows users to rerun the pipeline from any platform 
        * Pipelines can be built using Azure Machine Learning Designer or Azure Machine Learning Python SDK
        * Once a pipeline is trained, we can create a inference pipeline (make predictions)
    * Experiments: Details on a training task are detailed here
        * Experiments is the act of running a ML task (a run) on a virtual machine or container
    * Models: A list of models that have been trained and can be deployed
        * The model registry stores all models and we can:
            * Tag
            * Restore versions 
    * Endpoints: A model deployed contains hosted accessible endpoints (such as the REST API)
        * The main use of Azure Machine Learning endpoints is to publish ML models as a web service using the REST API
        * We can use realtime endpoints to provide remote access to a ML model running on Azure Kubernetes Service or Azure Container Service
        * We can use pipeline endpoints to provide remote access to a ML pipeline
    * Compute: The underlying computing instances used for notebooks and experiments
        * Computer instances (workstations)
        * Compute clusters (scalable VM clusters for on-demand processing)
        * Inference clusters (deployment targets for predictive services that use custom trained models)
        * Attached compute (Link existing Azure VMs or Azure Databricks to Azure Machine Learning Studio)
    * Datastores: A data repository where datasets are stored
        * Azure offers the ability to connect an Azure storage service to Azure Machine LEarning Studio without needing to put authentication credentials, reducing the risk to the original data source
        * There are a number of storage services that can be accessed:
            * Azure Blob storage
            * Azure File Share
            * Azure Data Lake Storage (Gen 2)
            * Azure SQL database
            * Azure Posgres database
            * Azure MySQL database
    * Environments: Reproducible Python environment for machine learning supervised learning.
    * Data Labelling: Hire humans that work with the assistance of ML to label data for supervised learning
        * Human-in-the-loop labelling is where humans are granted access to apply labels to data
        * Machine-learning-assisted data labelling is where machine learning is used to perform labelling
    * Linked Services: A portal for external services to connect to the workspaces (e.g., Azure Synapse Analytics).

Custom vision



* Azure custom vision is a no-code managed ML model that can classify and detect objects in an image
* The process of training a custom vision ML model involves:
    * Uploading labelled images 
    * Training the ML model
    * Evaluate the model using REST API to tag unlabelled images using the custom vision model
* Custom vision has different project types
    * Classification
        * Multi-label (apply multiple labels to an image)
        * Mult-class (apply one label amongst a set to an image; such as the fruit type)
    * Object detection
* Custom vision has different classification domains
    * General
        * A1 is optimised for accuracy and recommended for large datasets or difficult scenarios (requires more time)
        * A2 is optimised for accuracy and is faster than A1 for training 
    * Food
    * Landmarks
    * Retail
* Custom vision also has  different object detection domains
    * General
        * A1 is optimised for better accuracy and performs better in more difficult scenarios but needs larger datasets and more training time
    * Logo
    * Products on shelves
* Requirements for training custom vision model
    * Classification - Tag images (minimum 15 images per tag)
    * Object detection - Hover a cursor over a auto-generated bounding box (or create one manually) and tag the selected object (minimum 15 objects per tag)
    * As a model is trained, we can utilise the smart labeller to automatically tag images as we upload them; this is known as ML-assisted labelling
* Training type
    * Quick (less accurate)
    * Advanced (increase compute time for better results)
        * Utilises an evaluation metrics (precision and recall) to decide when to stop training when the computer believes further training will yield diminishing results
        * The threshold value is known as the probability threshold value
* Evaluation metrics
    * Precision (how many true positives were detected out of all positives / inverse probability of making a false positive)
    * Recall (how many true positive were detected out of all true positive and false negative results) which determines how many relevant items were returned
    * Mean average precision (mAP) which combines recall and precision
* Testing allows us to test our model on a sample image (that has been unlabelled)
* Once a model is complete, we can publish it which will allow us to access it via an API key

Generative AI



* Generative AI is a subset of AI that focuses on creating new content or data such as:
    * Text
    * Images
    * Music
    * Speech
    * Media
* Generative AI uses advanced ML techniques such as:
    * Generative adversarial networks 
    * Variational Autoencoders
    * Transformer models (such as generative pre-trained transformer GPT)

Large language model (LLM)



* A large language model is a machine learning algorithm that recognises patterns and predicts the next word in a sentence based on what it has seen
    * The model will  predict the next word in a sentence and based on the prediction, make another prediction, creating a chain of words
    * The length of the text can vary based on instruction or limitations imposed on the model
    * As the LLM develops, it can be refined and improved with feedback
* LLM require massive amounts of text data to be trained on where it will learn patterns in language such as grammar, style, tone and sentence structure
* LLMs are designed to understand context (the relationship between words that come before and after) 

Transformer models



* Transformer models is a type of machine learning model that excels at understanding and generating language
* Transformer models have two blocks (components)
    * Encoder
        * Reads and understands input text
    * Decoder
        * Generates a new piece of text based on encoder results
* Tokenization is the process of turning input words (or part of a word) into tokens and is used by transformer models to learn how to use words
    * Each word is given a token (unique number)
    * The same word will have the same token value
    * The transformer model will create links between tokens which establishes its ability to connect words together
* Embeddings are multi-dimensional vectors (represented by an array of numbers) which the transformer model gives to various words and are a way for our model to capture the meaning of the word                                                                                                                                                                            
    * Words with similar meanings or used in similar way will have similar vector values
    * After a word is tokenized, we then transform this value into a word embedding vector
* The order of words is preserved using positional encoding
    * Positional encoding happens after embedding vectors and involves adding a positional vector to each word to keep words in position
    * This allows for sentences which may contain the same words but in different order to be unique and keep the meaning of the sentence based on order of words
* Attention is the importance of a word in the meaning of a sentence, particularly in relation to other words
    * Words that are associated with each other in a sentence (such as "dog" and "bark" will be closely related) are given  'attention' and this process of 'self-attention' allows transformer models to understand context
    * During the encoding process, words are given a numerical representation 
    * During the decoding process, new text is generated and the decoded uses attention to figure out which words it has already generated are most important and uses this information to determine what to show next
    * Multi-head attention can be utilised to derive context by giving words multiple aspects of a word (such as its meaning, its role in the sentence (word class) or whether it is the subject in the sentence)

Azure OpenAI



* Azure OpenAI is a service that allows users to deploy and manage language models based on the work done by OpenAI (Chat-GPT)
* There are several models we can utilise
    * GPT-4 models 
    * GPT-3.5 models
    * GPT-3.5 turbo models (specialised for conversations)
    * Embedding models (converts text to vectors and can be used to compare different texts to see how similar they are)
    * DALL-E models (create images based on text prompts)
    * Whisper (transcribes and translates speech to text)
* Using Azure OpenAI service
    * We can use a prompt which will then generate a text response (completion) based on our prompt
    * Costs in Azure OpenAI is determined by token cost; the more tokens used the more it costs (also newer GPT models are more costly)
        *  
    * Azure OpenAI service is a resource just like everything else on Azure so it needs to be attached to an Azure subscription
* Azure OpenAI Studio is a web-based interface where users can deploy, test and manage large language models that support generative AI app development on Azure
    * The test interface creates a chatbot where users can test their model by providing prompts and the responses provided by the model can be tweaked with parameter control

Copilots



* Copilots are Microsoft's term for tools that integrates with applications to perform common tasks using generative AI models
* Custom copilots can be designed to utilise an organisation's data (such as an organisation's knowledge base) which is used to train a custom model which can then be used to generate specific results (such as a conversational AI that can help users when they write a prompt)
* The process of creating a copilot
    * Train a large language model with some data
    * Utilise Azure OpenAI service for pretrained models (or tweak existing models)
    * Deploy the model and integrate it with an application
* Some examples of Copilot
    * Microsoft Copilot
        * Assists users with documents, spreadsheets and presentations within Windows or Microsoft Edge browser
        * It can also respond to general queries and generate content using DALL-E
    * Microsoft Bing
        * Utilises the Bing search engine to enhance browsing or searching the internet
        * It can summarise search results opposed to showing the user an index of web pages
    * Microsoft 365 Copilot
        * Integrates with various 365 services such as PowerPoint and Outlook
        * It can help generate templates for documents, spreadsheets and presentations
    * Github Copilot
        * Provides automated documentation of code
        * It can also help by testing blocks of code
        * Provides real-time assistance with auto-completion of code and suggestions of code snippets

Prompt engineering



* Prompt engineering is the process that improves the 'prompts' that users input into generative AI models
* Prompt engineering is important in:
    * Improving the quality and accuracy of the output by the generative AI
    * Improve efficiency and reduces the need for end-users to iteratively change their prompts to get the results they want
    * Minimise biases
* Methods of prompt engineering
    * Designers can add a system message that guides the AI in how it should respond when an end-user provides a prompt (such as "respond in a helpful and friendly manner")
    * Users should use precise and explicit prompts to generate non-amboiguous and higher quality responses from AI
* AI models utilise zero-shot, one-shot and few-shot learning when generating responses
    * Zero-hot learning is where the AI model predcits based on existing knowledge to generate an output (an example would be write a song about Boomy - it has no prior knowledge of what Boomy is)
    * One-shot learning is where the AI model makes predictions based on one example (such as an uploaded document) 
