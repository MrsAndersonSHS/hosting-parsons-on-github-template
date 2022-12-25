---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
title: Variable Assignments & Expressions 
---
# Parsons Practice


## Price Per Shirt
Suppose a clothing store is having a sale where you can purchase three shirts for the cost of two.  For example, if the original price of a shirt is $45, then the total from buying 3 shirts would be $90 making the price for each shirt $30.  

Drag the blocks of code to to calculate the correct pricePerShirt for this sale. Click the Get Feedback button to check your solution or Reset to start over.

You may assume that variabled named price with double precision has already been declared and initialized.
        
<div id="pricePerShirt-sortableTrash" class="sortable-code"></div> 
<div id="pricePerShirt-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="pricePerShirt-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="pricePerShirt-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "double totalCost = $$toggle::price::pricePerShirt$$*2;\n" +
    "double $$toggle::price::pricePerShirt$$ = $$toggle::totalCost::price$$/3;\n" +
    "System.out.println(pricePerShirt);";
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
    "executable_code": "totalCost = $$toggle::price::pricePerShirt$$*2\n$$toggle::price::pricePerShirt$$ = $$toggle::totalCost::price$$/3\nprint(pricePerShirt)",
    "programmingLang": "java",
    "vartests": [
        {
            "message": "If each shirt is originally $45, then buying 3 cost for the cost of 2 would amount to $30 per shirt.",
            "initcode": "price=45",
            "code": "",
            "variables": {
                "totalCost": 90,
                "pricePerShirt": 30
            }
        },
        {
            "message": "If each shirt is originally $18, then buying 3 cost for the cost of 2 would amount to $12 per shirt.",
            "initcode": "price=18",
            "code": "",
            "variables": {
                "totalCost": 36,
                "pricePerShirt": 12
            }
        }
    ]
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
The following program segment should figure out the cost per person for a dinner including the tip. For example, suppose 5 friends go out to dinner and the bill is $95.  With a 20% tip the total is $114, so each person pays $22.80. 

Drag the blocks of code to to calculate the correct pricePerShirt for this sale. Click the Get Feedback button to check your solution or Reset to start over.

You may assume that a variable named bill with double precision has already been initiliazed.

<div id="pricePerShirt-sortableTrash" class="sortable-code"></div> 
<div id="pricePerShirt-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="pricePerShirt-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="pricePerShirt-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "double tip = bill * 0.2;\n" +
    "double total = bill + tip;\n" +
    "double costPerPerson = total / numPeople;\n" +
    "System.out.println(costPerPerson);";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "pricePerShirt-sortable",
    "max_wrong_lines": 10,
    "grader": ParsonsWidget._graders.LanguageTranslationGrader,
    "exec_limit": 2500,
    "can_indent": false,
    "x_indent": 50,
    "lang": "en",
    "show_feedback": true,
    "trashId": "pricePerShirt-sortableTrash",
    "executable_code": "tip = str(float(bill) * 1/5)\ntotal = str(bill + float(tip))\ncostPerPerson = str(float(total) / numPeople)\nprint(costPerPerson)",
    "programmingLang": "java",
    "vartests": [
        {
            "message": "5 people would each pay $22.80 if the bill was $95 before tip.",
            "initcode": "bill = 95\nnumPeople = 5",
            "code": "",
            "variables": {
                "tip": "19.0",
                "costPerPerson": "22.8"
            }
        },
        {
            "message": "3 people would each pay $35.72 if the bill was $89.30 before tip.",
            "initcode": "bill = 89.3\nnumPeople = 3",
            "code": "",
            "variables": {
                "tip": "17.86",
                "costPerPerson": "35.72"
            }
        },
        {
            "message": "The tip is 20% of the bill.",
            "initcode": "bill = 89.3\nnumPeople = 3",
            "code": "",
            "variables": {
                "tip": "17.86"
            }
        }
    ]
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

[Home](.index.markdown)
