# DigMeme
Developed a meme Sharing App on Android Studio using Kotlin, Volley and Glide APIs aimed for efficient, immaculate transfer of memes/images called upon by producing a JSON (JavaScript Object) Object Request and used Intent to share it.

The app has 2 prime functions:

1) Load Meme: We use Volley library to make an API call which also keeps check of caching using a priority queue. A queue is initiated in which we enqueue a JSON object GET request, which fetches the data from a certain specified URL.
The JSON object request is a standard for transmitting data from server to client. So, in this app, we are making a JSON request for a meme API of Heroku. In the response, we use the url from the JSON object to load the meme using 
Glide Library.

2) Share Meme: We make the inbuilt Android Intent request. For this app, we use the ACTION_SEND request of the type 'plain text'. We also provide an app chooser window using CreateChooser.

The next meme is loaded by designing a button to call upon a function which simply calls the load meme function.
    
