# 3.1.2 fetchTheStars
```java
void fetchTheStars() {
    while (!onBeeper()) {
        turnLeft();
        walkIt();
        dropBeeper();
        turnLeft();
        if (frontIsClear()){
            moveForward();
        }
    }
}

void walkIt() {
    if (frontIsClear()) {
        moveForward();
        walkIt();
        moveForward();
    }else{
        pickBeeper();
        turnAround();
    }
}
```
