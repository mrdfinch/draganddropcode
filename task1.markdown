<div id="number1-sortableTrash" class="sortable-code"></div> 
<div id="number1-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="number1-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="number1-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "print(&quot;Welcome to the Times table program!&quot;)\n" +
    "number = int(input(&quot;Which times table would you like to display?: &quot;))\n" +
    "for count in range(1,13):\n" +
    "    print(count,&quot;x&quot;,number,&quot;=&quot;,count*number)\n" +
    "Print(&quot;Welcome to the Times table program!&quot;) #distractor\n" +
    "number = input(&quot;Which times table would you like to display?: &quot;) #distractor\n" +
    "for count in range(1,12): #distractor\n" +
    "while count &lt;= 12: #distractor\n" +
    "    print(count,&quot;x&quot;,number,&quot;=&quot;,count x number) #distractor";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "number1-sortable",
    "max_wrong_lines": 10,
    "grader": ParsonsWidget._graders.LineBasedGrader,
    "exec_limit": 2500,
    "can_indent": true,
    "x_indent": 50,
    "lang": "en",
    "show_feedback": true,
    "trashId": "number1-sortableTrash"
  });
  parsonsPuzzle.init(initial);
  parsonsPuzzle.shuffleLines();
  $("#number1-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#number1-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>



<div id="number2-sortableTrash" class="sortable-code"></div> 
<div id="number2-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="number2-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="number2-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "print(&quot;test&quot;)\n" +
    "print(&quot;Hello&quot;)";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "number2-sortable",
    "max_wrong_lines": 10,
    "grader": ParsonsWidget._graders.LineBasedGrader,
    "exec_limit": 2500,
    "can_indent": true,
    "x_indent": 50,
    "lang": "en",
    "show_feedback": true,
    "trashId": "number2-sortableTrash"
  });
  parsonsPuzzle.init(initial);
  parsonsPuzzle.shuffleLines();
  $("#number2-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#number2-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>

