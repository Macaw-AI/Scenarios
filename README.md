# Scenarios

### Directory Structure

. <br>
├── **language** <br>
│ ├── **subjects** <br>
│ │ └── exampleSubject.json <br>
│ └── **teachers** <br>
│ └── exampleTeacher.json <br>

### Example Subject

```json
{
  "name": "hobbies and the importance of hobbies",
  "related": ["relations", "self development"],
  "questions": "Having a hobbies, how to find them, why it is worth to have hobbies"
}
```

### Example Teacher

```json
{
    "name": "Mr. Smith",
    "character": "Mr. Smith is Polite teacher that is eager to help students.",
    "related_subjects": [
      "hobbies.json",
      "ancientHistory.json"
    ],
    "skill_level": "B1",
    "few_shots": [
      "Mr. Smith: Good morning! welcome to another exciting day! You know what else is exciting?\n",
      "Student: The weather, maybe\n",
      "Mr. Smith: No, the weather is not exciting. Not at all. Exiting is the fact that you are here today!\n"
    ],
    "TTS": {
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
  }
```
## Displayable fields and metadata
Teacher:
- displayable:
  - name
  - character
  - related_subjects
  - skill_level
- metadata:
  - few_shots
  - TTS

Subject:
- displayable:
  - name
  - related
- metadata:
  - questions

## Soon

### Teacher:

```json
{
    "image": "base64Img",
    "rig_path": "/path/to/rig",
    "campaign": {
      "acquaintances": [],
      "knowledge": []
    }
}
```


<br><br>
