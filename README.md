Please Note: I learned this before from Coding with Russ!

import pygame (this just changes how python behaves to make it easier to create games)

pygame.init() (initializes pygame)

SCREEN_WIDTH = (choose which width you want)
SCREEN_HEIGHT = (choose which height you want)

screen = pygame.display.set_mode((SCREEN_WIDTH, SCREEN_HEIGHT)) (tells pygame to show the screen and how big it is)

run = True (
while run (the code that will involve actions in the game such as a highscore or movement of a charecter)

    screen.fill((R, G, B)) (choose the colour you want)


    for event in pygame.event.get(): (event queue)
        if event.type == pygame.QUIT: (if ptgame is quit)
            run = False (Everything in this loop will stop runnning)

    pygame.display.update() (updates the screen when there is movement which is helpful in a game)

pygame.quit() (pygame closes when the loop is over which would have to heppen when run = False like in line 18)
