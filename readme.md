![Hello World](brave-light.png)

# Brave-Browser 
## skimmed for faster browsing using group policies

i just took lots of overlapping files and combined one to fule them all into (GroupPolicy.json)
using this:

you should change values to your likings like

```js
"DefaultSearchProviderName": "Brave Search",
"DefaultSearchProviderSearchURL": "https://search.brave.com/search?q={searchTerms}",
"DnsOverHttpsMode": "secure",
"DnsOverHttpsTemplates": "put-your-DOH address here",
```

### now using in your current browser

```sh
sudo mkdir -p /etc/brave/policies/managed
sudo cp GroupPolicy.json /etc/brave/policies/managed
```

now after restarting brave you will be in an organization managed mode

more from here
(https://support.brave.app/hc/en-us/articles/360039248271-Group-Policy)

i couldnt find all options on braved own sites or was skimming them through too fast