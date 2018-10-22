# robotstreamer_mac_obs

You'll need robot id, camera id, and stream key. After registering at robotstreamer.com (if needed) and logging in, you can visit this link to create your new stream. You'll need to give it a name that identifies the stream, like JohnCam for example.

http://www.robotstreamer.com/new_stream.html


Save all the id's and stream key.

Now you can start installing:


code for running obs and connecting to robotstreamer.com on mac

[robotstreamer obs mac zip file](https://drive.google.com/file/d/1ibobaPBQFIvx5Q9_fz295ZW9K9Ua-_qk/view?usp=sharing)

the instructions for the osx app...
- unzip
- open folder
- open pippy-app (rsmacops)
- enter robotID, cameraID, streamKey and videoKey
- save & close
- open pippy-app again 
--- media server starts
--- connects to chat for tts
--- sends alive message
--- gets video and audio endpoints from api
- obs setup:
-- obs streaming settings:
-- custom server
-- server: rtmp://localhost/live
-- streamkey: cam
- obs click: start streaming

obs ->  rtmp -> pippy-app (ffmpeg) ->  robotstreamer

every time you change settings in the pippy-app you have to restart it to make them work

it uses apples terminalsay to speak.. get all voices with say -v '?'






![](https://raw.githubusercontent.com/robotstreamer/robotstreamer_mac_obs/master/obs.png)
