# cv
Vous trouverez ici les informations professionelles me concernant

flowchart TD
    A([Start Screen])
    B{Select Difficulty<br>and Start Game}
    C[Initialize Timer & Score]
    D[Gameplay Loop]
    E{Mouse stops<br>for required delay}
    F[Show Target (Dot)]
    G{Click on Dot?}
    H[Add Point, Feedback, Hide Dot]
    I[Miss Feedback, Hide Dot]
    J{Time Remaining?}
    K[End Game Screen]
    L{Restart?}
    M([End])

    A --> B
    B --> C
    C --> D
    D --> E
    E -- yes --> F
    F --> G
    G -- yes --> H
    H --> J
    G -- no (timer up) --> I
    I --> J
    J -- yes --> D
    J -- no --> K
    K --> L
    L -- yes --> B
    L -- no --> M
