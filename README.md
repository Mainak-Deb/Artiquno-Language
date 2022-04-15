# **Artiquno**
### version 1.0.4
--------------------------------
![Artiquno](Artiquno.png)
------------------------------------
1. What is **Artiquno** ? 
>Namaste everyone😊 I am **Mainak Deb**, this is a programming language made by me, you can make many graphics and do normal programming tasks using this language.

2. Who am i ?
>I am a twenty years old Computer Science Student and a forever learner. I live in West Bengal, India.

3. Why i made this ?
>I made this language just for learning and fun. My professor Dr. Prabir Kumar Naskar sir inspired me a lot for this work. I had a paper **Compiler Design** in my 5th semester. There i learnt basics about compiler design . I also knew python and had some experience in developing. So i started this project.At first i wanted to make a Markup language but suddenly my attenstion went to **LOGO** which was my first programming language .So i wanted to rebuild this with some extra features .

4. Why the name Artiquno ?
>The name **Artiquno** was inspired from the pokemon Articuno. I altered the spelling to avoid the copyright.As this is a Graphic language i wanted the name Art with it.

------------------------------------------
# How to Run?
At first make a file with `.aq` extension. Then go to
the folder consists `Artiquno.exe`. Now open the `Command Prompt` on that location and do this. 
```Bash
Artiquno.exe path/filename.eq
```
# **Syntaxes**

>**Creator**
```Bash
Artiquno.exe --creator
```
--------------------------------------------

>**Version**
```Bash
Artiquno.exe --version
```
--------------------------------------------

>**Comment**
```csharp
//comment the line
```
--------------------------------------------
>**Variable**
```csharp
@VariableName; 	
```
--------------------------------------------
>**Assign Variable**
```csharp
@variable_1=[[int(7)]]; 
@variable_2=[[float(3.14)]];
@variable_3=[[str("Artiquno")]];
@variable_4=@variable_1;
```
--------------------------------------------
>**Forward**
```csharp
//type >> and then a real number
>>100;
>>-100;
>>3.14;
>>@variable;
```
--------------------------------------------

>**Backward**
```csharp
//type << and then a real number
<<100;
<<-100;
<<3.14;
<<@variable;
```
--------------------------------------------

>**Rotate**
```csharp
//type ^^ and then a angle as real number
<<100;
<<-100;
<<3.14;
<<@variable;
```
--------------------------------------------

>**Pen up**
```csharp
PU;
```
--------------------------------------------
>**Pen Down**
```csharp
PD;
```
--------------------------------------------

>**Hide Arrow**
```csharp
HIDE;
```
--------------------------------------------

>**Show Arrow**
```csharp
SHOW;
```
--------------------------------------------

