# Slang::Nogil

Raku slang permiting __Not__ to use sigils

```raku
my a = 3; say a;  # OUTPUT: 3
```


### Why are sigils useful anyway ?

From [jnthn](https://stackoverflow.com/questions/50399784):

1. Syntactic disambiguation : you can call a variable whatever you want, even if there happens to be a keyword with that name
2. Readability : the data in the program stands out thanks to the sigil
3. Defining assignment semantics : in Perl 6 assignment means "copy in to", thus my @a = @b means iterate @b and put each thing in it into @a, thus any future assignments to @b will not affect @a
4. Restricting what can be bound there : only Positional things to @, for example
5. In the case of the $, controlling what will be considered a single item
6. In the case of @ on a signature parameter, causing an incoming Seq to be cached
7. Interpolation in string: Now you have to use `{}`


### Links

* [European sigil €](https://raku-musings.com/eu.html) <- from the time `token sigil` was a proto

