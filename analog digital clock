from turtle import Turtle, Screen
import datetime
window=Screen()
window.title("Analog digital lock")
window.bgcolor("black")
window.setup(height=800,width=800)


circle=Turtle()
circle.penup()
circle.pencolor("blue")
circle.speed(0)
circle.pensize(25)
circle.hideturtle()
circle.goto(0, -390)
circle.pendown()
circle.fillcolor("yellow")
circle.begin_fill()
circle.circle(400)
circle.end_fill()

Hhand=Turtle()
Hhand.shape("arrow")
Hhand.color("blue")
Hhand.speed(10)
Hhand.shapesize(stretch_wid=0.4,stretch_len=20)


mhand=Turtle()
mhand.shape("arrow")
mhand.color("white")
mhand.speed(10)
mhand.shapesize(stretch_wid=0.4,stretch_len=30)

shand=Turtle()
shand.shape("arrow")
shand.color("red")
shand.speed(10)
shand.shapesize(stretch_wid=0.4,stretch_len=40)

centercircle = Turtle()
centercircle.shape("circle")
centercircle.color("white")
centercircle.shapesize(stretch_wid=1.5,stretch_len=1.5)

pen=Turtle()
pen.color("blue")
pen.speed(0)

pen.penup()
pen.hideturtle()
pen.goto(170,260)
pen.write("1",align="center", font=("Times of Romans",50,"bold"))

pen.penup()
pen.hideturtle()
pen.goto(300,140)
pen.write("2",align="center",font=("Times of Romans",50,"bold"))

pen.penup()
pen.hideturtle()
pen.goto(340,-30)
pen.write("3",align="center",font=("Times of Romans",50,"bold"))

pen.penup()
pen.hideturtle()
pen.goto(300,-200)
pen.write("4",align="center",font=("Times of Romans",50,"bold"))

pen.penup()
pen.hideturtle()
pen.goto(170,-325)
pen.write("5",align="center",font=("Times of Romans",50,"bold"))

pen.penup()
pen.hideturtle()
pen.goto(0,-370)
pen.write("6",align="center",font=("Times of Romans",50,"bold"))

pen.penup()
pen.hideturtle()
pen.goto(-170,-325)
pen.write("7",align="center",font=("Times of Romans",50,"bold"))

pen.penup()
pen.hideturtle()
pen.goto(-300,-200)
pen.write("8",align="center",font=("Times of Romans",50,"bold"))

pen.penup()
pen.hideturtle()
pen.goto(-340,-30)
pen.write("9",align="center",font=("Times of Romans",50,"bold"))

pen.penup()
pen.hideturtle()
pen.goto(-280,140)
pen.write("10",align="center",font=("Times of Romans",50,"bold"))

pen.penup()
pen.hideturtle()
pen.goto(-160,260)
pen.write("11",align="center",font=("Times of Romans",50,"bold"))

pen.penup()
pen.hideturtle()
pen.goto(0,300)
pen.write("12",align="center",font=("Times of Romans",50,"bold"))

def moveHhand():
    currenthour=datetime.datetime.now().hour
    degree=(currenthour - 15)*-30
    currentminutes=datetime.datetime.now().minute
    degree=degree +  - 0.5 * currentminutes
    Hhand.setheading(degree)
    window.ontimer(moveHhand, 6000)


def movemhand():
    currentminutes = datetime.datetime.now().minute
    degree = (currentminutes - 15) * -6
    currentseconds = datetime.datetime.now().second
    degree = degree +(- currentseconds*0.1)
    mhand.setheading(degree)
    window.ontimer(movemhand, 1000)


def moveshand():
    currentsecond= datetime.datetime.now().second
    degree = (currentsecond - 15) * - 6
    shand.setheading(degree)
    window.ontimer(moveshand, 1000)


window.ontimer(moveHhand,1)
window.ontimer(movemhand, 1)
window.ontimer(moveshand, 1)
window.exitonclick()











