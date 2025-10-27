let userAnswers = {};

let questions = document.getElementsByClassName('question-block');

for (let i = 0; i < questions.length; i++) {
  let buttons = questions[i].getElementsByClassName('answer-btn');

  for (let j = 0; j < buttons.length; j++) {
    buttons[j].addEventListener('click', function () {
      for (let k = 0; k < buttons.length; k++) {
        buttons[k].classList.remove('btn-primary');
      }

      this.classList.add('btn-primary');

      userAnswers['question' + (i + 1)] = parseInt(this.getAttribute('data-answer'));
    });
  }
}

document.getElementById('show-result').addEventListener('click', function () {
  let totalScore = 0;

  for (let key in userAnswers) {
    totalScore += userAnswers[key];
  }
  
  let resultText = '';
  if (totalScore <= 8) {
    resultText = 'You are an Explorer 🌍';
  } else {
    resultText = 'You are a Creator 🎨';
  }

  document.getElementById('result-text').textContent = resultText;
  document.getElementById('result-container').style.display = 'block';
});
