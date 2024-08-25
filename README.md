# Experiment 1


----- ALPHABET SOUP PROBLEM -----

Create a function that takes a string and returns a string with its letters in alphabetical order.

    -- CODE --
    
    def alphabet_soup(input_word):     //define the function//
    
        sorted_word = ''.join(sorted(input_word))    //Sort the characters of the string in alphabetical order//
        
        return sorted_word


    -- OUTPUT --

    print(alphabet_soup("hello"))
    OUTPUT = ehllo

    print(alphabet_soup("hacker"))
    OUTPUT = acehkr


----- EMOTICON PROBLEM -----

Create a function that changes specific words into emoticons. Given a sentence as a string, replace the words smile, grin, sad, and mad with their corresponding emoticon.

    -- CODE --
    
    def emoticons(sentence):     //define the function//
    
       words = sentence.split()     //split the sentence into words//
    
       replaced_words = []      //create a list to hold all the replaced words//
    
       for emotion in words:      //replace words with their corresponding emoticons//
            if emotion == 'smile':
               replaced_words.append(':)')
            elif emotion == 'grin':
               replaced_words.append(':D')          //check for specific words and replace them//
            elif emotion == 'sad':
               replaced_words.append(':((')
            elif emotion == 'mad':
               replaced_words.append('>:(')
            else:
               replaced_words.append(emotion)      //if a word does not match, keep it unchanged//
   
       new_sentence = ' '.join(replaced_words)      //join the words back into a sentence with spaces//

       return new_sentence


       -- OUTPUT --

       print(emoticons("Make me smile"))
       OUTPUT = Make me :)

       print(emoticons("I am mad"))
       OUTPUT= I am >:(


----- UNPACKING LIST PROBLEM -----

Unpack the list writeyourcodehere into three variables, being first, middle, and last with middle being everything in between the first and last element. Then print all three variables.

    -- CODE -- 
    
    lst = [1,2,3,4,5,6]     //define the list//

    lst = first, *middle, last     //unpack the list into three variables//


    -- OUTPUT --
    
    print(f"First: {first}    Middle: {middle}    Last: {last}")      //print with f-strings and explicit spaces//

    OUTPUT = First: 1    Middle: [2, 3, 4, 5]    Last: 6






