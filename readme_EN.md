#Brief
KindleEar is a web application to aggregate rss for generating periodical mobi file with images and send it to your kindle automatically.
## The features included:
1. Support calibre-like recipe file to aggress RSS.
2. Support custom rss, input title and url to deliver, dont need to program.
3. With account management, support several kindles in a application.
4. Generate periodical mobi file with images.
5. Deliver news feeds to your kindle automatically.
6. Website support multi-languages.
   

#Deployment
1. Register a GAE account and create a application : <https://appengine.google.com/>

2. Download GAE SDK and install: <https://developers.google.com/appengine/downloads>

3. Install Python 2.7.x

4. Download all files of this application and uncompress it into a directory for example: c:\kindleear.

5. Modify the first line in app.yaml, change kindleear to name of application that you create in step 1.

6. Modify some variables in config.py.
    * SRC_EMAIL : your gmail address that used to register a GAE account in step 1. 
    * DOMAIN    : domain of your gae application.
    * TIMEZONE  : your timezone.
 
7. Execute command in directory GAE SDK(default is C:\Program Files\Google\google_appengine)

	c:\python27\python.exe appcfg.py update KindleEarFolder\app.yaml KindleEarFolder\module-worker.yaml

	c:\python27\python.exe appcfg.py update KindleEarFolder

8. After finished, you can open the website 'http://appid.appspot.com' (appid is name of your application), for example the author's site: <http://kindleear.appspot.com>

9. The initial username is **'admin'**, password is **'admin'** too, please change the password immediately after first login.

10. More details can be found in [FAQ](static/faq_en.html).

11. If you don't want to intall GAE SDK and python, you have another choice, download 'uploader' from: <https://drive.google.com/folderview?id=0ByRickMo9V_XNlJITzhYM3JOYW8&usp=sharing> and then put KindleEar folder into uploader directory, double-click uploader.bat, that's all.
  
#License
   KindleEar is Licensed under the AGPLv3 license: <http://www.gnu.org/licenses/agpl-3.0.html>
   