---
layout: post
title: "(Re-updated) Second working post"
date: 2023-10-22 18:43:54
categories: fresh
---
# (updated) Second working post

Ill edit this after the fact

*I have updated this post*

<!-- quiz -->
<script>
  var correctAnswer = '{{ correct_answer }}';  // This line replaces '{{ page.correct_answer }}'

  function checkAnswer() {
	var userAnswer = document.getElementById('answer').value.toLowerCase();
	var result = document.getElementById('result');
	if (userAnswer == correctAnswer) {
	  result.innerHTML = "Correct!";
	  result.style.color = "green";
	} else {
	  result.innerHTML = "Incorrect. Try again.";
	  result.style.color = "red";
	}
  }
</script>

{% assign correct_answer = "jekyll" %}
{% assign question = "What is the name of the static site generator used here?" %}

<p>{{ question }}</p>
<input type="text" id="answer" placeholder="Your answer here">
<button onclick="checkAnswer()">Submit</button>
<p id="result"></p>
