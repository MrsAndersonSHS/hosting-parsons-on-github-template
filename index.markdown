---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
title: Java Parsons Problems Homepage
---
# Links to Practice Pages

[Unit 1: Variables & Expressions](./parsons/VarAndExp.html)
[test link](./parsons/java-example.html)

<div id="pricePerShirt-sortableTrash" class="sortable-code"></div> 
<div id="pricePerShirt-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="pricePerShirt-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="pricePerShirt-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "double price = 45;\n" +
    "doube totalCost = price*2;\n" +
    "double pricePerShirt = totalCost/3;\n" +
    "System.out.println(pricePerShirt);\n" +
    "int pricePerShirt = totalCost/3; #distractor\n" +
    "System.out.println(&quot;pricePerShirt&quot;); #distractor";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "pricePerShirt-sortable",
    "max_wrong_lines": 2,
    "grader": ParsonsWidget._graders.LanguageTranslationGrader,
    "exec_limit": 2500,
    "can_indent": true,
    "x_indent": 50,
    "lang": "en",
    "show_feedback": true,
    "trashId": "pricePerShirt-sortableTrash",
    "executable_code": "price = 45;\ntotalCost = price*2;\npricePerShirt = totalCost/3;\nprint(pricePerShirt);",
    "programmingLang": "java",
    "vartests": []
  });
  parsonsPuzzle.init(initial);
  parsonsPuzzle.shuffleLines();
  $("#pricePerShirt-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#pricePerShirt-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>
