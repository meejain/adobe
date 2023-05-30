Front End - Franklin - 


https://www.hlx.live/developer/block-collection

Franklin lab exercise - Astha - 

https://cpcontents.adobe.com/public/newlearner/newlearner_d7e2e576.html?accountId=29997&userId=1080628#/course/6644033/overview?moduleId=11826514


Boilerplate - https://github.com/adobe/helix-project-boilerplate
Helix Bot - https://github.com/apps/helix-bot/installations/new
https://<branch>--<repo>--<owner>.hlx.page/

https://main--apollotyres--meejain.hlx.page/

https://phase1--apollotyres--meejain.hlx.page/

==========================

Franklin important links - 

https://www.hlx.live/developer/block-collection
https://www.hlx.live/developer/franklin-video-series#franklin-getting-started-episode-1
https://www.hlx.live/developer/markup-sections-blocks
https://www.hlx.live/developer/anatomy-of-a-helix-project

===========================



https://main--apollotyres--meejain.hlx.live/

git clone https://github.com/<owner>/<repo>

npm install -g @adobe/helix-cli

Once you are are ready to push your changes, simply use Git to add, commit, and push and your code to your preview (https://<branch>--<repo>--<owner>.hlx.page/) and production (https://<branch>--<repo>--<owner>.hlx.live/) sites.


Franklin as a DEV - Very Important by Jessica - 

https://wiki.corp.adobe.com/display/AEMSites/Franklin+as+a+dev








==================================================================================

Technology - 

CSS - 

Flex cheat sheet - 

https://css-tricks.com/snippets/css/a-guide-to-flexbox/

test on Flex - https://appbrewery.github.io/flexboxfroggy/
test on Grid - https://appbrewery.github.io/gridgarden/


Bhanu JS Recordings - 


https://adobe.sharepoint.com/sites/ReactJS/_layouts/15/stream.aspx?id=%2Fsites%2FReactJS%2FShared%20Documents%2FWorkshop%20%2D%20CSS%20and%20JS%2017th%2D21st%20April%202023%2FRecordings%2FDay%5F1%20CSS%20and%20JS%2Emp4&wdLOR=cC8FA3494%2DDA49%2D084D%2D9FD4%2D89198E5BF8C2&ga=1

https://adobe.sharepoint.com/sites/ReactJS/_layouts/15/stream.aspx?id=%2Fsites%2FReactJS%2FShared%20Documents%2FWorkshop%20%2D%20CSS%20and%20JS%2017th%2D21st%20April%202023%2FRecordings%2FDay%5F2%2Emp4&wdLOR=c80BE9E7F%2D5C04%2DD946%2D85EF%2DADAF53D6A70E&ga=1


===================================================================================

Default HTML Format - 

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <link rel="stylesheet" href="css/styles.css" >
</head>
<body>
 
    
    <script src="js/script.js"></script>
</body>
</html>


==================================================================================
JS factorial - 

function fact(num){
    if (num == 0) return 1;
    var result = num * fact(num-1);
    return result;
}

var x=fact(4);
console.log(x);

=========================================================================

JS Fibonacci - 

function fib(num){
    var result=(num==1||num==2) ? 1: fib(num-2) + fib(num-1);
    return result;
}

var x=fib(10);
console.log(x);


=========================================================================

DOM - 

1) Creation of Element Node - 

var elementnode=document.createElement('p');
var textnode=document.createTextNode('content');
var attributenode=document.createAttribute('class');
elementnode.appendChild(textnode);
attributenode.value="some-class";
elementnode.setAttributeNode(attributenode);
document.body.appendChild(elementnode);


2) Add a random no. in paragraph element one after the other - clicking the button - 


const btn=document.querySelector("#btn-1");
function addpara(){
  const rand=Math.floor(Math.random() * 100);
  const context="Random no. is "+rand;
  const elementnode=document.createElement('p');
  const textnode=document.createTextNode(context);
  elementnode.appendChild(textnode);
  document.body.appendChild(elementnode);
}

btn.addEventListener('click',addpara);


3) Change the value of 2nd element li within ul - 

var listitem=document.querySelector("ul");
var listitemchildren=listitem.children.item(1);
listitemchildren.textContent="I have changed the Point";

Create another li - 

listitem.appendChild(document.createElement("li"));
listitem.children.item(3).textContent="Hey How are u ";


4) How to insert a new element via parent - 

var newelement=document.createElement('p');
newelement.textContent="This is a live example";
var parent=document.querySelector(".main");
var oldelement=document.querySelectorAll('p').item(0);
parent.insertBefore(newelement,oldelement);


5) Removing an old image from a div container and adding a new image - 

var container1=document.querySelector(".testing");
var newimage=document.createElement('img');
newimage.setAttribute('src',"https://blog.logrocket.com/wp-content/uploads/2020/12/localstorage-javascript-complete-guide.png");
container1.innerHTML="";
container1.appendChild(newimage);


6) Setting an attribute and hide element inner HTML - 

var newelement=document.createElement('p');
newelement.setAttribute('id',"new para");
newelement.hidden=true;

















