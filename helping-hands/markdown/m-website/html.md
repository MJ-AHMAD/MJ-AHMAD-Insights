[Page Source Code](https://github.com/CSC109/MarkdownWebsite/blob/master/html.md){:target="_blank"}

[Home](./)

# HTML

Plain HTML, CSS, and JavaScript can be used anywhere, since markdown gets converted to HTML anyway. `.html` files can be used instead of `.md` if desired. You may also have separate style sheets and script files just as you would with a regular website, but for these examples everything will be inline. 

## Colored Text
<p style="color:green;">This text is green.</p>

Only <span style="color:purple;">some</span> of this text is <span style="color:purple;">purple</span>.

<p style="background:green;">This text's background is green.</p>

<p style="background:black;color:white;">This text's background is black and its text color is white.</p>

<p style="color:teal;">
Anything I put here is teal.
All of it.
Teal.
So much Teal.
</p>

## Specify Font

<p style="font-family:times new roman;">This text is using Times New Roman font.</p>

<p style="font-family:serif;color:red">This text is using Serif font and is colored red.</p>

## Specify Font Size

<p style="font-size:80px;">Hello!</p>

## Image Size

Octocat image `octocat.png` located in the `assets/images` folder.
The first image is at 20% its original size.
The second is at 50% its original size.
The third is explicitly set to be 80 pixels wide.
The fourth is explicitly set to be 80 pixels wide and 40 pixels tall.

<img src="./assets/images/octocat.png" alt="Octocat" width="20%">

<img src="./assets/images/octocat.png" alt="Octocat" width="50%">

<img src="./assets/images/octocat.png" alt="Octocat" width="80px">

<img src="./assets/images/octocat.png" alt="Octocat" width="80px" height="40px">

An image's width and height will automatically scale together unless both are set.

## Button

<button>I'm a button</button>

<button style="color:pink;background:purple" >I'm a pink button</button>

<button onclick="location.href='https://google.com';">Go to Google</button>

## Styled Links

<a href="./" style="color:green;">Click this green link to go to the index page</a>

## Programming Logic

This is where JavaScript comes in! If you are not familiar with this, I don't recommend diving into it here unless you are feeling really adventurous...it's a PITA.

### Number Counter Example

<p id="increasing-number">0</p>
<button onclick="increaseByOne()" style="color:white;background:black">Increase number by 1</button>

<script>
function increaseByOne() {
    const increasingNumberTag = document.getElementById("increasing-number");
    const number = parseInt(increasingNumberTag.innerHTML, 10);
    increasingNumberTag.innerHTML = number + 1;
}
</script>

### Alert Example

<button onclick="createAlert()" style="color:rgb(2, 10, 50);background:rgb(10, 130, 128)">Give me a compliment!</button>

<script>
function createAlert() {
    alert("You are a great person!");
}
</script>

### Disappearing and Reappearing Example

<img id="ghost" style="visibility:visible;" src="./assets/images/ghost.png" alt="Ghost">
<script>
setInterval(toggleVisibility, 1000);
function toggleVisibility() {
    const imageTag = document.getElementById("ghost");
    imageTag.style.visibility  = imageTag.style.visibility === "visible"
        ? "hidden"
        : "visible";
}
</script>