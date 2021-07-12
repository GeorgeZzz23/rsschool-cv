## Name: Giorgi 
## Surname: Gogokhia
## Contact Info : (+995)551 31-22-04, gogokhiagio23@gmail.com, 19200200@ibsu.edu.ge.
---
---

## Summary
 Since 2018, when I started studying at the International Black Sea University, I have always wanted to find my path in information technologies, I have tried multiple things: Mobile applications, Computer Archutechture, Computer networks, Graphical design, etc but none of them have been as satisfying and interesting to work on as **web development** , I have studied it for a year in my university and have reached one of the highest points in my group, so I have narrowed my possible field of education down to a few things one of them being web development,I have no experience of working as a web developer in a working environement but as I have already mentioned **I have passed "Web programming 1" and "Web programming 2" english courses in my university**, I also have a longer experience with coding in general, I have been coding since 2016, I have also passed courses such as advanced Python programming, Angular JS, Javascript and many more, my main goal in life is to create a career that requires me to do a job that I enjoy doing and I'm hoping to get the necessary information out of this course to help me get to the next level.


## Skills: 
* Information technologies Knowledge:
    * Advanced Python programming
    * object-oriented programming knowledge
    * Mid-level Javascript, HTML, CSS, PHP knowledge
    * Mid-level SQL knowledge 
    * experience with Angular JS
* Language Skills: 
    * English C1 level (Toefl standard) from a test conducted in 2018 in the International Black Sea University.
* Personal skills:
    * hard working
    * competitive 
    * willing to learn and get better.


## Code Examples: 

