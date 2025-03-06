# sentence_analysis_algo

## DESCRIPTION

this project reads a sentence and provides the following details:

- The length of the sentence (the number of characters).
- The number of words in the sentence (assuming that the words are separated by a single space).
- The number of vowels in the sentence.

## ALGORITHM

Algorithme sentance_read <!--name of algo-->

var: <!--declaration of variables-->
word_count : integer; <!--to count the nbr of words in the sentence-->
char_count: integer; <!--to count the nbr of characters in the sentence-->
vowels_count: integer; <!--to count the nbr of vowels in the sentence-->
vowels : Array of charachter; <!--list of vowels-->
chara : character; <!--current char being read-->

<!--the body-->

BEGIN

<!--Initialize-->

word_count :=0;
char_count :=0;
vowels_count :=0;
vowels :=[a, e, i, u, y, o, A, E, I, O, U, Y];
chara :=' '; <!--empty-->

DO{
read chara;

IF(chara ∈ vowels) THEN
vowels_count := vowels_count +1;
ELSE
char_count := chr_count +1;
ENDIF

IF (chara := ' ') THEN
word_count := word_count+1;
ENDIF

}WHILE (char != '.')

print "word_count", word_count;
print "char_count", char_count;
print "vowels_count ", vowels_count ;

END
