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
  "displayable": {
    "name": "hobbies and the importance of hobbies",
    "related": [
      "relations",
      "self development"
    ]
  },
  "metadata": {
    "questions": "Having a hobbies, how to find them, why it is worth to have hobbies"
  }
}
```

### Example Teacher

```json
{
  "displayable": {
    "name": "Mr. Smith",
    "character": "Mr. Smith is Polite teacher that is eager to help students.",
    "related_subjects": [
      "hobbies.json",
      "ancientHistory.json"
    ],
    "skill_level": "B1"
  },
  "metadata": {
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
}
```

## Soon

### Teacher:
```json
{
  "displayable": {
    "image": "base64Img"
  },
  "metadata": {
    "rig_path": "/path/to/rig",
    "campaign": {
      "acquaintances": [],
      "knowledge": []
    }
  }
}
```

### Subject:
```json
{
  "displayable": {
  },
  "metadata": {
  }
}
```

<br><br>