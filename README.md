# PipUpgrader.py

rom tkinter import *
import os

def upgradeWIN():
    os.system('cmd /c "pip install --upgrade pip"')

def upgradeMAC():
    os.system("sudo pip3 install --upgrade pip")

window = Tk()
window.title('pip upgrader')
window.configure(background='white')
window.geometry("280x300")

Label (window, text="Click to upgrade PIP", bg="white", fg="black", font="none 20 bold") .grid(row=1, column=0, sticky=S)


Label (window, text="powered with love by Ug0ne", bg="white", fg="black", font="none 10 bold") .grid(row=2, column=0, sticky=S)


Label (window, text=" ", bg="white", fg="black", font="none 10 bold") .grid(row=3, column=0, sticky=S)
Label (window, text=" ", bg="white", fg="black", font="none 10 bold") .grid(row=4, column=0, sticky=S)
Label (window, text=" ", bg="white", fg="black", font="none 10 bold") .grid(row=5, column=0, sticky=S)
Label (window, text=" ", bg="white", fg="black", font="none 10 bold") .grid(row=6, column=0, sticky=S)


Label (window, text="Choose platform:", bg="white", fg="black", font="none 12 bold") .grid(row=7, column=0, sticky=S)

Button(window, text="upgrade on windows", width=30, command=upgradeWIN) .grid(row=8, column=0, sticky=S)

Label (window, text=" ", bg="white", fg="black", font="none 10 bold") .grid(row=9, column=0, sticky=S)

Button(window, text="upgrade on Mac/Linux", width=30, command=upgradeMAC) .grid(row=10, column=0, sticky=S)



window.mainloop()
