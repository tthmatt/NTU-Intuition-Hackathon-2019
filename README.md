# NTU-Intuition-Hackathon-2019

from mblock import event
import time

def lineFollow():
    if 0 < 6:
        if sprite.get_variable('moveSpeed') > 230:
            sprite.set_variable('moveSpeed', 230)

        sprite.set_variable('lineFollowerSensor', 0)
        if sprite.get_variable('lineFollowerSensor') == 0:
            forward()
            sprite.set_variable('lineDirIndex', 10)

        else:
            if sprite.get_variable('lineFollowerSensor') == 1:
                forward()
                if sprite.get_variable('lineDirIndex') > 1:
                    sprite.set_variable('lineDirIndex', ((sprite.get_variable('lineDirIndex') - 1)))


            else:
                if sprite.get_variable('lineFollowerSensor') == 2:
                    forward()
                    if sprite.get_variable('lineDirIndex') < 20:
                        sprite.set_variable('lineDirIndex', ((sprite.get_variable('lineDirIndex') + 1)))


                else:
                    if sprite.get_variable('lineDirIndex') == 10:
                        turnLeft()

                    if sprite.get_variable('lineDirIndex') < 10:
                        turnLeft()

                    if sprite.get_variable('lineDirIndex') > 10:
                        turnRight()





    if False:
        if sprite.get_variable('moveSpeed') > 230:
            sprite.set_variable('moveSpeed', 230)

        sprite.set_variable('lineFollowerSensor', 0)
        if sprite.get_variable('lineFollowerSensor') == 0:
            forward()
            sprite.set_variable('lineDirIndex', 10)

        else:
            if sprite.get_variable('lineFollowerSensor') == 1:
                forward()
                if sprite.get_variable('lineDirIndex') > 1:
                    sprite.set_variable('lineDirIndex', ((sprite.get_variable('lineDirIndex') - 1)))


            else:
                if sprite.get_variable('lineFollowerSensor') == 2:
                    forward()
                    if sprite.get_variable('lineDirIndex') < 20:
                        sprite.set_variable('lineDirIndex', ((sprite.get_variable('lineDirIndex') + 1)))


                else:
                    if sprite.get_variable('lineDirIndex') == 10:
                        turnRight()

                    if sprite.get_variable('lineDirIndex') < 10:
                        turnLeft()

                    if sprite.get_variable('lineDirIndex') > 10:
                        turnRight()





    if 0 > 8:
        if sprite.get_variable('moveSpeed') > 230:
            sprite.set_variable('moveSpeed', 230)

        sprite.set_variable('lineFollowerSensor', 0)
        if sprite.get_variable('lineFollowerSensor') == 0:
            forward()
            sprite.set_variable('lineDirIndex', 10)

        else:
            if sprite.get_variable('lineFollowerSensor') == 1:
                forward()
                if sprite.get_variable('lineDirIndex') > 1:
                    sprite.set_variable('lineDirIndex', ((sprite.get_variable('lineDirIndex') - 1)))


            else:
                if sprite.get_variable('lineFollowerSensor') == 2:
                    forward()
                    if sprite.get_variable('lineDirIndex') < 20:
                        sprite.set_variable('lineDirIndex', ((sprite.get_variable('lineDirIndex') + 1)))


                else:
                    if sprite.get_variable('lineDirIndex') == 10:
                        turnLeft()

                    if sprite.get_variable('lineDirIndex') < 10:
                        turnLeft()

                    if sprite.get_variable('lineDirIndex') > 10:
                        turnRight()







@event.greenflag
def on_greenflag():
    sprite.set_variable('moveSpeed', 100)
    sprite.set_variable('lineDirIndex', 10)
    while not False:
        sprite.say('')
        sprite.set_variable('dist', 0)
        if False:
            obstacleAvoidance()

        else:
            lineFollow()




def obstacleAvoidance():
    turnLeft()
    time.sleep(0.6)
    stop()
    makeCircle()


def makeCircle():
    while not 0 < 3:
        pass

    stop()


def forward():
    pass

def turnRight():
    pass

def turnLeft():
    pass

def backward():
    pass

def stop():
    pass