>**Go To a position**
```csharp
// write X then write a real number and do the same with Y
X100Y50;
X-100Y50;
X73.89Y67.53;
X0Y0;
```
--------------------------------------------
>**Set Window size**
```csharp
// write WINDOW-X then write a positive integer and do the same with Y
WINDOW-X400Y400; 
```
--------------------------------------------
>**Set Background Color**
```csharp
// write BG-R then write a positive integer between 0-255 and do the same with G and B 
BG-R100G50B20; 
```
--------------------------------------------
>**Set Pen Color**
```csharp
// write COL-R then write a positive integer between 0-255 and do the same with G and B 
BG-R100G50B20; 
```
--------------------------------------------
>**Set Fill Color**
```csharp
// write FILL-R then write a positive integer between 0-255 and do the same with G and B 
FILL-R100G50B2; 
```
--------------------------------------------
>**Start filling**
```csharp
STARTFILL;                                        
```
--------------------------------------------
>**Stop filling**
```csharp
STOPFILL;                                        
```
--------------------------------------------
>**Pen Width**
```csharp
//type WIDTH->integer;
WIDTH->10;
```
--------------------------------------------
>**Mathematical Expression**
```csharp
@newvar=[[5*10]];
@newvar=[[sin(50)]];
@newvar=[[@newvar+1]];
@newvar=[[int(@newvar)]];                              
```
--------------------------------------------
>**Mathematical Expression*
```csharp
@newvar=[[5*10]];
@newvar=[[sin(50)]];
@newvar=[[@newvar+1]];
@newvar=[[int(@newvar)]];                              
```
--------------------------------------------
>**Speed of the pen**
```csharp
SPEED-VERYFAST;
SPEED-FAST;
SPEED-NORMAL;
SPEED-SLOW;        
```
--------------------------------------------
>**Print statement**
```csharp
WRITE->[["HELLO EVERYONE"]] ;
WRITE->[["HELLO EVERYONE"+" AND YOU"]] ;
WRITE->[["My age is "+str(20)]] ;
WRITE->[["My name is " + @name]] ;
```
--------------------------------------------
>**Input statement**
```csharp
@n=TAKE[["Enter a number: "]] ;
@n=TAKE[["Enter "+ @i +"th number: "]] ;
```
--------------------------------------------
>**Conditional statement**
```csharp
IF[[EXPRESSION]]{//CONDITION
    THEN->{
        //IF INTRUCTION
    }
    ELSE->{
        //IF INTRUCTION
    }
}

//example code
IF[[@name=="Mainak"]]{    //CONDITION
    THEN->{
        WRITE->[["I will not greet you " + @name]];
    }
    ELSE->{
        WRITE->[["Hello " + @name + "! Have a nice day"]];
    }
}
```
--------------------------------------------
>**Loop statement**
```csharp
LOOP(100){//loop
    //code here
}   

//example code
@i=[[int(0)]];
LOOP(100){
    WRITE->[[str(@i)+"\n"]];
    @i=[[@i+1]];
};
```
--------------------------------------------
>**Text statement**
```csharp
//TEXT(textsize)->[[text]]
TEXT(20)->[["WELCOME BOSS"]] 
TEXT(40)->[["Welcome boss"+" and you"]] ;
TEXT(10)->[["My age is "+str(20)]] ;
TEXT(5)->[["My name is " + @name]] ;
```
--------------------------------------------
>**BUNCH**
```csharp
 //code replacer, acts like a function but not a function, we can't any parameter to it

BUNCH->SETNAME{   
    //code here
}

```
--------------------------------------------
>**Call BUNCH**
```csharp
<SETNAME>      //call BUNCH
```
--------------------------------------------

>**Example of BUNCH**
```csharp
BUNCH->rect{ //this is a bunch of rectangle
    @size=[[int(200)]];
    >>@size;
    ^^90;
    >>@size;
    ^^90;
    >>@size;
    ^^90;
    >>@size;
};

<rect>;
>>100;

<rect>;
>>100;

<rect>;

```
--------------------------------------------


>**An example of how to run code**

--------------------------------------------
File structure
```Bash
D:.
│   Artiquno.exe
│   Artiquno.png
│   README.md
│
├───example codes
       sun.aq

```
---------------------------------------------
Example code: sun.aq

```csharp

SPEED-VERYFAST;
@i=[[int(0)]];
PU;
^^90;
<<100;
^^-90;
PD;
COL-R255G123B0;
BG-R25G217B227;
FILL-R255G255B0;

STARTFILL;
WIDTH->10;
LOOP(90){ 
        @i=[[@i+1]];
        >>10;
        ^^4;
        ^^-90;
        IF[[@i%2==0]]{
                THEN->{
                        >>20;<<20;
                }
                ELSE->{
                      >>40;   <<40;
                }
        };
        
        
        ^^90;
};    
ENDFILL;
COL-R255G0B0;
PU;
X-80Y-80;
PD;
TEXT(60)->[["SUN"]];
 
```
---------------------------
Run code
```Bash
Artiquno.exe "example codes\sun.aq"
```
Output:
![sun_output](https://raw.githubusercontent.com/Mainak-Deb/Artiquno_dist/master/images/sun_output.png)

