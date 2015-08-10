# 99 Bottles of Beer Song

## Summary
```text
99 bottles of beer on the wall, 99 bottles of beer.
Take one down, pass it around, 98 bottles of beer on the wall!

98 bottles of beer on the wall, 98 bottles of beer.
Take one down, pass it around, 97 bottles of beer on the wall!

97 bottles of beer on the wall, 97 bottles of beer.
Take one down, pass it around, 96 bottles of beer on the wall!

... and so on...

1 bottle of beer on the wall, 1 bottle of beer.
Take one down, pass it around, no more bottles of beer on the wall!
```
*Figure 1*.  Text of the song 99 Bottles of Beer.

Ah, the good old [99 Bottles of Beer](http://en.wikipedia.org/wiki/99_Bottles_of_Beer) song (see Figure 1).  Are we familiar with the song?

We're going to model someone singing this song by writing a method which produces the lyrics for the entire song.  We'll write a method `bottle_song_lyrics`, and in our virtual beer hall, calling `bottle_song_lyrics(99)` represents asking our rowdy neighbor to start singing 99 Bottles of Beer.

The verses of this song are all very similar—at least, until there's only one bottle of beer on the wall.  As we can imagine, this challenge deals with handling repetition.


## Releases
### Pre-release:  Provided Files
We'll be writing our `bottle_song_lyrics` method in the file `bottle_song_lyrics.rb`.  Remember, our method will return the lyrics of the song, dependent upon the number passed to the method.

If we want to see the text printed to the command line, we can run the file `runner.rb`, which calls the method and prints out the return value.


### Release 0: Lyrics for Any Number of Bottles
Let's define the body of our `bottle_song_lyrics` method.  The method takes as its input a positive integer that represents the number of bottles at the start of the song; we could start our song with 1 bottle, 99 bottles, or even 500 bottles.  The method returns the lyrics to the whole song as a `String` object.

How can we know that our method is operating as we expect?  Do we have tests?


###Release 1 : Refactor

Now that you have working code, it's time to refactor and DRY it up.  Consider the following:

* Are there lots of special cases in my code?  Can I isolate those special cases by creating new helper methods?
* Did I pay attention to the fact that the last two stanzas contain "1 bottle of beer" and "no more bottles of beer," respectively?
* If not, can I modify my code to handle those cases without making the code a rat's nest of conditionals?

What other improvements can you make? Find at least 3!

###Release 2 :  Sing it, recursively (Optional)

Write a **recursive** version of `bottle_song_lyrics` that has the same output as the iterative `bottle_song_lyrics`.


<!-- ##Optimize Your Learning  -->

##Resources

* Looping: [Integer#downto](http://www.ruby-doc.org/core-1.9.3/Integer.html#method-i-downto)
* [Recursion](http://en.wikipedia.org/wiki/Recursion_(computer_science))
