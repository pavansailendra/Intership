# Intership
#auto correct tool
# Input
my_word = input("Enter any word:")
 
# Counting word function
word_count = counting_words(main_set)
 
# Calculating probability
probs = probab_cal(word_count)
 
# only storing correct words
tmp_corrections = get_corrections(my_word, probs, main_set, 2)
for i, word_prob in enumerate(tmp_corrections):
    if(i < 3):
        print(word_prob[0])
    else:
        break
