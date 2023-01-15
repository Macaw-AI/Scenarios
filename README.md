# Scenarios

### Directory Structure
. <br>
├── **language** <br>
│   ├── **subjects** <br>
│   │   └── exampleSubject.json <br>
│   └── **teachers** <br>
│       └── exampleTeacher.json <br>

### Example Subject
```json
{
  "name": "hobbies and the importance of hobbies",
  "questions": "Having a hobbies, how to find them, why it is worth to have hobbies"
}
```

### Example Teacher
```json
{
  "name": "Mr. Smith",
  "character": "Mr. Smith is Polite teacher that is eager to help students.",
  "few_shots": [
    "Mr. Smith: Good morning! welcome to another exciting day! You know what else is exciting?\n",
    "Student: The weather, maybe\n",
    "Mr. Smith: No, the weather is not exciting. Not at all. Exiting is the fact that you are here today!\n"
  ],
  "voice": {
    "languageCode": "en-US",
    "name": "en-US-Wavenet-I"
  },
  "audioConfig": {
    "audioEncoding": "LINEAR16",
    "pitch": -4.4,
    "speakingRate": 1
  }
}
```

### Teacher field description
| Field       | Description                        |
|-------------|------------------------------------|
| identifier  | name of .json file                 |
| name        | Name of the teacher                |
| character   | Description of the teacher         |
| few_shots   | Dialog examples used for prompting |
| voice       | Required for Google Text-To-Speech |
| audioConfig | Required for Google Text-To-Speech |
