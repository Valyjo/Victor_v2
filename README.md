# Victor_v2

import pyowm

from pyowm.utils import config

from pyowm.utils import timestamps


from colorama import init

from colorama import Fore, Back, Style

# use Colorama to make Termcolor work on Windows too
init()

from subprocess import call

print (Back.MAGENTA)
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

import os
print(Back.CYAN)
print(Fore.WHITE)

text = 0

while (text < 10):
	print("______________Чего желаетe?_______________")
	text1  = input("1-video, 2-music, 3-exit, 4-other options:")
	if text1 == "4":
		break
	if text1 == "1":
		os.startfile("https://www.youtube.com/watch?v=anOApXWUS4I")

	elif text1 == "2":
		os.startfile('D:\\PROGRAMM\\MUSIC\\M.O.O.N-Crystals.mp3')
	elif text1 == "3":
		raise SystemExit(1)

	elif text1 == "4":
		test3 = 1
text3 = 0
while text3 < 10:
	print(Back.CYAN)
	print(Fore.WHITE)
	text2 = input("1-chat, 2-music_N_2, 3-exit, 4-weather:")
	
	if text2 == "1":
		print(Back.RED)
		print("это пока-что в разработке")
	
	elif text2 == "2":
		print(Back.CYAN)
		import os
		os.startfile('D:\\PROGRAMM\\MUSIC\\Lil_NasX_Jack_Harlow-INDUSTRY_BABY.mp3')

	elif text2 == "3":
		raise SystemExit(1)

	elif text2 == "4":
		print(Back.YELLOW)
		owm = pyowm.OWM("2b5bc007e2b5eae9454b4f7eddbd8e2b")
		mgr = owm.weather_manager()
		dai = input("Введите ваш город/страну:")
		observation = mgr.weather_at_place(dai)
		w = observation.weather
		temp = w.temperature("celsius")["temp"]
		print("В городе " + str(dai) + " сейчас " + str(w.detailed_status))
		print("Температура сейчас в районе|" + str(temp) + " градусов")
 
		if temp < 10:
			print("ЭЭЭ вася на улице холодно пипец, одевайся как танк")

		elif temp < 20:
			print("УУУУ на улице прохладно, одевайся потеплее")

		else:
			print("Слйшай братик на улице тепло так, что одевайся как хочешь и иди гуляй")



