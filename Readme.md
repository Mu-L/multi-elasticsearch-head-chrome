# Multi Elasticsearch Head

This is a major improvement over Elasticsearch Head extension.
* Add dropdown for multiple Elasticsearch Head end-points
* More minimal look
* Able to handle non-JSON response in Any Request tab

- [X] This extension is now live on [Google Webstore](https://chrome.google.com/webstore/detail/multi-elasticsearch-head/cpmmilfkofbeimbmgiclohpodggeheim) (2020-09-13), You can add it to Chrome and Edge 

## Synopsis

Chrome Extension containing the excellent [ElasticSearch Head](https://github.com/mobz/elasticsearch-head) application.

## Motivation of Multi Elasticsearch Head

The original Elasticsearch Head doesn't offer us the easy ability to switch between different clusters, and the bookmark solution is not favorable to us.

## Motivation of Elasticsearch Head

This was created because ElasticSearch 5 removed the ability to run ElasticSearch Head as an Elastic Plugin.  This offers an alternative to self-hosting in your own web server.  It also has the advantage of bypassing CORS without configuring CORS on your Elastic server.

## Installation

Head over to [Multi Elasticsearch Head](https://chrome.google.com/webstore/detail/multi-elasticsearch-head/cpmmilfkofbeimbmgiclohpodggeheim) page on the Chrome Web Store.

## Usage

1. Click the extension icon in the toolbar of your web browser.
2. Type the address for your elastic node into the top of the new tab that opened.
3. Click the Connect button.

## Usage tips

To make this more convenient to use (ie: without having to enter in the remote ElasticSearch URL each time), it's helpful to know that you can decorate the URL to the plugin, and use a bookmark on your bookmark bar to use in the future.

* If your Elasticsearch server is local, you can use
`chrome-extension://ffmkiejjmecolpfloofpjologoblkegm/elasticsearch-head/index.html?base_uri=http://localhost:9200`
* If your Elasticsearch server is remote and you have to use a SSH tunnel through a jump host:
	* setup your tunnel (in my example, port 29200)
	  `ssh -N -L 29200:myeshost:9200 myusername@jumphost`
	* then use `chrome-extension://ffmkiejjmecolpfloofpjologoblkegm/elasticsearch-head/index.html?base_uri=http://localhost:29200` to get to the remote ES cluster.


