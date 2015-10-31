How to add your own provider.

# Introduction #

Pidgin send-screenshot comes with a list of HTTP image hosting providers and let you upload your screenshots to one of them.

Every month, new providers appear while other unfortunately disappear.
Also, more and more providers require you to register (for free) before beeing able to upload pictures. That's the reason why we had to remove some providers from our list.
Please help us to keep this list up-to-date ;-)

**PLEASE REMEMBER**

Your screenshots will be available for everyone, so **do not send private data!**

Rather than using a public provider, the best solution is to add access to your own personal hosting provider.
The next section teaches you how to do it...

# Add your own #

## Prerequisites ##

You must have a basic knowledge about [html forms](http://www.w3schools.com/htmL/html_forms.asp) and [Perl regular expressions](http://perldoc.perl.org/perlretut.html).

We assume you've already build a functional HTML form to upload pictures.

## Syntax ##

Now, let's learn how the plugin and your HTML form can communicate.
Here is the **xml synthax** you have to use:

```
       <host name="Hostname (as it will appear in the configure dialog)">
            <param location="Country where the server is located">. Not currently used.
            <param form_action="Server-side form handler"/> 
            <param file_input_name="Name of the file-select control."/>
            <param regexp="Perl regexp to mach with the (direct image link)"/.> The interesting part must be surrounded by parenthesis.

            <param name="extra name1" value="extra value1"/>
              ...
	    <param name="extra name_n" value="extra value_n"/>
        </host>
```

Note : the regexp shouldn't contain any _spaces_ as they are removed from the HTTP response.

## Where to ? ##

The action takes place in the _"send-screenshot\_data"_ folder.
It is usually located in:
  * _Drive:\Program Files\Pidgin\_ under Microsoft Windows,
  * _/usr/share/_ under Mac and Linux.

Please open _**"img\_hosting\_providers.xml"**_, then add the new xml block (and remove the providers you don't need).

## Icon ##

Located in the _"icons"_ subfolder.
Must be _PNG_ format and 32x32 sized.
Name must be "Hostname.png"

## Terms Of Service ##

Located in the _"tos"_ subfolder.
Simple text file, name must be "Hostname.txt"