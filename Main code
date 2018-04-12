# Maze-and-dragons

import pygame

pygame.init()

win = pygame.display.set_mode((500,500))
pygame.display.set_caption("Test Game")

x = 50
y = 50
width = 40
height = 60
move_speed = 5

running = True
while running:
    pygame.time.delay(50)

    for event in pygame.event.get():
        if event.type == pygame.QUIT:
            running = False


    key = pygame.key.get_pressed()
    if key[pygame.K_ESCAPE]:
        pygame.quit()
    if key[pygame.K_a]:
        x -= move_speed
    if key[pygame.K_d]:
        x += move_speed
    if key[pygame.K_w]:
        y -= move_speed
    if key[pygame.K_s]:
        y += move_speed

    win.fill((0,0,0))
    pygame.draw.rect(win, (0,240,0), (x, y, width, height))
    pygame.display.update()



pygame.quit()
