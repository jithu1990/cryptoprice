# cryptoprice
Alexa skill for fetching Coinbase API spot prices built using the Alexa Skills Kit and powered by AWS Lambda.

## Configuration
To run your own copy of the skill you can follow the directions in this [Alexa Python tutorial](https://developer.amazon.com/alexa-skills-kit/alexa-skill-quick-start-tutorial) with the following changes:
		
* You'll need to add an environment variable named `applicationID` to your Lambda function with the value set to the Application ID displayed in the Alexa Skill Developer Console.
* This skill is written in Python 3, so make sure your Lambda function's language is set accordingly.
* Replace the intent schema in the tutorial with the contents of [InteractionModel.json](InteractionModel.json).
* Since this skill uses packages not found in the default Lambda environment, you'll need to [package the Python file](https://docs.aws.amazon.com/lambda/latest/dg/lambda-python-how-to-create-deployment-package.html) to include the proper dependencies. After doing this once you can use the inline editor to make further changes.

## Custom Slot Types

* CRYPTOCURRENCY_TYPE	bitcoin | ethereum | litecoin | ether	 
* FIAT_CURRENCY_TYPE	us dollars | pounds | euros | pounds stirling | dollars

## Sample Utterances

* GetPriceIntent what's the price of {cryptocurrency}  in {fiat_currency}
* GetPriceIntent what's the {cryptocurrency} exchange rate
* GetPriceIntent how much is a {cryptocurrency} worth in {fiat_currency}
* GetPriceIntent show prices
* GetPriceIntent give prices
* GetPriceIntent give {cryptocurrency} prices in {fiat_currency}
* GetPriceIntent get prices
* GetPriceIntent get the current {cryptocurrency} price in {fiat_currency}
* GetPriceIntent what is the price of {cryptocurrency} in {fiat_currency}
* GetPriceIntent give me the price of {cryptocurrency} in {fiat_currency}
* GetPriceIntent give me the price of {cryptocurrency}
* GetPriceIntent look up the price of {cryptocurrency} in {fiat_currency}
* GetPriceIntent list prices
* GetPriceIntent how much does a {cryptocurrency} cost in {fiat_currency}
* GetPriceIntent how much does a {cryptocurrency} cost
* GetPriceIntent how much is a {cryptocurrency} worth
* GetPriceIntent how much is a {cryptocurrency} worth in {fiat_currency}
* GetPriceIntent list prices in {fiat_currency}
* GetPriceIntent get prices in {fiat_currency}
* GetPriceIntent update
* GetPriceIntent update in {fiat_currency}
* GetPriceIntent update {cryptocurrency} in {fiat_currency}
* GetPriceIntent update {cryptocurrency}
* GetPriceIntent give me the price of {cryptocurrency} in {fiat_currency}
* GetPriceIntent give me the price of {cryptocurrency}
* GetPriceIntent give me price
* GetPriceIntent give me the price
* GetPriceIntent give me prices
* GetPriceIntent give me an update on the {cryptocurrency} price
* GetPriceIntent fetch price
* GetPriceIntent fetch prices
* GetPriceIntent fetch the price of {cryptocurrency}
* GetPriceIntent fetch the price of {cryptocurrency} in {fiat_currency}
* GetPriceIntent fetch me prices
* GetPriceIntent fetch me the price of {cryptocurrency}
* GetPriceIntent fetch me the price of {cryptocurrency} in {fiat_currency}