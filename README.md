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

Grid: 2D array of size N x M
Snake: Queue (stores positions as (x, y))
Food: Position (x, y)
Direction: (dx, dy) tuple (Right, Left, Up, Down)
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
if food.x > head.x: return RIGHT
if food.x < head.x: return LEFT
if food.y > head.y: return DOWN
if food.y < head.y: return UP
function is_valid(pos):
    return pos not in snake and within_bounds(pos)
function is_valid(pos):
    return pos not in snake and within_bounds(pos)
