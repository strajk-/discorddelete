# discorddelete
###### a tool to delete messages from any discord channel

## how do i get my auth token and channel id?
I currently do not have an automated way of grabbing these so I generally do it by hand in inspect element.
Press control + shift + i to open inspect element and select the network tab.
Filter it to XHR only in order to not get spammed by requests you dont care about.
Find either a `typing` or `messages` request and select it. The auth token is under request headers > authorization,
and the channel id is in the request url (`http://discordapp.com/api/v6/channel_id/request`)

I may look into automating this through better discord or some sort of js that you can paste into the console.
We'll see :crystal_ball: