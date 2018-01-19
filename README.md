**Text2Solresol**

This project is in its infancy, and is currently only a placeholder for when I have time to actually do it.

Text2Solresol is a python module for converting an input string into Solresol.  Further, an audio representation of the sentence/word will be generated as well.

```python
import text2solresol as tsr

text_to_translate = "Hello World"
text_in_solresol = tsr.translate(text_to_translate)

# By default, print will put out the alphanumeric representatio in solresol
print text_in_solresol

# Further, the solresol object will have a play function.  Ideally, this will include varying instruments for playing it
text_in_solresol.play(instrument="piano")
text_in_solresol.save_audio("Hello_World", instrument="piano")

# Finally, in the case of visual representation, a mapping of solresol onto ROYGBIV is done.
text_in_solresol.display()
text_in_solresol.save_image("Hello_World")
```

