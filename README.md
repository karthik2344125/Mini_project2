# Mini_project2

The provided code reads a story template from a file named "story.txt" and prompts the user to fill in the placeholders (like `<adjective1>`, `<place>`, etc.) with their own words. After collecting the user inputs, it replaces the placeholders in the story with the provided words and prints the completed story.

Here’s a breakdown of how the code works:

1. **Reading the Story**: The code opens "story.txt" and reads its content into the variable `story`.

2. **Finding Placeholders**: It iterates through the characters in the story to find placeholders enclosed in angle brackets (`<...>`). When it finds a starting bracket `<`, it notes the index. When it finds a closing bracket `>`, it extracts the word and adds it to a set called `words`.

3. **User  Input**: For each unique placeholder found, the code prompts the user to enter a word to replace that placeholder. The user inputs are stored in a dictionary called `answers`.

4. **Replacing Placeholders**: The code then replaces each placeholder in the original story with the corresponding user input from the `answers` dictionary.

5. **Output**: Finally, it prints the completed story with all placeholders replaced by the user's words.

### Example of How It Works

If the content of "story.txt" is:

```
In the <adjective1> land of <place>, a <animal> was feeling <emotion>. The <animal> had lost its <object>.

Suddenly, a <character> appeared. 'I will help you find your <object>,' they said.

Together, they journeyed through <terrain> and faced the <weather_condition>. Finally, they found the <object> in a <place2>. The <animal> was so <emotion2> and thanked the <character>. They lived <adverb> ever after.
```

The user might provide the following inputs:

- `<adjective1>`: "magical"
- `<place>`: "Wonderland"
- `<animal>`: "rabbit"
- `<emotion>`: "sad"
- `<object>`: "watch"
- `<character>`: "tortoise"
- `<terrain>`: "forest"
- `<weather_condition>`: "rain"
- `<place2>`: "cave"
- `<emotion2>`: "happy"
- `<adverb>`: "happily"

The output would be:

```
In the magical land of Wonderland, a rabbit was feeling sad. The rabbit had lost its watch.

Suddenly, a tortoise appeared. 'I will help you find your watch,' they said.

Together, they journeyed through forest and faced the rain. Finally, they found the watch in a cave. The rabbit was so happy and thanked the tortoise. They lived happily ever after.
```

This interactive story creation process allows for a fun and personalized storytelling experience! If you need any modifications or further assistance, feel free to ask!
