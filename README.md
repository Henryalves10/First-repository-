# Area Calculator

This is the beginning of my journey on GitHub! For this first project, I built a simple Python command-line calculator that computes the area of squares, rectangles, triangles, and circles.

## Features
- Calculate the area of a **Square**, **Rectangle**, **Triangle**, or **Circle**
- Interactive menu that loops until the user chooses to quit
- Input validation for invalid menu choices

## Shapes supported
| Shape     | Formula              |
|-----------|-----------------------|
| Square    | side × side           |
| Rectangle | base × height          |
| Triangle  | (base × height) / 2   |
| Circle    | π × radius²            |

## Code

```python
import time
import os

while True:
    print('====================\nArea Calculator\n====================')

    print('1) Square\n2) Rectangle\n3) Triangle\n4) Circle\n5) Quit ')
    Answer = int(input('Which shape: '))

    if Answer == 1:
        Side = int(input('Side: '))
        print(f'Area = {Side * Side}')
    elif Answer == 2:
        Base = int(input('Base: '))
        Height = int(input('Height: '))
        print(f'Area = {Base * Height}')
    elif Answer == 3:
        Base = int(input('Base: '))
        Height = int(input('Height: '))
        print(f'Area = {(Base * Height) / 2}')
    elif Answer == 4:
        pi = 3.14
        Radius = float(input('Radius: '))
        print(f'Area = {pi * (Radius * Radius)}')
    elif Answer == 5:
        print('See you later!')
        break
    else:
        print('Invalid number, try again ')

    time.sleep(3)
    os.system('cls' if os.name == 'nt' else 'clear')
```
