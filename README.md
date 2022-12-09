# week1

- [x] 重新调整vim以适应rust的开发

- [x] 阅读rust语言圣经到2.5节的内容

- [x] rustlings 18/94 成到quiz1之后

# week2

## day1 
- [x] rustlings 32/94

## day2
- [x] 今天在赶学校ddl

## day3
- [x] rustlings 45/94

- [] 完成rustlings的练习

- [] 阅读rust语言圣经到2.14

# week3

🕊️了第二周的记录，本来计划第二周写完的，然而计划赶不上变化，突然新加了大实验，被迫赶了三天大实验，本周总算完成了全部的rustlings题目

- [x] rustlings 94/94
- [x] 阅读rust语言圣经到3.10

接下来因为之前学过了riscv相关的知识，所以要开始正式的os实验了

# week4

## day2

查看了github ci运行的结果，发现本地运行没问题的94/94 在ci中只有92/94 经过详细的排错（比较费眼），找到了有问题的四个题目，分别是intro2，clippy1，clippy2，问题如下：

- clippy1 ```use core::f32::consts::PI;``` -> ```//use core::f32::consts::PI; let pi=f32::consts::PI;``` 
- clippy2 ```while let Some(x)=option{...}``` -> ```if let Some(x)=option{...}```


# week emmmm? i forgot but today is 2022/12/9

## friday
🕊️了好久，一部分是因为期末，另外一部分还是因为期末 😭😭😭

上次写了一点lab1但没有记录日志，现在所有的课程都转线上了，我继续来加上。

上次写了lab1 然而，我发现如果我设定每一个task都有一个500*i32的数组来记录系统调用次数时，就会出现一些比较奇怪的问题，后来在mail list看到了相关的解决方案，然后今天做了修正。

此外由于我使用Rfcell的不严谨，在使用了可变借用的时候，又使用了不可变借用，导致出现了panic，现在已经修好了。
