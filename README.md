# Victor_v2

from colorama import init
from colorama import Fore, Back, Style
# use Colorama to make Termcolor work on Windows too
init()
from subprocess import call

print (Back.YELLOW)
print("Пароль:")
age = int(input())
if age == 1215:
	print(Fore.BLACK)
	print(Back.GREEN)
	print("_______________Доступ открыт_______________\n_______________Добро пожаловать_______________")
	post = 3

else:
	print(Fore.BLACK)
	print(Back.RED)
	print("Доступ закрыт")
	input("На ваш адрес уже вызвана оперативная группа ")
	post = 0

if post > 1:
	input("_______________Нажмите любую клавишу_______________")

else:
	raise SystemExit(0)
#вот
if post > 1:
	print(Back.CYAN)
	print(Fore.WHITE)
	print("______________Чего желаетe?_______________")
	vopros = int(input("1-video, 2-music, 3-exit, 4-other options:"))

if vopros == 1: 
	post2 = 1

elif vopros == 2:
	post2 = 3

elif vopros == 3:
	post2 = 5

elif vopros == 4:
	post2 = 7

if 0 < post2 < 2:
	import os
	os.startfile("https://www.youtube.com/watch?v=anOApXWUS4I")
	text1 = input("1-chat, 2-music_N_2, 3-exit:")

elif 2 < post2 < 4:
	import os
	os.startfile('D:\\PROGRAMM\\MUSIC\\M.O.O.N-Crystals.mp3')
	text1 = input("1-chat, 2-music_N_2, 3-exit:")

elif 4 < post2 < 6:
	raise SystemExit(1)

elif 6 < post2 < 8:
	text1 = input("1-chat, 2-music_N_2, 3-exit:")

if text1 == "1":
	print(Back.RED)
	print("это пока-что в разработке")
	
elif text1 == "2":
	print(Back.CYAN)
	import os
	os.startfile('D:\\PROGRAMM\\MUSIC\\Lil_NasX_Jack_Harlow-INDUSTRY_BABY.mp3')

elif text1 == "3":
	raise SystemExit(1)

