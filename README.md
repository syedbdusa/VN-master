# VN-master

# Tentative Style and Conventions Guide

In order to keep the code base from becoming spaghetti (very easy in renpy), please follow these rules or I will not accept your pull request.

*Note:* These are not final, if something doesn't really work out or could be better, just start a conversation on discord

* Route names for programmming purposes will be the last name of the corresponding character
* All .rpy files relating to a specific route *must* be under a subfolder
  
  * That subfolder should have the name of the route
  
* *ALL* global labels must be formatted as such: `routename_x`, where x can be anything you want.

  * For example, dwinelle_lunch is a possible global label.
  
  * This is to prevent label collision. Unfortunately, having all labels inside a specific route be sublabels is not terribly feasible, so this pseudo namespace is the compromise
  
* Character definitions in start.rpy will use the full name. You may rebind them inside your .rpy to single letters, but you must rebind them every single time.

  * It may seem like a waste of time, but it is important that you be able to look at the top of a file and see what letters are bound to what characters. This prevents having to figure out who 'e' is. 
  
  * For example, 
  
  ```
  p = player
  d = dwinelle
  ```
  
  you must rebind these in every single file.
  
  
