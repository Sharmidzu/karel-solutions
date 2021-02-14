# 3.1.1 partyAgain
```java
void partyAgain() {
    while (onBeeper()) {
        turnLeft();
        pickBeeper();
        walkIt();
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
        dropBeeper();
        turnAround();
    }
}
```
