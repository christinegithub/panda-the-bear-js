<!-- Select the element that contains the profile image (hint: look for the class). Change the src attribute so it points to a picture of your choosing instead.
PROTIP: use the inspector to learn the dimensions of the current profile image and use a placeholder image service such as Place Bear to get an image of the same size. -->

var profileImage = document.querySelector('.profile-image')

profileImage.src = "https://placebear.com/400/400"


<!-- Use the same approach to select the element that contains the photo of the sky and change the src attribute to another picture URL of your choosing. -->

var div = document.querySelector("#left-image")

var image = div.getElementsByTagName('img')[0]

image.src = "https://placebear.com/325/225"


<!-- Select the heading that says "Panda the Bear" and change it to your own name. -->

var heading = document.querySelector("h1.highlight");

heading.innerText = "Christine Lee";

<!-- Select the heading that says "Employment" and change it to something else. (hint: use a descendant selector) -->

var heading = document.querySelector("#employment").querySelector("h3.info-title");

heading.innerText = "Work Experience"


<!-- Change the colour of the body. -->

var body = document.querySelector("body");

body.style.backgroundColor = "grey";


<!-- Change the colour of each element using the highlight class. Use a for loop to do this. -->

var highlight = document.getElementsByClassName("highlight");

for (var i = 0; i < highlight.length; i++) {
    current = highlight[i];
    current.style.color = "blue";
}

<!-- Change the font family of the h1 to 'monospace'. -->

var h1 = document.querySelector("h1");

h1.style.fontFamily = "moonspace";


<!-- Find a way to select the round icons in the sidebar and then change their colour. -->

var icons = document.querySelectorAll("a.action-icon-bg");

for (var i = 0; i < icons.length; i++) {
    currentIcon = icons[i];
    currentIcon.style.backgroundColor = "gold";
}

<!-- Scroll down to the contact form. Change the placeholder attribute of the name field to "identify yourself". -->

document.getElementById("name").placeholder = "Identify Yourself";

<!-- Change the placeholder attribute of the message field to "state your business". -->

document.getElementById("message").placeholder = "State your business";

<!-- Give the name field a "value" attribute of "your nemesis". -->

document.getElementById("name").value = "your nemesis";

<!-- Change the value attribute of the email field to "koalathebear@gmail.com". -->

document.getElementById("email").value = "koalathebear@gmail.com";

<!-- Change the value of the submit button on the contact form to "En garde!". -->

document.getElementById("submit").value = "En garde!"

<!-- We should stop Koala from sending an email to Panda that they might regret! Find a way to disable the submit button (hint: familiarize yourself with the disabled attribute). -->

var submit = document.getElementById("submit")

submit.disabled = true

<!-- We should help Panda protect their privacy by erasing their personal details from the sidebar. -->

var ul = document.querySelector("ul");

var li = document.querySelectorAll(".bio-info-item");

ul.remove();
