# tippitytappity-design

tippitytappity is a program to practice typing


## Data model

```mermaid
classDiagram
  User <|-- Level
  class User{
        - name: string
        - email: string
        - password: string
        + login(user: string, pass: string) boolean
        + get_email() string
  }
  class Level{
        - badges vector~string~
        + add_badge(title: string)
        + get_badges() vector~string~
  }

  Phrase o-- Word
  class Phrase{
        - words: (pass: string)
        - numWords: integer
  }
  class Word{
        - text: integer
        - numbers: boolean
        - special chars: boolean
        - caps: boolean
  }     
```
