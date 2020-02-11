# Android WSR срез (Конвертер валют)
## Unboarding
 На первом экране необходимо реализвоать "onboarding" [пример][onboarding]. Мы должны показать пользователю экран с основной функцианальностю приложения. Этот экран необходимо показать при первом запуске приложения и при последующих больше не показывать. Т.к. в приложении часто появляются новые фичи, небходимо получать струкру экранов от сервера пример response`а
 ```
 {
    "onboarding_screens":[
    	{
    		"img_url": "url",
    		"bg_color": "#bebebe",
    		"title": "title text",
    		"description": "description text"
    	},
    	{
    		"img_url": "url",
    		"bg_color": "#bebebe",
    		"title": "title text",
    		"description": "description text"
    	},
    	{
    		"img_url": "url",
    		"bg_color": "#bebebe",
    		"title": "title text",
    		"description": "description text"
    	} 
]}
 ```
 
 ## Currency converter
 На этом экране нужно реализовать обмен валют. При каждом входе в приложение следует пытаться загрузить по сети курсы валют и (в случае их доступности) сохранять их локально (кэшировать следует безусловно, не нужно проверять, отличаются ли загруженные курсы от закэшированных). В случае, если загрузить не удалось / не успели, следует использовать закэшированные курсы. Response будет в XML
 
## Settings
На этом экране нужно реализовать смену языка в приложении

[onboarding]: <https://cdn.dribbble.com/users/4859/screenshots/6269561/bitlish_onboarding_4x.png>
