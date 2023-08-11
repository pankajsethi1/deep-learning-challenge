**  Overview of the analysis: 
The nonprofit foundation Alphabet Soup wants a tool that can help it select the applicants for funding with the best chance of success in their ventures. With our  knowledge of machine learning and neural networks, we used the features in the provided dataset to create a binary classifier that can predict whether applicants will be successful if funded by Alphabet Soup.

**  Results: 
Created a Depp learnig model which predicts whether the applicant will be successful or not with close to 75% accuracy,

**  Data Preprocessing

    *   What variable(s) are the target(s) for your model? IS_SUCCESSFUL
    *   What variable(s) are the features for your model? 
        STATUS
        ASK_AMT
        APPLICATION_TYPE_Other
        APPLICATION_TYPE_T10
        APPLICATION_TYPE_T19
        APPLICATION_TYPE_T3
        APPLICATION_TYPE_T4
        APPLICATION_TYPE_T5
        APPLICATION_TYPE_T6
        APPLICATION_TYPE_T7
        APPLICATION_TYPE_T8
        AFFILIATION_CompanySponsored
        AFFILIATION_Family/Parent
        AFFILIATION_Independent
        AFFILIATION_National
        AFFILIATION_Other
        AFFILIATION_Regional
        CLASSIFICATION_C1000
        CLASSIFICATION_C1200
        CLASSIFICATION_C2000
        CLASSIFICATION_C2100
        CLASSIFICATION_C3000
        CLASSIFICATION_Other
        USE_CASE_CommunityServ
        USE_CASE_Heathcare
        USE_CASE_Other
        USE_CASE_Preservation
        USE_CASE_ProductDev
        ORGANIZATION_Association
        ORGANIZATION_Co-operative
        ORGANIZATION_Corporation
        ORGANIZATION_Trust
        INCOME_AMT_0
        INCOME_AMT_1-9999
        INCOME_AMT_10000-24999
        INCOME_AMT_100000-499999
        INCOME_AMT_10M-50M
        INCOME_AMT_1M-5M
        INCOME_AMT_25000-99999
        INCOME_AMT_50M+
        INCOME_AMT_5M-10M
        SPECIAL_CONSIDERATIONS_N
        SPECIAL_CONSIDERATIONS_Y
    *   What variable(s) should be removed from the input data because they are neither targets nor features - 
        'EIN', 'NAME'


**  Compiling, Training, and Evaluating the Model

*   How many neurons, layers, and activation functions did you select for your neural network model, and why?
    Layer 1 - 100
    layer 2 - 40
    Activation fucntions - relu and tanh

    Just played around to get these numbers.


*   Were you able to achieve the target model performance? Yes.
*   What steps did you take in your attempts to increase model performance? 
    *   Increased the neurons in the two layers
    *   changed the activation function
    *   Increased epochs
*   Summary: Summarize the overall results of the deep learning model. Include a recommendation for how a different model could solve this classification problem, and then explain your recommendation.
*   The overall model oerfromance is pretty good with accuracy close to 75%. We can use a Randon Forest Classification Model as an alternative.