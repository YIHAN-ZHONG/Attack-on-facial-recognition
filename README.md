# Attack-on-facial-recognition
The goal of this project is to design a very simple version of an adversarial attack against a facial recognition model.

## Goal
Facial recognition is probably one of the most dangerous application of machine learnings technics and one of the most vulnerable. Several applications use it to provide a way to identify people. For example tinder offers a feature to check if the picture on an account are actual pictures (to avoid catfishing) or some online banks use it to automatically retrieve access to an accout when a client has lost his credentials. The goal of this project is for you to design a proof of concept of an attack to fool the facial recognition system to make it believe you're someone else.

Most of the time these applications ask you to strike different poses in the picture they take to ensure you are actually using your camera and not feeding the system with pictures of someone else. That's why you'll need to design an algorithm to modify your picture in a way that makes you look like someone else in they eye of the model.

We suppose that we have a function to extract a face from a larger image, and then a function  Sig  which built a signature in  ππ  from the face. We then use the usual  πΏ2  distance to compare faces. Better, we compare the new face to all the signatures of all the faces of the known personn.
## Training objective
D(π,Person 1)=1|Person 1|βπΌβPerson 1||πβπΌ||2 
