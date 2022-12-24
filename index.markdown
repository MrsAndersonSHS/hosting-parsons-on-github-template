---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
title: Variable Assignments & Expressions 
---
# Parsons Practice


## Price Per Shirt
The following program segment should figure out the cost for each shirt if they are buy 2 and get the third free and they are originally $45 each. But the blocks have been mixed up and may include extra blocks that aren't needed in the solution. Drag the blocks from the top and put them in the correct order below. Click the Get Feedback button to check your solution or Reset to start over.
        
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
    "double totalCost = price * 2;\n" +
    "double pricePerShirt = totalCost / 3;\n" +
    "System.out.println(pricePerShirt);\n" +
    "int totalCost = price * 2 #distractor\n" +
    "print(&quot;pricePerShirt&quot;) #distractor";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "pricePerShirt-sortable",
    "max_wrong_lines": 10,
    "grader": ParsonsWidget._graders.LanguageTranslationGrader,
    "exec_limit": 2500,
    "can_indent": true,
    "x_indent": 50,
    "lang": "en",
    "show_feedback": true,
    "trashId": "pricePerShirt-sortableTrash",
    "executable_code": "price = 45\ntotalCost = price * 2\npricePerShirt = totalCost / 3\nprint(pricePerShirt)",
    "programmingLang": "pseudo",
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

## Per Person Cost
The following program segment should figure out the cost per person for a dinner including the tip. But the blocks have been mixed up and may include an extra block that isn’t needed in the solution. Drag the needed blocks from the top and put them in the correct order below. Click the Get Feedback button to check your solution & Reset Puzzle to start over.

<div id="PerPersonCost-sortableTrash" class="sortable-code"></div> 
<div id="PerPersonCost-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="PerPersonCost-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="PerPersonCost-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "double bill = 89.23;\n" +
    "double tip = bill * 0.20;\n" +
    "double total = bill + tip;\n" +
    "int numPeople = 3;\n" +
    "double perPersonCost = total/numPeople;\n" +
    "System.out.println(perPersonCost);\n" +
    "System.out.println(perpersoncost); #distractor";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "PerPersonCost-sortable",
    "max_wrong_lines": 10,
    "grader": ParsonsWidget._graders.LanguageTranslationGrader,
    "exec_limit": 2500,
    "can_indent": true,
    "x_indent": 50,
    "lang": "en",
    "show_feedback": true,
    "trashId": "PerPersonCost-sortableTrash",
    "executable_code": "bill = 89.23;\ntip = bill * 0.20;\ntotal = bill + tip;\nnumPeople = 3;\nperPersonCost = total/numPeople;\nprint(perPersonCost);",
    "programmingLang": "java",
    "vartests": []
  });
  parsonsPuzzle.init(initial);
  parsonsPuzzle.shuffleLines();
  $("#PerPersonCost-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#PerPersonCost-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>

## Gas Tank
The following code should calculate how many miles you can go on half a tank of gas if the miles per gallon is 26 and your tank holds 15 gallons. But, the blocks have been mixed up and may include extra blocks that aren't needed in the solution. Drag the needed blocks from the top and put them in the correct order below. Click the Get Feedback button to check your solution & Reset Puzzle to start over.

<div id="HalfTank-sortableTrash" class="sortable-code"></div> 
<div id="HalfTank-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="HalfTank-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="HalfTank-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "int mpg = 26;\n" +
    "int tankHolds = 15;\n" +
    "double numGallons = (double) tankHolds / 2;\n" +
    "double miles = numGallons * mpg;\n" +
    "System.out.println(miles);\n" +
    "double numGallons = tankHolds / 2; #distractor\n" +
    "int miles = numGallons * mgp; #distractor";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "HalfTank-sortable",
    "max_wrong_lines": 10,
    "grader": ParsonsWidget._graders.LanguageTranslationGrader,
    "exec_limit": 2500,
    "can_indent": true,
    "x_indent": 50,
    "lang": "en",
    "show_feedback": true,
    "trashId": "HalfTank-sortableTrash",
    "executable_code": "mpg = 26\ntankHolds = 15\nnumGallons = (double) tankHolds / 2\nmiles = numGallons * mpg\nprint(miles)",
    "programmingLang": "java",
    "vartests": []
  });
  parsonsPuzzle.init(initial);
  parsonsPuzzle.shuffleLines();
  $("#HalfTank-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#HalfTank-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>

## Average of 3 Numbers
Arrange the blocks to compute the average of three integers.  There may be extra blocks that aren't needed in the solution. Drag the needed blocks from the top and put them in the correct order below. Click the Get Feedback button to check your solution & Reset Puzzle to start over.

<div id="Average-sortableTrash" class="sortable-code"></div> 
<div id="Average-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="Average-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="Average-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "int num1 = 10;\n" +
    "int num2 = 13;\n" +
    "int num3 = 6;\n" +
    "double average = (double)(num1 + num2 + num3)/3;\n" +
    "System.out.println(average);\n" +
    "double average = num1 + num2 + num3 / 3; #distractor\n" +
    "double average = (num1 + num2 + num3) / 3; #distractor\n" +
    "System.out.println(&quot;average&quot;); #distractor";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "Average-sortable",
    "max_wrong_lines": 2,
    "grader": ParsonsWidget._graders.LanguageTranslationGrader,
    "exec_limit": 2500,
    "can_indent": true,
    "x_indent": 50,
    "lang": "en",
    "show_feedback": true,
    "trashId": "Average-sortableTrash",
    "executable_code": "num1 = 10\nnum2 = 13\nnum3 = 6\naverage = (num1 + num2 + num3)/3\nprint(average)",
    "programmingLang": "java",
    "vartests": []
  });
  parsonsPuzzle.init(initial);
  parsonsPuzzle.shuffleLines();
  $("#Average-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#Average-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>


### Implementation Notes

When you host multiple Parson's problems on a single markdown page, you need to add a unique prefix. You can easily do this in the Codio generator by typing a unique prefix into the "Prefix" textbox and pressing Enter/Return. Then you can simply copy-paste like normal.

If want each problem to be it's own page, you can use relative path links at the bottom of each of your markdown pages as seen below. If you want students to be able to return to previous problems in this format, consider adding previous links or link to a table of contents like page.

### Example Next Link
[Next](./parsons/exmaple1.html)
