## tarbell configure

<pre><code class="bash" data-trim>
$ tarbell configure

Configuring Tarbell. Press ctrl-c to bail out!

Would you like to use Google spreadsheets [Y/n]? y

Login in to Google and go to https://code.google.com/apis/console/ to create an app and generate the 
client_secrets.json authentication file. You should create credentials for an `installed app`. See 
http://tarbell.readthedocs.com/ for more information.

Where is your client secrets file? [~/Downloads/client_secrets.json] 

Copying /Users/davideads/Downloads/client_secrets.json to /Users/davideads/.tarbell

Would you like to authenticate your client_secrets.json? [Y/n] y
Go to the following link in your browser:

    https://accounts.google.com/o/oauth2/auth?scope=https%3A%2F%2Fwww.googleapis.com%2Fauth%2Fdrive&redirect_uri=urn%3Aietf%3Awg%3Aoauth%3A2.0%3Aoob&response_type=code&client_id=705475625983-bdm46bacl3v8hlt4dd9ufvgsmgg3jrug.apps.googleusercontent.com&access_type=offline

...

</code></pre>

<hr/>

[Read the configuration docs &raquo;](http://tarbell.readthedocs.org/en/latest/configure.html)