```python
from tkinter import *
from tkinter import messagebox

window = Tk()

window.title("Welcome to Amit Tic-Tac-Toe ")
window.geometry("400x300")

lbl = Label(window, text="Tic-tac-toe Game", font=('Helvetica', '15'))
lbl.grid(row=0, column=0)
lbl = Label(window, text="Player 1: X", font=('Helvetica', '10'))
lbl.grid(row=1, column=0)
lbl = Label(window, text="Player 2: O", font=('Helvetica', '10'))
lbl.grid(row=2, column=0)

turn = 1  # For first person turn.


def clickedproccessing():
    global turn
    if turn == 1:
        turn = 2
        return "X"
    elif turn == 2:
        turn = 1
        return "O"


def clicked1():
    global turn
    if btn1["text"] == " ":  # For getting the text of a button
        btn1["text"] = clickedproccessing()
        check()


def clicked2():
    global turn
    if btn2["text"] == " ":
        btn2["text"] = clickedproccessing()
        check()


def clicked3():
    global turn
    if btn3["text"] == " ":
        btn3["text"] = clickedproccessing()
        check()


def clicked4():
    global turn
    if btn4["text"] == " ":
        btn4["text"] = clickedproccessing()
        check()


def clicked5():
    global turn
    if btn5["text"] == " ":
        btn5["text"] = clickedproccessing()
        check()


def clicked6():
    global turn
    if btn6["text"] == " ":
        btn6["text"] = clickedproccessing()
        check()


def clicked7():
    global turn
    if btn7["text"] == " ":
        btn7["text"] = clickedproccessing()
        check()


def clicked8():
    global turn
    if btn8["text"] == " ":
        btn8["text"] = clickedproccessing()
        check()


def clicked9():
    global turn
    if btn9["text"] == " ":
        btn9["text"] = clickedproccessing()
        check()


def check():
    global flag
    b1 = btn1["text"] # Getting value from each button,
    b2 = btn2["text"] # to check for any possible win event
    b3 = btn3["text"]
    b4 = btn4["text"]
    b5 = btn5["text"]
    b6 = btn6["text"]
    b7 = btn7["text"]
    b8 = btn8["text"]
    b9 = btn9["text"]
    flag += 1
    # Check every possible win on map
    if b1 == b2 and b1 == b3 and b1 == "O" or b1 == b2 and b1 == b3 and b1 == "X":
        win(b1)
    if b4 == b5 and b4 == b6 and b4 == "O" or b4 == b5 and b4 == b6 and b4 == "X":
        win(b4)
    if b7 == b8 and b7 == b9 and b7 == "O" or b7 == b8 and b7 == b9 and b7 == "X":
        win(b7)
    if b1 == b4 and b1 == b7 and b1 == "O" or b1 == b4 and b1 == b7 and b1 == "X":
        win(b1)
    if b2 == b5 and b2 == b8 and b2 == "O" or b2 == b5 and b2 == b8 and b2 == "X":
        win(b2)
    if b3 == b6 and b3 == b9 and b3 == "O" or b3 == b6 and b3 == b9 and b3 == "X":
        win(b3)
    if b1 == b5 and b1 == b9 and b1 == "O" or b1 == b5 and b1 == b9 and b1 == "X":
        win(b1)
    if b7 == b5 and b7 == b3 and b7 == "O" or b7 == b5 and b7 == b3 and b7 == "X":
        win(b7)
    elif flag == 9:
        messagebox.showinfo("DRAW !", "DRAW")
        window.destroy()


def win(player):
    ans = "Game complete, player " + player + " wins !!!"
    messagebox.showinfo("WIN !!!", ans)
    window.destroy()  # is used to close the program


btn1 = Button(window, text=" ", bg="green", fg="Black", width=3, height=1, font=('Helvetica', '20'), command=clicked1)
btn1.grid(column=1, row=1)
btn2 = Button(window, text=" ", bg="green", fg="Black", width=3, height=1, font=('Helvetica', '20'), command=clicked2)
btn2.grid(column=2, row=1)
btn3 = Button(window, text=" ", bg="green", fg="Black", width=3, height=1, font=('Helvetica', '20'), command=clicked3)
btn3.grid(column=3, row=1)
btn4 = Button(window, text=" ", bg="green", fg="Black", width=3, height=1, font=('Helvetica', '20'), command=clicked4)
btn4.grid(column=1, row=2)
btn5 = Button(window, text=" ", bg="green", fg="Black", width=3, height=1, font=('Helvetica', '20'), command=clicked5)
btn5.grid(column=2, row=2)
btn6 = Button(window, text=" ", bg="green", fg="Black", width=3, height=1, font=('Helvetica', '20'), command=clicked6)
btn6.grid(column=3, row=2)
btn7 = Button(window, text=" ", bg="green", fg="Black", width=3, height=1, font=('Helvetica', '20'), command=clicked7)
btn7.grid(column=1, row=3)
btn8 = Button(window, text=" ", bg="green", fg="Black", width=3, height=1, font=('Helvetica', '20'), command=clicked8)
btn8.grid(column=2, row=3)
btn9 = Button(window, text=" ", bg="green", fg="Black", width=3, height=1, font=('Helvetica', '20'), command=clicked9)
btn9.grid(column=3, row=3)

flag = 0  # Flag used to apeend (1) in every turn is occurred

window.mainloop()
```


## Experience: 
* 5 year-long experience with coding
* 1 year-long course in python(including object-oriented programming)
* 1 year course for web programming,
* 1year course for sql,
* half a semester course for angular js,
* Operating Systems,
* mobile applications,

 projects at the end of all of the above-mentioned courses in order to pass and/or receive higher points.


## Education: 
1. *School education*: General information about Infomation technologies
1. *University education*: SQL, Python programming 1-2, Introduction to AI, Computer Architecture, Angular JS, Fundamentals of Electronics, Statistics with Programming, Data Structure and Algorithms 1-2, Operating Systems, Java Programming, Web programming 1-2, Cyber Security Essentials, Arduino Programming, Computer Communication and Networks, Mobile Applications.
1. *Personal online education*: w3resource.com (python, html, css, c++ exercises), [Thenewboston](https://www.youtube.com/user/thenewboston) - youtube channel(python, html, css, c++, sql courses)
___

![Markdown Logo](https://ibsu.edu.ge/wp-content/uploads/2020/02/logo-1.svg)
___

## English: 
>I have been speaking to American, British people and other foreigners in English since I was 12 years old, studied English at school for 7 years, I received a c1 level grade after completing a toefl official test in the International Black Sea University upon entering the university in 2018,  where I have just recently completed my third year in a faculty where teaching is conducted in english, I have taught English language to adults at an academy in Tbilisi for over a year as my first job