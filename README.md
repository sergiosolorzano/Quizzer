## Project
Early cut of a Quiz generator: an Azure function app chunks in decently large sections a wikipedia page and requests AzureOpenAI to generate a couple of questions/answer pairs for each.

User enters the desired but exact wikipedia page title as a query parameter at the end of the URL. For example add &wiki=Video Game. If incorrect it returns Q&A for artist Roy Lichtenstein :)

It takes about 2 minutes to generate the Q&A.

https://quiz-sp-funcapp.azurewebsites.net/api/http_trigger?code=PtzKYVRXpCEkYOkbOW4jb-Cnr5GtT7W-r0GOehHfs6gxAzFuzBFtNg%3D%3D&wiki=coffee

It needs some polishing and prompt engineering work to avoid openAI repeating questions or ask about random topics.
