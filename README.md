# Task 1

* * *

## 1. Introduction

The task was to create or open an Unreal C++ Project, and to compile and run the project sucsessfully before then identifying one refelected class and one reflected property or function. This task was a first look at C++ projects rather than soly blueprints within the software, the whole goal was simple creating,opening and making simple starts within a C++ project and to become familiar with the EDI used together with Unreal.

* * *

## 2. Implementation (≈200 words)

The main engine used is Unreal engine along with Visual Studio 2022 as the EDI for a C++ project and Github with github large files for version control and cloud saving. For writing markdown both Visual studio code and a software called Typedown were used.

Demonstrating and understanding the working between two apllications, the EDI and the engine, we created a class, an actor, within Unreal which then craeted the files within the EDI. The only function that we created was a simple function that printed a string to the log when the project is compiled.

Unreal uses C++ but it's Unreal C++ therefore there is added rules, macros and systems, this required some added learning to write correct C++ so that it worked in Unreal.
'''c
    void ATestActor::SayHi(){    
      //This function uses UE_LOG To Print "Hi!"    
      UE_LOG(LogTemp, Warning, TEXT ("%s"), *FString(message));
    }
'''
Code snippet of the function for printing a string to the log.

* * *

## 3. Outcome (≈150 words)

We created two properties for the actor we created within in Unreal; a string called Message, it was created within the header file and the function, the function prints the variable Message to the log when the projet is compiled, is defined in the source file but called in the header file.

I created a new project in Unreal to use C++ rather than just blueprints and I used Visual Studio as the EDI alongside it, within in Unreal I created an actor class and then created a variable and function within the header file of the actor in the EDI.
'''c
    UPROPERTY(EditAnywhere, BlueprintReadWrite, Category = TestActor)    FString message;
'''
Code snippit of the variable called Mesage being created in the header file.

* * *

## 4. Bibliography

* _Setting Up Visual Studio Development Environment for C++ Projects in Unreal Engine | Unreal Engine 5.7 Documentation | Epic Developer Community_ (s.d.) At: [Setting Up Visual Studio Development Environment for C++ Projects in Unreal Engine | Unreal Engine 5.7 Documentation | Epic Developer Community](https://dev.epicgames.com/documentation/en-us/unreal-engine/setting-up-visual-studio-development-environment-for-cplusplus-projects-in-unreal-engine) (Accessed 03/02/2026).
* _Getting into C++ with Unreal Engine - Part1 - Setting up_ (2023) Directed by GGameDev. At: [Getting into C++ with Unreal Engine - Part1 - Setting up - YouTube](https://www.youtube.com/watch?v=dS5AUaYFcdw) (Accessed 03/02/2026).
* _Unreal Engine CPP Quick Start | Unreal Engine 5.7 Documentation | Epic Developer Community_ (s.d.) At: [Unreal Engine CPP Quick Start | Unreal Engine 5.7 Documentation | Epic Developer Community](https://dev.epicgames.com/documentation/en-us/unreal-engine/unreal-engine-cpp-quick-start) (Accessed 03/02/2026).

* * *
