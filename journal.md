#This is the journal for Comp Sci

Jan 30th Thu
1. What did we do?
We did an activity of making Dr. Ruben make a jam sandwich. Each step was taken seriously and one lacking part or vague information would make the step not work

1. What did you learn?
I learned that making the steps to vague or to specific leads to a problem in the program.

1. What questions do I have?
I want to learn how to judge what the information that needs to be told is and how you can give percise information in the program

Feb 11th Tue
1. What did we do?
We made circles and squares with a code that would allow us to use a dice on our computer. 

1. What did you learn?
I learned how to make squares with curved edges, circles, and how to use the if to make the dice function

1. What questions do I have?
I want to be able to do the programming more quickly so I can make more complex patters (How I can achieve this?)

Feb 13th Thurs
1. What did we do?
We updated the dice. We put a bargraph so that we can look at the infomation/data moe quickly and we also changed the colors of different things.

#These variables are to count the rools of the divice

ones=0
twos=0
threes=0
fours=0
fives=0
sixes=0

def setup():
    size(600,600)

def draw():
    #White background
    x=0
    delay(50)
    mouseClick()
    barGraph()

    
def barGraph():
    global ones
    fill(0)
    textSize(20)
    for x in range (6):
        text(x+1,(50+50*x),580)
   
    stroke(255,0,0)
    fill(255,0,0)
    rect(45,550 - ones, 20, ones)
    
    fill(255,100,0)
    stroke(255,100,0)
    rect(95,550 - twos, 20, twos)
    
    stroke(255,230,0)
    fill(255,230,0)
    rect(145,550 - threes, 20, threes)
    
    stroke(0,255,0)
    fill(0,255,0)
    rect(195,550 - fours, 20, fours)
    
    stroke(0,0,255)
    fill(0,0,255)
    rect(245,550 - fives, 20, fives)
    
    stroke(255,0,255)
    fill(255,0,255)
    rect(295,550 - sixes, 20, sixes)


def mouseClick():
    global ones, twos, threes, fours, fives, sixes
    fill(255)
    background(255)
    stroke(0)
    strokeWeight(2)
    rect(100,100,400,400,10)
    stroke(200,230,50)
    strokeWeight(5)

    n = random(0,6)
    if 0<=n<1:
        stroke(255,0,0)
        circle(300,300,50)
        ones= ones + 1
        print("Number or times one has been rolled:",ones)

    if 1<=n<2:
        circle(200,200,50)
        circle(400,400,50)
        twos= twos + 1
        print("Number or times twos has been rolled:",twos)

    if 2<=n<3:
        circle(200,200,50)
        circle(400,400,50)
        circle(300,300,50)
        threes= threes + 1
        print("Number or times threes has been rolled:",threes)
    
    if 3<=n<4:
        circle(200,200,50)
        circle(400,200,50)
        circle(200,400,50)
        circle(400,400,50)
        fours= fours + 1
        print("Number or times fours has been rolled:",fours)
        
    if 4<=n<5:
        circle(200,200,50)
        circle(400,400,50)
        circle(200,400,50)
        circle(400,200,50)
        circle(300,300,50)
        fives= fives + 1
        print("Number or times fives has been rolled:",fives)

    if 5<=n<6:
        circle(200,400,50)
        circle(400,200,50)
        circle(200,300,50)
        circle(400,300,50)
        circle(200,200,50)
        circle(400,400,50)
        sixes= sixes + 1
        print("Number or times sixes has been rolled:",sixes)

1. What did you learn?
I learned how to code bargraphs and I also learned how to put in loops/patters (for x in range)

1. What questions do I have?
I want to learn how to be able to make colors quickly. Also to be able to make the loops more quickly

