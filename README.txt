README
======
Name: Patani Kalp Bharatkumar
Roll no: M26CSA009

Files
  reasoning_agent.ipynb : full implementation (parser, forward-chaining reasoner, evaluation)
  submission.csv        : predictions (id,label)
  report.pdf            : short report (representation, algorithms, experiments, traces)

How to run
  1. pip install datasets pandas reportlab
  2. Put the test file next to the notebook as test.csv (columns: id, context, question)
     or change TEST_PATH in the first cell.
  3. Run all cells. The last cells print accuracy and inference time and write the three
     files above into the submission/ folder.

Method in one line
  Regex parser -> facts + rules -> forward chaining with unification and stratified
  negation-as-failure -> True/False. No generative AI is used for the prediction.
