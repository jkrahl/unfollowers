# Instagram unfollowers
Check for people that don't follow you back on Instagram.

## 1. Get a list of all followers
Go to your Instagram profile on a **computer web browser**, open the followers list by clicking in 'X Followers' and scroll to the end (use Middle-Click and drag the mouse down to go faster).

Open the Developer Tools using `Ctrl+Shift+I`, go to the 'Console' tab and paste the following code:


``` javascript
$$('._aacl._aaco._aacw._aacx._aad7._aade')
.map(div => div.innerText)
.sort()
.join('\n')
```

This will give you a list of all your followers.
Copy the result and save it in a txt file for later use.

> You can save this list from time to time, so that when someone unfollows you, you can [compare](https://www.diffchecker.com/text-compare/) the lists and see who unfollowed you.
## 2. Get a list of following users
In your Instagram profile, open the following list by clicking in 'X Following' and scroll to the end.

Again, paste the following code in the 'Console' tab:
``` javascript
$$('._aacl._aaco._aacw._aacx._aad7._aade')
.map(div => div.innerText)
.sort()
.join('\n')
```
This will give you a list of all the users you follow.
Copy the result and save it in a txt file for later use.

## 3. Compare 
Go to a website like [Diff Checker](https://www.diffchecker.com/text-compare/) to compare the lists.
On one side you will have highlighted your followed people that don't follow you, and on the other you will have your followers highlighted that you don't follow.
