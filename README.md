# MyMediaForAlexa
This is the XML template for installing the **My Media for Alexa** app to run as a docker container on an unRAID system using the Community Applications plugin.

**What is My Media For Alexa?**   
A media server that allows you to stream audio files (e.g. music and audiobooks) that are stored on your unRAID server to Alexa enabled devices such as Amazon Echo or Amazon Dot using voice control.

More details and the full list of features can be found on **My Media For Alexa**  [web site](http://mymediaalexa.com).

**Licensing:**   
My Media for Alexa can be used for free for seven days to allow you to evaluate it.  After that you need a (very modestly priced) license to continue using it.  Details of the prices for licenses can be found  on the [My Media for Alexa](http://mymediaalexa.com) web site.  If you want to run multiple instances of My Media for Alexa then you will require a license for each instance. 

The license is activated when you use the My Media for Alexa admin screen to connect to your Amazon account.

**Networking**

Port 52050:   Communicating with Alexa   
Port 52051:   Admin of My Media For Alexa   
These ports are fixed and cannot be changed as they are hard-coded into the Alexa skill.

The settings in the default template are fine if you only want to run a single instance of the MyMediaForAlexa docker.  In this case the docker will be running using the IP address of the unRAID server.

 If you happen to want to run multiple instances of **My Media For Alexa** (perhaps with each instance handling different media) then since the ports to be used are fixed you need to be aware that each running instance of My Media for Alexa must have its own IP address. To set this up on unRAID all instances other than the first need to be set up to use the Custom networking option.  On many systems this will be *Custom:br0* but as the name of the bridge can vary according to your unRAID setup you need to select a setting appropriate for your system.

More detail on the networking requirements can be found on the [My Media for Alexa](http://mymediaalexa.com) web site.

**Port and Path Mapping**   
The My Media for Alexa docker container has two pre-configured paths:

- ***/datadir***:   This  should be mapped to where My Media For Alexa will store its configuration information and indexing information on the unRAID server.
- ***/medialibrary***: This should be mapped to where your media is stored on your unRAID server.   

Additional paths for media can be added if your media is stored at several locations, but you will then also need to add these paths as new Watch folders via the My Media for Alexa WebUI admin screens.

**Support**   
Support for the main ***My Media for Alexa*** app is via the [My Media for Alexa](http://mymediaalexa.com) web site.   
A [change log](https://www.mymediaalexa.com/home/changelog) of what has changed in recent releases is available.   
There is a [FAQ](https://www.mymediaalexa.com/#section-10) available covering common problems encountered by users.   
Support for unRAID specific issues is via the Docker Container section of the unRAID forums.

**Note**   
Do not forget that you also have to have activated the My Media skill via the Alexa app on your phone or tablet before you can start using My Media for Alexa to start playing your media.</Overview>
