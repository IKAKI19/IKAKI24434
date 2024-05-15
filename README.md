import pygame
import random

# Initialize Pygame
pygame.init()

# Set up display
WIDTH, HEIGHT = 800, 600
screen = pygame.display.set_mode((WIDTH, HEIGHT))
pygame.display.set_caption("Speed Driving Game")

# Colors
WHITE = (255, 255, 255)
BLACK = (0, 0, 0)
RED = (255, 0, 0)

# Player
player_width = 50
player_height = 100
player_x = (WIDTH - player_width) // 2
player_y = HEIGHT - player_height - 50
player_speed = 5

# Enemy
enemy_width = 50
enemy_height = 50
enemy_x = random.randint(0, WIDTH - enemy_width)
