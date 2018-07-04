# MyMediaForAlexa
This is the XML template that can be used via Community Applications to install the **My Media for Alexa** app to run as a docker container on an unRAID system.

**What is My Media For Alexa?**   
A media server that allows you to stream audio files (e.g. music and audiobooks) that are stored on your unRAID server to Alexa enabled devices such as Amazon Echo or Amazon Dot using voice control.

More detail and the full list of features can be found on the [My Media for Alexa](http://mymediaalexa.com) web site.

**Licensing:**   
My Media for Alexa can be used for free for seven days to allow you to evaluate it.  After that you need a (very modestly priced) license to continue using it.  Details of the prices for licenses can be found  on the [My Media for Alexa](http://mymediaalexa.com) web site.  If you want to run multiple instances of My Media for Alexa then you will require a license for each instance. 

The license is activated when you use the My Media for Alexa admin screen to connect to your Amazon account.

**Networking**

Port 52050:   Communicating with Alexa   
Port 52051:   Admin of My Media For Alexa   
These ports must are fixed and cannot be changed.

Each running instance of My Media for Alexa must have its own IP address. More detail on the networking requirements can be found on the [My Media for Alexa](http://mymediaalexa.com) web site.

**Mapping**   
The My Media for Alexa docker container has two pre-configured:

- ***/datadir***:   This  should be mapped to where My Media For Alexa will store its configuration information and indexing information.
- ***/medialibrary***: This should be mapped to where your media is stored on your unRAID server.

Additional paths for media can be added if your media is stored at several locations, but you will then also need to add these paths  inside the container via the My Media for Alexa admin screens.

**Support**   
Support for the main ***My Media for Alexa*** app is via the [My Media for Alexa](http://mymediaalexa.com) web site.   
Support for unRAID specific issues is via the Docker Container section of the unRAID forums.

**Note**   
Do not forget that you also have to have activated the My Media skill via the Alexa app on your phone or tablet before you can start using My Media for Alexa to start playing your media.</Overview>
