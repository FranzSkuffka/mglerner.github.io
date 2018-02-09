<!--
.. title: NonNewtonian Scientists
.. slug: nonnewtonian-scientists
.. date: 2018-02-04 02:10:56 UTC
.. tags: 
.. category: 
.. link: 
.. description: 
.. type: text
-->

I've been working on developing an annotated syllabus for
diversity/inclusion/decolonisation in Physics and Astronomy. You can
see the results
[here](https://github.com/mglerner/IntroductoryPhysics), and this page
makes it easy for you to contribute: research a scientist, fill out
the fields below, click the link, and you'll get the text I need to
add someone to the syllabus. You can either email it to me (mglerner@protonmail.com) or send me a PR. I'll gladly reformat them to fix
any small mistakes, so don't let that stop you!

<!-- Thanks to -->
<!-- https://www.w3schools.com/js/tryit.asp?filename=tryjs_form_elements -->
<!-- for example javascript code -->

<form id="ScientistForm">
  The scientist's name:<br>
  <input type="text" name="Name" size="60"><br>
  Where this goes in a specific textbook, e.g. "Knight, 3rd edition,
  Chapter 32, section 2" Fill in as much as you know, but feel free to
  leave parts out if you don't know them. E.g. I'll do something
  reasonable with "Halliday Resnick and Walker, 6th edition":<br>
  <input type="text" name="Textbook" size="60"><br>
  Do you know information about a second, or third textbook? Let me
  know! <br>
  <input type="text" name="Textbook" size="60"><br>
  <br>
  <input type="text" name="Textbook" size="60"><br>
  Contributors: (you can put your name here if you'd like it to be
  public, or leave it out if not!) <br>
  <input type="text" name="Contributors" size="60"><br>
  Description of the scientist: <br>
  <textarea rows="10" cols="60" name="Description"></textarea><br>
  Sources: (please cite things via the APA style if possible, but I'll
  convert your citations if you'd rather just give me
  <i>something</i>). Include as many sources as you'd like here. <br>
  <textarea rows="3" cols="60" name="Sources"></textarea><br>
  Photo: please give me the URL of a photo of the scientist. I can
  make smaller versions, so don't worry about size. <br>
  <input type="text" name="Photo" size="60"><br>

</form>
  
Click "Try it" to generate the combined text, then email me the
results (<mglerner@protonmail.com>) or send me a PR (again,
the repository is [here](https://github.com/mglerner/IntroductoryPhysics))!


<button style="height:50px;width:100px" onclick="myFunction()">Try it</button>

<p id="ScientistResults"></p>

<script>
function myFunction() {
    var x = document.getElementById("ScientistForm");
    var text = "";
    var i;
    for (i = 0; i < x.length ;i++) {
        text += "# " + x.elements[i].name + "<br>" + x.elements[i].value + "<br><br>";
    }
    document.getElementById("ScientistResults").innerHTML = text;
}
</script>

