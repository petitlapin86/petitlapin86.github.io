---
layout: post
title:      "Breaking down Javascript Storage "
date:       2018-04-26 14:54:24 +0000
permalink:  breaking_down_javascript_storage
---


AKA --->  how to prevent info from dissappearing whenever the browser screen is refreshed. Its a great asset to improve the usability of your site.

Previously, cookies were the only option for remembering this type of local, temporary data. Local storage has a significantly higher storage limit and doesn’t get sent with every HTTP request, so it can be a better option.
web storage options:

* Local Storage: 5mb of data saved to users computer

* Session Storage: is very similar but the data disappears when the browser window is closed

* Local Storage only stores string data…you couldn’t store videos or jpegs. (however you can work around  this by using JSON.stringify() to convert a data array to a string. You can then use JSON.parse() to convert the contents of localStorage back into something you can work with later in the data variable)

Here are some local storage methods you can call:

setItem()	 Adds a key and value to local storage
getItem()	 Retrieves a value by the key
removeItem()	Removes an item by key
clear()	Clears all storage


Example: 

localStorage.setItem(‘color’, ‘green’)

sessionStorage.getItem()

localStorage.removeItem()

delete localStorage.color

You can Set, Get and Remove properties in local storage the exact same way you would any other javascript object. 

Here is a great article with more information and examples about how to use Local Storage 
https://www.taniarascia.com/how-to-use-local-storage-with-javascript/



