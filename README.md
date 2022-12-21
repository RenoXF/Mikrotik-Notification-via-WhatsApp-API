# Whatsapp Gateway

Simple whatsapp api for only send message without any authentication.

## Build from source

1. `git clone https://github.com/vermaysha/whatsapp-gateway.git`
2. `cd whatsapp-gateway`
3. `yarn install` or `npm install`
4. `yarn run build` or `npm run build`
5. `yarn run serve` or `npm run serve`

## Production

1. You must build this source code first
2. `yarn install --production=true` or `npm install --omit=dev`
3. `yarn run serve` or `npm run serve`
4. then, you can setup your reverse proxy web server.

## How to Send Messages to Group Chats

1. go to folder src --> controller
2. rename ChatController.ts into what ever you want (ChatController.backup.txt for example)
3. rename ChatController.txt to ChatController.ts
4. build

## How to Get Group ID
1. open https://web.whatsapp.com/
2. open the Group Profile
3. on your keyboard press CTRL + SHIFT + I (Developer Tools / Inspect Element)
4. go to Elements TAB
5. find value with press CTRL + F
6. type @g.us and then enter
7. the value must be like this `false_123456789xxx@g.us_BAE5AB1xxxx_62xxxxx@c.us`
8. Your Group ID is `123456789xxx@g.us` (just the number)
