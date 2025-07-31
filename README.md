🌙
<!---
Himasopn/Himasopn is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
  **Java**: 
  [![Java](https://img.shields.io/badge/Java-orange?style=flat&logo=java&logoColor=white&link=https://github.com/AyGemuy/OOP-JAVA-and-Android-App-Developer)](https://github.com/AyGemuy/OOP-JAVA-and-Android-App-Developer) 
  [![Spring](https://img.shields.io/badge/-Spring-lightgray?style=flat&logo=spring&link=https://github.com/AyGemuy/Java-Web-Developer)](https://github.com/AyGemuy/Java-Web-Developer)
  [![SpringBoot](https://img.shields.io/badge/-Springboot-black?style=flat&logo=springboot&link=https://github.com/AyGemuy/Java-Web-Developer)](https://github.com/AyGemuy/Java-Web-Developer)
  [![Maven](https://img.shields.io/badge/Maven-C71A36?style=flat&logo=apache-maven&link=hhttps://github.com/AyGemuy/Java-Web-Developer)](https://github.com/AyGemuy/Java-Web-Developer) 
  [![Gradle](https://img.shields.io/badge/Gradle-02303A?style=flat&logo=gradle&link=hhttps://github.com/AyGemuy/Java-Web-Developer)](https://github.com/AyGemuy/Java-Web-Developer)
  [![Jenkins](https://img.shields.io/badge/Jenkins-gray?style=flat&logo=jenkins&link=hhttps://github.com/AyGemuy/Java-Web-Developer)](https://github.com/AyGemuy/Java-Web-Developer) 
  [![XML](https://img.shields.io/badge/-XML-orange?style=flat&logo=xml&link=https://github.com/AyGemuy/Java-Web-Developer)](https://github.com/AyGemuy/Java-Web-Developer)
  [![JSON](https://img.shields.io/badge/-JSON-lightgray?style=flat&logo=json&link=https://github.com/AyGemuy/Java-Web-Developer)](https://github.com/AyGemuy/Java-Web-Developer)

XD :)

# 🐍 Automatic Snake Game (Auto Mode)

### 📦 Data Structures

- Grid: 2D array of size N x M  
- Snake: Queue (stores positions as (x, y))  
- Food: Position (x, y)  
- Direction: (dx, dy) tuple (RIGHT, LEFT, UP, DOWN)  

---

### 🔁 Game Loop

```python
while game_is_running:
    head = snake.front()
    direction = get_direction_toward(food, head)
    next_pos = head + direction

    if is_valid(next_pos):
        if next_pos == food:
            snake.push_front(next_pos)
            spawn_new_food()
        else:
            snake.push_front(next_pos)
            snake.pop_back()
    else:
        game_over()
```

---

### ➡️ get_direction_toward(food, head)

```python
def get_direction_toward(food, head):
    if food.x > head.x:
        return RIGHT
    elif food.x < head.x:
        return LEFT
    elif food.y > head.y:
        return DOWN
    elif food.y < head.y:
        return UP
```

---

### ✅ is_valid(pos)

```python
def is_valid(pos):
    return pos not in snake and within_bounds(pos)
```

---

### 🔲 within_bounds(pos)

```python
def within_bounds(pos):
    return 0 <= pos.x < N and 0 <= pos.y < M
```

---

### 🍴 When Food is Eaten

- Grow snake (don’t remove tail)
- Spawn new food at a random empty cell

---

### 🧠 AI Type

This is a **Greedy AI** (moves directly toward food).  
Advanced version can use:
- BFS (Breadth-First Search)
- A* Algorithm (for safest path)

---

### 🧪 Example Grid

```
. . . . . .
. S S S . .
. . . F . .
. . . . . .
```

S = Snake, F = Food  
Snake auto-moves toward food safely.
