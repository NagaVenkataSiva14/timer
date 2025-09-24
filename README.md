from tkinter import *
from tkinter.ttk import *
from time import strftime
b =Tk()
b.title('BigBoss clock')
def time():
    string = strftime('%d %B %y, %I:%M:%S %p')
    lbl.config(text=string)
    lbl.after(100, time)
lbl = Label(b,font=('ARIAL',40,'bold'),
            background = 'red',
            foreground = 'black')
lbl.pack(anchor ='center')
time()
mainloop()
