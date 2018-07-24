# Sonic-Animation
def setup():
    size(1000,1000)
    global imageList, imageIndex
    imageIndex = 0
    imageList = [loadImage("Sonic1.png"),loadImage("Sonic2.png"),loadImage("Sonic3.png"),loadImage("Sonic2.png"),loadImage("Sonic1.png"),loadImage("Sonic5.png"),loadImage("Sonic6.png"),loadImage("Sonic5.png")]

def draw():
    global imageList, imageIndex
    image(imageList[imageIndex],20,50,35,50)
    if frameCount%50 == 0:
     imageIndex= imageIndex + 1
     imageIndex = imageIndex%len(imageList)
