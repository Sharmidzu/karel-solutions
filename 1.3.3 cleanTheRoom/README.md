# 1.3.3 cleanTheRoom

## Lösung

```java
void cleanTheRoom() {
    repeat (4) {
        moveRight();
        moveLeft();
    }
    moveRight();
    moveAndPick();
}

void moveRight() {
    moveAndPick();
    turnLeft();
    maybePick();
    moveForward();
    turnLeft();
}

void moveLeft() {
    moveAndPick();
    turnRight();
    maybePick();
    moveForward();
    turnRight();
}

void moveAndPick() {
    repeat (9) {
        maybePick();
        moveForward();
    }
}

void maybePick() {
    if (onBeeper()) {
        pickBeeper();
    }
}
```
