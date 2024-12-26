This project is all about building a translating chatbot using AWS services like Lambda(to interact with AWS services), IAM(for secure access using user permissions),
Amazon Lex(build the chatbot and define conversation flow), and Amazon Translate(for translation of the sentence according to the input language specified).

First, we create a blank bot, where we specify bot name and intent.
Second, we specify intent details, such as sample utterances(possible user frases).
Third, we create manually slot type, that of language type, and enter possible languages data. After creating the slot type, we add it to the intent, as well as a text input slot.
Fourth, we specify fullfilment details which run our Lambda function to fulfill the intent.
Fifth, we create an IAM role assigned to Lambda along with TranslateFullAccess and AWSLambdaBasicExecutionRole, which will be used for Lambda function permission.
Then, we create Lamda function with necessary code and deploy and test it.
Lastly, we go back to our intent, specify Lambda function to be used by Lex, and test the translating chatbot. Possible outputs are similar to those provided in the project.
