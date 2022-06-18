# Find the maze count.
---
- ## Question
![alttext](https://github.com/dhrupad17/Backtracking/blob/main/images/Screenshot%20(142).png)
---
- ## Solution
**Code :**
```java
public class MazeCount {
    public static void main(String[] args) {
        System.out.println(count(3,3));
    }
    static int count(int r,int c)
    {
        if(r==1 || c==1)
            return 1;
        int left=count(r-1,c);
        int right=count(r,c-1);
        return left+right;
    }
}
