# Testing

This portfolio entry will cover the tasks completed in week 6. This will include code
created for a hangman game, and the proceeding tests created for this code. 

Two tests will be conducted on the same piece of code, this was done out of neccessity
as there has been a lack of understanding and communication, thus the code and tests created
were all done by myself.

The idea of adding code to numerous methods was considered, however, this would have been unfair
on the other members of the team. 

## Test 1

The first test was created for a piece of code which would return a word based on the difficulty 
setting a user made in Hangman. The choices are easy, medium and hard. Based on this choice,
the word returned would be easier or harder. The comments provided stated that the word difficulty would be
based on the number of letters the word contained. Easy words would contain a maximum of 6 letters, medium would
be upto 9 and hard would be 10 and over. Also, each word returned would be chosen randomly from a list of words
which meet the criteria. 

The test code for this method is as follows:

```
[Fact]
public void TestIfWordsReturnCorrectly()
{
    GamePage gamepage = new GamePage("");

    string selectedWord = gamepage.SelectWord("Easy");
    Assert.True(selectedWord.Length < 6);

    selectedWord = gamepage.SelectWord("Medium");
    Assert.True(selectedWord.Length >= 6 && selectedWord.Length < 10);

    selectedWord = gamepage.SelectWord("Hard");
    Assert.True(selectedWord.Length >= 10);

}
```
This test, named "TestIfWordsReturnCorrectly" creates an instance of "GamePage", then
creates a string named "selectedWord" and that string is equal to the string returned from 
calling the SelectWord method. This same test is done three times, to test the three parameters possible. 
The "Assert.True" is an assertion statement which will check if the conditions in the parenthasis are true,
if it is true, the test will pass. If any of the three assertion statements fail, the test fails,
even if the others pass. It is also worth noting, the first line shows "[Fact]", which signifies
that the method should be treated as a unit test.

This is an important test as it will show if the "SelectWord" method is functioning correctly and successfully
returning suitable words based on the users difficulty choice. And the test is suitable to validate
this as it ensures the words are suitable and only those words, with stringent validation.

## Test 2

As previously discussed, both tests would be on the same piece of code. The tests however differ
in their approach to testing. The first test ensured that the words returned were suitable based
on user choice. The second test will ensure that the method behaves appropriately if given an invalid
input. 

The test is as follows:

```
[Fact]
public void InvalidGameTypeTest()
{
            
    GamePage gamepage = new GamePage("");

    string selectedWord = gamepage.SelectWord("InvalidChoice");

    Assert.Equal("Unknown", selectedWord);

}
```

Some parts of this test are the same, as previously discussed, the "[Fact]" tag must be included for 
the program to know that it is a test. The name of this test is "InvalidGameTypeTest", which as the 
name suggests, this test will verify the behaviour which will occur if the code were to be given an
unsuitable parameter. The code starts like the previous test by creating an instance of "GamePage",
called gamepage. This allows access to the methods contained within the "GamePage". Using the same variable
name, "selectedWord", it is instead now equal to the value returned by passing to the "SelectWord" method,
"InvalidChoice". After, an assertion statement ensures that the information stored within "selectedWord"
should be "Unknown". If it is, the test passes.

This is important to test as it ensures that the precautions placed within the method work as intended.
If this test were to fail, it could show issues buried deeper in the program. However, it is unlikely
that this method would receive invalid information, it is none the less important to check that measures
have been taken to avoid a program crash. 

## Reflection

This week has been difficult. Due to health reasons, I wasn't able to attend the class, and asking for help within
the team proved fruitless. I understand that for this sort of work its incredibly useful for the student to get
experience working within a team. However, in a team of 15+ people, 3 people communicate, and none of them
have past experience in any of the areas covered. 

Thus, this week, I had to attempt to do this task with only the information available to me. And the quality
may not be as good as it usually is and maybe be slightly inaccurate. 

