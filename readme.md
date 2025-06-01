Project for Math 156 made by Sunny Liang, Jonathan Moradkhan, and Uday Shukla

Simple word-prediction model that can train off of sample text and use the first part of a given phrase (in this case, a "phrase" just represents any short sequence of words that is gramatically correct; for example "He slammed the wooden door shut" would be a six-word phrase) and then guesses the rest of the phrase based on the training data.

(For instance, we might ask the model to complete the phrase "He slammed the wooden door" by guessing the final word. Words such as "shut" or "loudly" would be good guesses, whereas words like "hello" or "pineapple" would not since the phrase "He slammed the wooden door loudly" makes sense whereas the phrase "He slammed the wooden door pineapple" does not)

To evaluate the accuracy of our predictions, we used two publicly available options - GPT-2 and BERTScore, both of which can assess the grammatical sensibility of our completed phrases. In our testing, we generally found BERTScore to be a much more effective metric as it gave better scoring (in our view), but we've preserved the GPT-2 code for the sake of transparency. 