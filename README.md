# Reloj_Unico
Se realizara un reloj único hecho por Juan Sebastian Daza

y_position = 0
color_is = False
def setup():
    size(600,610)
    
def draw():
    global y_position 
    background(30)
    if color_is == True:
       fill(0, 100, 0)
    else:
       fill(20, 60, 200)

    ellipse(width /1.15, y_position, 50, 50)
    if y_position > height:
       y_position = 0
    else:
       y_position = map(second(), 0, 59, 0, height)


    ellipse(width / 5, y_position, 50, 50)
    if y_position > height:
       y_position = 0
    else:
       y_position = map(minute(), 0, 59, 0, height)
       
    ellipse(width / 1.85, y_position, 50, 50)
    if y_position > height:
       y_position = 0
    else:
       y_position = map(hour(), 0, 200, 0, height)

    textSize(25)
    text("15",0,149)
    textSize(20)
    text("30",0,299)
    textSize(20)
    text("45",0,449)
    textSize(20)
    text("59",0,599)
    textSize(20)
    text("1",425,49)
    textSize(20)
    text("2",425,74)
    textSize(20)
    text("3",425,99)
    textSize(20)
    text("4",425,124)
    textSize(20)
    text("5",425,149)
    textSize(20)
    text("6",425,174)
    textSize(20)
    text("7",425,199)
    textSize(20)
    text("8",425,224)
    textSize(20)
    text("9",425,249)
    textSize(20)
    text("10",425,274)
    textSize(20)
    text("11",425,299)
    textSize(20)
    text("12",425,324)
    textSize(20)
    text("13",425,349)
    textSize(20)
    text("14",425,374)
    textSize(20)
    text("15",425,399)
    textSize(20)
    text("16",425,424)
    textSize(20)
    text("17",425,449)
    textSize(20)
    text("18",425,474)
    textSize(20)
    text("19",425,499)
    textSize(20)
    text("20",425,524)
    textSize(20)
    text("21",425,549)
    textSize(20)
    text("22",425,574)
    textSize(20)
    text("23",425,599)
def mousePressed():
    global color_is
    color_is = not color_is