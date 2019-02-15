# Bookmarklets
Some version of Chrome disabled the ability to drag a link to the bookmarks bar. If you want to find out how to install bookmarklets, either google it or check out this tutorial by [CrossBrowserTesting.com](https://help.crossbrowsertesting.com/live-testing/getting-started/installing-the-bookmarklet/). I will add a textfield with the appropriate link data to each bookmark to copy and paste in case the drag & drop functionality is not working in your browser.

## unfix
This simple little Bookmarklet will change the position of all fixed elements to relative. This should prevent most ads and toolbars from scrolling with the content, possibly hiding parts of it.
You can install it by dragging the following link to your bookmarks bar:

<a href="javascript:for%28var%20elements%3Ddocument.body.getElementsByTagName%28%27%2A%27%29%2Clen%3Delements.length%2Ci%3D0%3Bi%3Clen%3Bi%2B%2B%29%27fixed%27%21%3Dwindow.getComputedStyle%28elements%5Bi%5D%2Cnull%29.getPropertyValue%28%27position%27%29%26%26%27sticky%27%21%3Dwindow.getComputedStyle%28elements%5Bi%5D%2Cnull%29.getPropertyValue%28%27position%27%29%7C%7Celements%5Bi%5D.setAttribute%28%27style%27%2C%27position%3Arelative%20%21important%3B%27%29%3B">unfix</a>

Or manually adding this link:
<input value="javascript:for%28var%20elements%3Ddocument.body.getElementsByTagName%28%27%2A%27%29%2Clen%3Delements.length%2Ci%3D0%3Bi%3Clen%3Bi%2B%2B%29%27fixed%27%21%3Dwindow.getComputedStyle%28elements%5Bi%5D%2Cnull%29.getPropertyValue%28%27position%27%29%26%26%27sticky%27%21%3Dwindow.getComputedStyle%28elements%5Bi%5D%2Cnull%29.getPropertyValue%28%27position%27%29%7C%7Celements%5Bi%5D.setAttribute%28%27style%27%2C%27position%3Arelative%20%21important%3B%27%29%3B">

## YouTube Ad skip & hide
Skipping YouTube ads has never been easier before. This Bookmarklet will help you prevent using annoying adblockers which sometimes also get detected and blocked. Once clicked, it will skip youtube ads and hide the banners. Should work until you manually refresh the page.

You can install it by dragging the following link to your bookmarks bar:
<a href="javascript:var%20style%20%3D%20document.createElement%28%27style%27%29%3B%20style.innerHTML%20%3D%20%27.video-ads%2C%20%23player-ads%20%7Bdisplay%3Anone%20%21important%7D%27%3B%20document.body.appendChild%28style%29%3B%20function%20removeAds%28%29%20%7B%20console.log%28%22skipping%20ad%21%22%29%3B%20if%20%28document.getElementsByClassName%28%22ad-interrupting%22%29.length%29%7B%20var%20video%20%3D%20document.getElementsByClassName%28%22html5-main-video%22%29%5B0%5D%3B%20video.currentTime%20%3D%20video.duration-0.1%3B%20document.getElementsByClassName%28%22ytp-ad-skip-button%22%29%5B0%5D.click%28%29%3B%20%7D%20%7D%20document.addEventListener%28%27yt-navigate-finish%27%2C%20removeAds%28%29%29%3B%20removeAds%28%29%3B">skip</a>

Or manually adding this link:
<input value="javascript:var%20style%20%3D%20document.createElement%28%27style%27%29%3B%20style.innerHTML%20%3D%20%27.video-ads%2C%20%23player-ads%20%7Bdisplay%3Anone%20%21important%7D%27%3B%20document.body.appendChild%28style%29%3B%20function%20removeAds%28%29%20%7B%20console.log%28%22skipping%20ad%21%22%29%3B%20if%20%28document.getElementsByClassName%28%22ad-interrupting%22%29.length%29%7B%20var%20video%20%3D%20document.getElementsByClassName%28%22html5-main-video%22%29%5B0%5D%3B%20video.currentTime%20%3D%20video.duration-0.1%3B%20document.getElementsByClassName%28%22ytp-ad-skip-button%22%29%5B0%5D.click%28%29%3B%20%7D%20%7D%20document.addEventListener%28%27yt-navigate-finish%27%2C%20removeAds%28%29%29%3B%20removeAds%28%29%3B">

## Open Page in Helium Browser

After watching the [following Video](https://youtu.be/cqjpa8-Cp-s) from Quinn at Snazzy Labs I have decided to write a simple bookmarklet for opening pages in the Helium browser.

You can install it by dragging the following link to your bookmarks bar:
<a href="javascript:window.location%20%3D%20%22helium%3A%2F%2F%22%2Bwindow.location.href.substr%28window.location.protocol.length%2B2%29%3B">Open in Helium</a>

Or manually adding this link:
<input value="javascript:window.location%20%3D%20%22helium%3A%2F%2F%22%2Bwindow.location.href.substr%28window.location.protocol.length%2B2%29%3B">

