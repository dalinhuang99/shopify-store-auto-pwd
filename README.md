# shopifyhack
shopify pwd hack

1. create a new shopify store
2. goto Admin -> Online Store -> Preferences, goto Google Analytics, setup google Analytics,
3. After you setup google analytics there will an options [dditional Google Analytics Javascript]
4. Yep, thet's where we hacking it...
5. you neet to close the script tag like the following:

```javascript
}catch(e){};ga('send', 'pageview');
</script>
<script>

// your js code here ...

//bypass the pwd for public users, also u can use jquery
document.getElementById("Password").value = 'shopifypass';
document.getElementById("login_form").submit();
</script>
```

6. you only got 8000 characters so remove the tab/space you don't need (I know it will look ugly!)
7. see my example here: 
[https://dalinhuang.myshopify.com/](https://dalinhuang.myshopify.com/)
