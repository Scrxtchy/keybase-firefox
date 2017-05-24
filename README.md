# keybase-firefox
simple hack to get it working (Perhaps, this goes untested. Made entirely off theory)

* Import extension into firefox
* Add the native messenger path for your apporpriate operating system
	* Linux

	```
	/usr/lib/mozilla/native-messaging-hosts/io.keybase.kbnm.json
	-- OR --
	/usr/lib64/mozilla/native-messaging-hosts/io.keybase.kbnm.json
	-- OR --
	~/.mozilla/native-messaging-hosts/io.keybase.kbnm.json
	```

	* OSX

	```
	/Library/Application Support/Mozilla/NativeMessagingHosts/io.keybase.kbnm.json
	-- OR -- 
	~/Library/Application Support/Mozilla/NativeMessagingHosts/io.keybase.kbnm.json
	```

	* Windows

	```
	HKEY_CURRENT_USER\SOFTWARE\Mozilla\NativeMessagingHosts\io.keybase.kbnm
	```

		* Have the default value of this key point to `\path\to\keybase\kbnm.json`

	For more information, check this article on MDN; https://developer.mozilla.org/en-US/Add-ons/WebExtensions/Native_messaging