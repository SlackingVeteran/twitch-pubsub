# Setup topics, auth and istall requirement
* Open `webSocketClient.py` and edit value for `self.topics` and `self.auth_token` to include your channel id for channel you want to listen to and auth token for the channel
* Install the requirement with `pip3 install websockets`

# Run the pubsub client
`python3 main.py`

# Note
* Auth token for channel must have required scopes for topic you want to listen to.
* This client doesnt handle all the connection management, for ex. it doen't reconnect when twitch send `RECONNECT` signal or when connection between this client and twitch has failed.
* Please refer to Twitch's official documents to see how connections should be handled <https://dev.twitch.tv/docs/pubsub#connection-management>
