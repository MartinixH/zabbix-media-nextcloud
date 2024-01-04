# zabbix-media-nextcloud
Media type for Zabbix to send alerts to Nextcloud Talk

## 1. Create user in your Nextcloud
First of all you will need to create user in your Nextcloud instance, that will send alerts.

## 2. Create chat in Nextcloud Talk
Login to created user in previous step, create chatroom, invite contacts who will recieve alerts and note room ID. You can create as chatrooms as you like.

![chatroomid](https://github.com/MartinixH/zabbix-media-nextcloud/assets/5636244/3373c157-4d76-4a57-947e-0e5f0cdb91ef)

## 3. Import media type
Go to Zabbix -> Alerts -> Media Types -> Import and select zbx_nextcloud_mediatype.yaml

## 4. Setup
Open media type and enter username and password created in fist step and change serverurl to match yours Nextcloud.

In Zabbix open Users -> Users, select user which should receive alerts, click Media -> Add, as Media Type select Nextcloud and to Send to type room ID from step 2.

That's all :)
