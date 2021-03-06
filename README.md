# The Sentimental Verses
An emotionally filterable book of Genesis, based on [IBM Watson Tone Analyser's](https://www.ibm.com/watson/services/tone-analyzer/) interpretation of the scripture. The prototype (in the _GenesisProto_ folder) made with [Processing](http://processing.org) assigns a color block to each verse, corresponding to the tones and the likelihood of accuracy detected by Watson. The  tones are __joy__, __sadness__, __anger__, __analytical__, __confident__, __tentative__ and __fear__. 

The deliverable (in the _GenesisProd_ folder), uses [P5*js](https://p5js.org) It displays each verse with an emoji indicator and filters at the top. I use a subset of emotions here, omiting ~~analytical~~, ~~confident~~ and ~~tentative~~.

It is often said that religions are whatever people make them to be. This website allows us to go a bit further by filtering out passages that might not fit the tone that resonates most with a reader at a given moment.

This quick and dirty project was made for the Creative Coding Lab course at [HEAD Media Design, Geneva](https://www.hesge.ch/head/formations-recherche/master-en-media-design).

![alt text](https://raw.githubusercontent.com/simonpinkas/The-Sentimental-Verses/master/Screenshot.png "The Sentimental Verses Screenshot")

## Installation
You must have node and [yarn](https://yarnpkg.com/en/) installed. 

```sh
git clone https://github.com/simonpinkas/The-Sentimental-Verses.git

cd The-Sentimental-Verses/GenesisProd

yarn global add harp

harp server
```
The website should be available at <http://localhost:9000>

You can request a random verse corresponding to an emotion through [this tiny API](https://thesentimentalversesapi.herokuapp.com/verses/joy). The code is available [here](https://github.com/simonpinkas/The-Sentimental-Verses-API)