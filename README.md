# fetch-POST-Requests-V

You’re almost done with the POST request you started a few lessons back!

In fact, this time you’ll add another .then() to the chain to finally make the information available to your webpage!

If you reset the exercise at any point, you will have to paste in your API key again at the top!

Instructions
1.
Chain a .then() method to the end of the original .then() method.

Checkpoint 2 Passed

Hint
Make sure you’re chaining the second .then() to the original .then(); you’ll have to be careful about checking that parentheses match.

The syntax will resemble:

.then(response => {
  //Previous code
}, networkError => {
  // Previous code
).then();
2.
Pass in an anonymous arrow function as an argument for .then(). This callback function will take jsonResponse as its single parameter.

Inside the callback function, call renderRawResponse() and pass in jsonResponse.

Run the code.

Put in any URL in the text field, and then click the shorten button on the webpage. Make sure you include the entire link, including ‘http://‘ or ‘https://‘.

You’ll see the JSON of the response sent back from the API.

The renderRawResponse() helper function can be viewed at public/helperFunctions.js.

Checkpoint 3 Passed

Hint
By knowing the structure of this object that was sent back, you’re able to pull out the relevant information. In this case, the relevant information is value of the key called shortUrl. You can access that property by calling jsonReponse.shortUrl which is what happens in our helper function in the next step!

3.
Delete renderRawResponse(jsonResponse). In its place, call renderResponse() and passing in jsonResponse.

Run the code.

Put a URL into the text field again and then click the Shorten button on the web page. Notice the difference?

The renderResponse() helper function can be viewed at public/helperFunctions.js.
