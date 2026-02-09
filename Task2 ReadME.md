# Task 2

* * *

## 1. Introduction

We were asked to created a simple project with an actor which at least 3 of the following: OnConstruction, BeginPlay, Tick or EndPlay with some logic and to use UE_LOG() to clearly label which function is running

Instead of opening a new project I forked my last project to build on as it already had a simple actor class with a Begin play function. I had chosen to use BeginPlay, Tick and EndPlay in my project.

This project acts a slow introduction into using/creating functions which we are familiar with in blueprints but now as C++ code.

* * *

## 2. Implementation 

I used Unreal Engine and Visual Studio as my IDE for a C++ project.

Forking my past project meant my project already had an actor class in it but it wasn't empty, it already had some simple starting code to help me build from that as to not start from a blank project.

I used a BeginPlay function where the log would display a random number and I also used a Tick function to print to the log a number which incremented each tick.

I was unsure on how to use EndPlay, every source I seemed to find while searching for how to use it were a mix of vauge or not directly showing how to use it.

* * *

## 3. Outcome (≈150 words)

* State what the final result does and how it behaves

I created two variables, one which was the Result of a random number picked with a max of 100 which was called and printed to the log during BeginPlay and the other started at 0 and within the function Tick it was incrememnted and printed to the log.
```c
    void AMyActor::BeginPlay()
    {
    	Super::BeginPlay();
    	UE_LOG(LogTemp, Log, TEXT("Begin Play Function"));
    	UE_LOG(LogTemp, Log, TEXT("My Random Int Value: %lld"), Result);
    }
```
```c
    void AMyActor::Tick(float DeltaTime)
    {
    	Super::Tick(DeltaTime);
    	UE_LOG(LogTemp, Log, TEXT("Event Tick Function"));
    	number++;
    	UE_LOG(LogTemp, Log, TEXT("My Counting Int Value: %lld"), number);
    }
```
I was only able to use two of the list but they both have logic within them and in each there is a UE_LOG() to identify which function is being called.

<u>img link</u>

* * *

## 4. Bibliography

The Unreal Engine 5 Cheatsheet for blueprint nodes to C++ code:

Henning, M. (2026) _marcohenning/ue5-cheatsheet_. At: [GitHub - marcohenning/ue5-cheatsheet: A collection of Unreal Engine 5 blueprint nodes translated into C++](https://github.com/marcohenning/ue5-cheatsheet) (Accessed 09/02/2026).

* * *
