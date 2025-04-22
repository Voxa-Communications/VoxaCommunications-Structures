Poorly written docs. \
For example, loading a user_settings struct would be `voxa.api.user.user_settings` \
For source code on .kv visit `https://pypi.org/project/kvprocessor/0.1.5/`
## How it works: 
 - kvprocessor loads the raw config.json file
 - program invokes kvprocessor with a string like the one mentioned above
 - name defined in config.json is spliced
 - "." are replaced by "/"
 - ".kv" is appended to our string
 - our string is appended to the URL defined in config.json
 - a GET requests fetches the file