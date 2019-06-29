**Open Speech Recording** is a small web application to collect short snippets
of speech, and upload them to cloud storage BUT we have modified this version to allow local storage. It's designed to help gather open
speech data sets to train machine learning systems.

It's based around a small Flask app that will run on Google App Engine. This
serves up a client-side Javascript app that prompts for a series of words,
records the audio, and then POSTs the results back to the server.

## Running

To get started, you'll need to edit  the main.py file specifically the upload method and use the correct slash for your kind of OS to enable file and directory creation

```
dev_appserver.py app.yaml
```

I've often had trouble getting local copies of the app to work with cloud
storage, so you may see errors on the final upload stage with this setup. To
deploy it to an appspot instance, run this:



## Credits
To this guy Pete Warden, pete@petewarden.com  whose code we are customizing
