Part 1
======
1)
image_id = document.querySelector('#left-image');
image = image_id.querySelector('img');
image.src = "https://placebear.com/cache/150-145.jpg";

2)
heading = document.querySelector('H1');
heading.innerText = "Bill Li";

3)
employ_id = document.querySelector('#employment');
employ_h3 = employ_id.querySelector('H3');
employ_h3.innerText = "   Something else";

4)
document.querySelector('body').style.color = 'red';

5)
hl_list = document.getElementsByClassName('highlight');

for(i = 0; i < hl_list.length; i++) {
   hl_list[i].style.color = 'blue';
 };

6)
h1Elements = document.getElementsByTagName("h1");

for(i = 0; i < h1Elements.length; i++) {
   h1Elements[i].style.fontFamily = 'monospace';
};

7)
icon_div = document.querySelector('.action-container');
icon_elm = icon_div.getElementsByClassName('action-icon');

for(i = 0; i < icon_elm.length; i++) {
   icon_elm[i].style.color = 'red';
};

8)
document.querySelector('#name').placeholder = 'identify yourself';

9)
document.querySelector('#message').placeholder = 'state your business';

10)
document.querySelector('#name').setAttribute("value", "your nemesis");

11)
document.querySelector('#email').setAttribute("value", "koalathebear@gmail.com");

12)
document.querySelector('#submit').value = 'En garde!';

13)
document.querySelector('#submit').disabled = true;

14)
document.querySelector('.bio-info').innerText = "";


Part 2
======
1)
images = document.querySelectorAll('img');
clonedImage = images[2].cloneNode(true);
document.querySelector('.portfolio-container').appendChild(clonedImage);

2)
for ( i = 0; i < 10; i++) {
  clonedImage = images[2].cloneNode(true);
  document.querySelector('.portfolio-container').appendChild(clonedImage);
}

3)
var listItem = document.createElement('li');
var leftSpan = document.createElement('span');
var lastUpdated = document.createTextNode('Page last updated on');
leftSpan.appendChild(lastUpdated);
listItem.appendChild(leftSpan);

var rightSpan = document.createElement('span');
today = new Date();
var todayDate = document.createTextNode(today);
rightSpan.appendChild(todayDate);
listItem.appendChild(rightSpan);

ul = document.querySelector('.bio-info');
ul.appendChild(listItem);
