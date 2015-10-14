Problem 1
What is the specificity of this selector:

body .warning {
  background-color: orange;
  border: 1px solid rgb(0, 0, 0);
}
ANS: 11. (10 for class plus 1 for Element) Background orange with a thin black border (1 pixel) for a class of warning.

Problem 2
What is the specificity of this selector:
body header p#introduction.important {
  color: red;
  font-size: 150%;
}
ANS: 112 (one class, one id and two elements)

Problem 3
What is the specificity of this selector:

body p p p .welcome.back {
  background-color: blue;
  color: white;
}
ANS: 4 Elements, 2 classes = 24

Problem 4
What's wrong with this CSS rule?

p {
  color: rgba(277, 60, 0, 0);
}
ANS: First number has a max value of 255.

Problem 5
Research and explain the difference between em and rem units.

Problem 6
Style The Shard information page from Day 2.

Improve layout with padding, border, margin properties.
Use display property.
Use position property.
