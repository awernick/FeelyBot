# FeelyBot
![iOS Screenshot](https://challengepost-s3-challengepost.netdna-ssl.com/photos/production/software_photos/000/443/681/datas/gallery.jpg)

### Inspiration
The idea for FeelyBot came to us from the desire to help people with emotional disorders. There are millions of people in the world that suffer from depression, social anxiety, or other forms of disorders. We asked ourselves how we could use the Jibo platform and it's super cute interface to cheer up or improve a user's mood. FeelyBot aims to be your closest and most loyal friend; he will always be there for you, through the good and the bad. FeelyBot's goal is to improve a person's day, and in the long term help treat behavioral and emotional disorders.

### What it does
The application is designed to respond to the user's emotions while improving the interactive function between the user and bot. The app uses the database (timeline posts and photos) from the user's Facebook account, and then processing this information using numerous APIs such as Clarifai, Microsoft Emotion API, and IBM AlchemyAPI. Via these APIs, Feelybot can evaluate the strength of the user's five basic emotions: happiness, sadness, anger, disgust, and fear. The Node JS server uses Wit.ai to parse the data and build a personalized AI that can cater to the user's specific emotional needs. The AI communicates through the Jibo device to provide text-to-speech interactions to the user.

### How we built it
The server will track if there is a new Facebook post and run a sentimental analysis on the post. There are two types of post that are going go to be analyzed: text posts and image posts. With text post, FeelyBot will call an AlchemyAPI, which scores the different emotions of the post. FeelyBot then interprets the result and responds to the user in a positive way. With image post, FeelyBot will collect the image, then call Microsoft Emotion API to analyze the sentimental elements and Clarifai to get an overall description of the image. FeeleyBot combines the results from both APIs and uses it to determine the user's emotional state. All API is being called via Rapid API or native API.

The Jibo platform POSTs information to the Node server in order to get the processed information and interact with the user through text-to-speech. The user's input is then sent back to the Node server, where it is being constantly analyzed and used to improve the backend's AI to make it more personalized.

### Challenges we ran into
Javascript stupidity. JSON communication between the Jibo and a NodeJS server.

### Accomplishments that we're proud of
Killing a Jibo and bringing it back to life. We were really scared, but we ended up bonding with our Jibo after that frightening experience. We now treat every Jibo with love, and respect.

### What we learned
Facebook Authentication, Managing multiple Facebook users through OAuth, IBM Watson's Alchemy API. But most importantly, we learned how to kill and revive Jibos multiple times.

### What's next for FeelyBot
In the future, we would like to expand the FeelyBot's capabilities by taking advantage of the new Jibo API that includes better support for motion detection, and facial recognition to provide support for different users and automatically customize FeelyBot's personality for each one.

### Resources
[Devpost](https://devpost.com/software/feelybot)
