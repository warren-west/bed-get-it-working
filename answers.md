1. Create a let variable called isDark. It should be initialized to false.

```JavaScript
let isDark = false
```

2. JQuery: Write the code for accessing when the document is ready
```JavaScript
$("document").ready(() => {
    // do stuff here

})
```

3. Write a click event handler for the button. It should link to a function called "changeMode"

```JavaScript
$("#btn-dark-mode").on("click", changeMode)

function changeMode() {
    // do stuff here
}
```

4. Inside the function "changeMode", check if isDark is true or false

```JavaScript
$("#btn-dark-mode").on("click", changeMode)

function changeMode() {
    if (isDark) {
        // do stuff here
    }
    else {
        // do other stuff here
    }
}
```

5. If it's true, change the background color of the body to white, and the foreground color to #111. Change the color of the header to #111. Change the button text to 🌑

```JavaScript
$("#btn-dark-mode").on("click", changeMode)

function changeMode() {
    if (isDark) {
        $("body").css("background-color", "white").css("color", "#111")
        $(".header").css("color", "#111")
        $(this).text("🌑")
    }
    else {
        // do other stuff here
    }
}
```

6. If it's false, change the background color of the body to #111, and the foreground color to aliceblue. Change the color of the header to aliceblue. Change the button text to 🌕

```JavaScript
$("#btn-dark-mode").on("click", changeMode)

function changeMode() {
    if (isDark) {
        $("body").css("background-color", "white").css("color", "#111")
        $(".header").css("color", "#111")
        $(this).text("🌑")
    }
    else {
        $("body").css("background-color", "#111").css("color", "aliceblue")
        $(".header").css("color", "aliceblue")
        $(this).text("🌕")
    }
}
```

7. Finally, change the value of isDark to whatever it wasn't before

```JavaScript
$("#btn-dark-mode").on("click", changeMode)

function changeMode() {
    if (isDark) {
        $("body").css("background-color", "white").css("color", "#111")
        $(".header").css("color", "#111")
        $(this).text("🌑")
    }
    else {
        $("body").css("background-color", "#111").css("color", "aliceblue")
        $(".header").css("color", "aliceblue")
        $(this).text("🌕")
    }
    isDark = !isDark
}
```