#CSS Dock Menu

##Tutorial

If you are a big Mac fan, you will love this CSS dock menu.

![CSS dock menu screenshot](http://i.imgur.com/5VS6Z4d.jpg)

It is using Jquery library and Fisheye component from Interface and some icons.
It comes with two dock position: top and bottom.

Here I will show you how to implement it to your web page.

1. Download Source Files
    Download the CSS dock menu zip package.

2. Insert Code
    In between the HTML head tag, add the following code

    ```html
    <!--javascript-->
    <script src="https://ajax.googleapis.com/ajax/libs/jquery/1.9.0/jquery.min.js"></script>
    <script type="text/javascript" src="js/iutil.js"></script>
    <script type="text/javascript" src="js/fisheye.js"></script>
    <!--css-->
    <link href="css/dock.css" rel="stylesheet" type="text/css">
    ```

3. Configuration
    Don't forget to add the following code to anywhere within the body tag:
    ```html
    <script type="text/javascript">
        $(document).ready(function() {
            $('#dock2').Fisheye({
                maxWidth: 60,
                items: 'a',
                itemsText: 'span',
                container: '.dock-container2',
                itemWidth: 40,
                proximity: 80,
                alignment : 'left',
                valign: 'bottom',
                halign : 'center'
            }
        )};
    </script>
    ```

4. Add or Remove Items
    To add menu item to the top dock (note: span tag is after the img tag):

    ```html
    <a class="dock-item" href="#"><img src="images/home.png" alt="home"><span>Home</span></a> 
    ```
    To add menu item to the bottom dock (note: span tag is before the img tag):

    ```html
    <a class="dock-item2" href="#"><span>Home</span><img src="images/home.png" alt="home"></a>
    ```

##Browser Compatibility
Tested on IE 6, IE 7, Opera 9, Firefox 2, and Safari 2.

There may be some minor rendering issues with Safari.

##Resources

* [Original Tutorial](http://ndesign-studio.com/blog/css-dock-menu)
* [Original Source](http://interface.eyecon.ro/download)
* [Demo](http://jsbin.com/equron/1) (jsbin)